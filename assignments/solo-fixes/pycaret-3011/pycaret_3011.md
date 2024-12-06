# Fixing Fold Number Calculation and Validation Issues ([Issue #3011](https://github.com/pycaret/pycaret/issues/3011))

**Author**: Mehedi Hasan Sizar  
**Date**: 12/05/2024  
**Forked Repository**: [https://github.com/mhsizar/pycaret](https://github.com/mhsizar/pycaret)  

## **Project**: [PyCaret](https://github.com/pycaret/pycaret)

### **Issue Overview**

&rarr; **Issue**: The `fold` parameter in PyCaret's time series module accepts non-integer values, such as custom cross-validation (CV) objects, leading to incorrect behavior and inconsistent fold numbers in the output.  
&rarr; **Goal**: Ensure that the `fold` parameter only accepts integers and that CV objects are passed to the `fold_strategy` parameter as per the documentation.

---

### **Steps Taken to Resolve the Issue**

1. **Initial Group Solution**:  
   As part of the group, we focused on fixing the incorrect fold number display in the `_set_fold_generator` function by calculating the fold count dynamically for CV objects passed to `fold`. The group assumed that accepting CV objects in `fold` was an expected behavior and sought to fix the fold count calculation logic directly.

   **Why I Switched to a New Solution**:  
   Upon reviewing the official PyCaret [documentation](), I realized that the group’s assumption was incorrect. The documentation explicitly states that the `fold` parameter must accept only integers and that custom CV objects like `ExpandingWindowSplitter` must be passed to the `fold_strategy` parameter instead. The existing behavior of accepting CV objects in `fold` was therefore unintended and required a stricter validation mechanism.  

2. **Validation for `fold` Parameter**:  
   - Added a type check in the `setup()` function to raise a `TypeError` when a non-integer is passed to `fold`.
   - Provided a clear error message to guide users to use `fold_strategy` for custom CV objects.

   **Code snippet**:  
   ```python
   # Validate fold
   if not isinstance(fold, int):
       raise TypeError(
           f"The 'fold' parameter must be an integer. You provided: {type(fold).__name__}. "
           "If you intended to use a custom cross-validation object such as SlidingWindowSplitter or "
           "ExpandingWindowSplitter, please pass it to the 'fold_strategy' parameter instead. "
           "The 'fold' parameter is ignored when 'fold_strategy' is a custom CV object."
       )
   ```

3. **Updated `_set_fold_generator` Logic**:  
   - Simplified the logic to handle `fold` and `fold_strategy` correctly, ensuring consistent behavior when the parameters are used as intended.

4. **Test Case Updates**:  
   - Modified test cases to validate the new behavior.
   - Ensured the `Fold Number` and `Fold Generator` values in the setup summary align with the documentation.

---

### **Why the New Solution Is Better**

- **Compliance with Documentation**:  
  The updated solution enforces the behavior described in the PyCaret documentation, improving consistency and reducing confusion for users.  

- **Error Handling**:  
  By raising a `TypeError` for invalid `fold` inputs, the solution prevents silent failures and provides clear guidance to users on the correct usage of `fold` and `fold_strategy`.

- **Future-proofing**:  
  This solution prevents further issues related to misuse of the `fold` parameter and aligns with the best practices of strict parameter validation.

---

### **Outcome**

The changes address the issue by:  
- Enforcing type safety for the `fold` parameter.  
- Clarifying expected usage of `fold` and `fold_strategy`.  
- Aligning the behavior with PyCaret's documentation.  

These updates prevent users from misusing parameters and improve output accuracy.  

Pull request: [PR #4104](https://github.com/pycaret/pycaret/pull/4104)

---

### **Example Usage**  

Here’s how the `setup()` function should now be used:

```python
import numpy as np
from pycaret.time_series import TSForecastingExperiment
from pycaret.datasets import get_data
from sktime.forecasting.model_selection import ExpandingWindowSplitter

# Load dataset
y = get_data(114, folder="time_series/seasonal", verbose=False)

# Define a custom cross-validation strategy
cv = ExpandingWindowSplitter(fh=np.arange(1, 13), initial_window=24, step_length=4)

# Initialize and setup experiment
exp = TSForecastingExperiment()
exp.setup(y, fh=12, fold_strategy=cv)  # Correct usage
```

For incorrect usage, such as passing `cv` to `fold`, the function now raises an error:

```plaintext
TypeError: The 'fold' parameter must be an integer. You provided: ExpandingWindowSplitter. 
If you intended to use a custom cross-validation object such as SlidingWindowSplitter or 
ExpandingWindowSplitter, please pass it to the 'fold_strategy' parameter instead. 
The 'fold' parameter is ignored when 'fold_strategy' is a custom CV object.
```

This provides clarity to the users and enforces proper parameter usage.  
