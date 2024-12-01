# Solo Fix Progress Report (Week-13)
*Author: Mehedi Hasan Sizar*  
*Date: 11/25/2024*  

## Project: [PyCaret](https://github.com/pycaret/pycaret)

&rarr; **Issue**: Making plotting dependencies optional ([Issue #4066](https://github.com/pycaret/pycaret/issues/4066)).  
&rarr; **Goal**: Move plotting libraries to an optional dependency section and update the installation process.

---

### Progress Overview

- **Completed Tasks**:
  - Moved over plotting libraries from `requirements.txt` to `requirements-optional.txt` to separate visualization tools from the core PyCaret installation.
  - Updated `setup.py` to include a `plots` key in `extras_require` for optional plotting installation.
  - Verified installation and error handling workflows for users with and without the optional plotting dependencies.
  - [Documented the fix](https://github.com/bennColl-cs4387/sizar/tree/main/assignments/solo-fixes/pycaret-4066) and submitted [Pull Request #4102](https://github.com/pycaret/pycaret/pull/4102).

- **Learnings**:
  - Gained experience in managing Python dependencies through `setup.py`.
  - Understood the importance of clear error messages and documentation in improving user experience.

### Status Update

All tasks related to this issue have been completed, and the pull request is under review by PyCaret maintainers.