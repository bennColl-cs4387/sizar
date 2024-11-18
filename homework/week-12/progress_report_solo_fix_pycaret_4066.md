# Solo Fix Progress Report (Week-12)
*Author: Mehedi Hasan Sizar*  
*Date: 11/17/2024*

## Project: [PyCaret](https://github.com/pycaret/pycaret)

&rarr; **Issue**: Making plotting dependencies optional in PyCaret ([Issue #4066](https://github.com/pycaret/pycaret/issues/4066)).  
&rarr; **Goal**: Relocate heavy plotting libraries (`plotly`, `kaleido`, etc.) to an optional dependency section in order to optimize installation time and size for users who do not require visualization features.

---

### Progress Overview
- **Completed Steps**:
  - **Refactoring Dependencies**: Successfully moved plotting libraries from `requirements.txt` to `requirements-optional.txt` to separate visualization tools from the core PyCaret installation.
  - **Updating `setup.py`**: 
    - Introduced a `"plots"` key in the `extras_require` dictionary to enable optional installation via `pip install pycaret[plots]`.
    - Ensured all adjustments are consistent with the existing structure and practices of the PyCaret project.
  - **Uninstall and Reinstall Testing**: Verified installation behavior with and without the optional dependencies to ensure the modification worked as intended.
- **In Progress**:
  - **Error Handling**: Modifying relevant code sections to raise meaningful errors when plotting libraries are missing and provide clear instructions for users to install them.
  - **Comprehensive Testing**: Implementing test cases to confirm that PyCaret remains functional when the optional plotting dependencies are not installed.

### Challenges & Learnings
- **Managing Dependencies**: It is challenging to identify all points in the codebase where plotting libraries are used and ensuring graceful failure when dependencies are absent.
- **Understanding the Codebase**: The process requires a deeper understanding of how PyCaret integrates visualization, necessitating additional time for research and testing.
- **Ensuring Backward Compatibility**: Need to ensure that the proposed changes do not disrupt workflows for existing PyCaret users.

### Next Steps
- **Complete Error Handling**: Finalize and test error handling mechanisms to enhance user experience.
- **Write Documentation**: Update PyCaret’s documentation to guide users on how to install the plotting dependencies if needed.
- **Submit Pull Request**: Aim to have a complete and thoroughly tested pull request ready for review by the end of Week-13.