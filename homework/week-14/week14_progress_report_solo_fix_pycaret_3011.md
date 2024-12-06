# Solo Fix Progress Report (Week-14)
*Author: Mehedi Hasan Sizar*
*Date: 12/05/2024*

## Project: [PyCaret](https://github.com/pycaret/pycaret)

&rarr; **Issue**: Fixing incorrect fold number calculation and validation of the `fold` parameter ([Issue #3011](https://github.com/pycaret/pycaret/issues/3011)).  
&rarr; **Goal**: Ensure `fold` parameter accepts only integers, and cross-validation objects are passed correctly to the `fold_strategy` parameter.

---

### Progress Overview

- **Completed Tasks**:
  - Updated the `setup()` function in `oop.py` to validate the `fold` parameter and ensure only integers are allowed. 
  - Added a `TypeError` for cases where a non-integer value is passed to the `fold` parameter, and instructing users to use the `fold_strategy` parameter instead.

- *Learnings**:
  - Understood the implications of passing CV objects to the wrong parameter, leading to incorrect behavior and confusion in fold count.
  - Gained clarity on PyCaret's design for separating integer folds (`fold`) from CV objects (`fold_strategy`).
  - Improved skills in debugging and identifying the root causes of parameter handling issues in Python libraries.

- **Why I switched from the group solution**:
  - The initial group solution did not validate the `fold` parameter type, leading to potential misuse when CV objects were incorrectly passed to it.
  - This solo fix ensures stricter type checking and provides a clear error message to guide users, addressing the core issue.

---

### Status Update

All tasks related to this issue have been completed, and the pull request has been created: [Pull Request #4104](https://github.com/pycaret/pycaret/pull/4104). Awaiting review and feedback from PyCaret maintainers.