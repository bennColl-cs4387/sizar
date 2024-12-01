# Making Plotting Dependencies Optional in PyCaret ([Issue #4066](https://github.com/pycaret/pycaret/issues/4066))

*Author: Mehedi Hasan Sizar*  
*Date: 12/01/2024*  
*Forked Repository: [https://github.com/mhsizar/pycaret](https://github.com/mhsizar/pycaret)*  

## Project: [PyCaret](https://github.com/pycaret/pycaret)

### Issue Overview

&rarr; **Issue**: Optimize PyCaret installation by moving heavy plotting libraries like `plotly` and `kaleido` into an optional dependency section ([Issue #4066](https://github.com/pycaret/pycaret/issues/4066)).  
&rarr; **Goal**: Allow users to opt-in for visualization features by specifying `[plots]` during installation, reducing default installation size and time for users who doesn't need visualization tools.

---

### Steps Taken to Resolve the Issue

1. **Refactored Dependencies**:
   - Moved plotting-related libraries from `requirements.txt` to the optional dependecy file, `requirements-optional.txt`.
   - Updated `setup.py` to include a `plots` key in `extras_require` to allow users installed the plotting libraries using `pip install pycaret[plots]` command.

2. **Tested Changes**:
   - Verified installations with and without the optional `[plots]` dependency.
   - Confirmed PyCaret raises meaningful errors when plotting libraries are missing.

### Outcome

These changes provide a lighter default installation and improve flexibility for PyCaret users. See the pull request here: [PR #4102](https://github.com/pycaret/pycaret/pull/4102).