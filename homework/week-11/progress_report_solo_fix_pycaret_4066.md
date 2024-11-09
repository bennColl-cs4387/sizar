# Solo Fix Progress Report (Week-11)
*Author: Mehedi Hasan Sizar*  
*Date: 11/09/2022*

## Project: [PyCaret](https://github.com/pycaret/pycaret)

&rarr; **Issue**: Making plotting dependencies optional in PyCaret ([Issue #4066](https://github.com/pycaret/pycaret/issues/4066)).  
&rarr; **Goal**: Move heavy plotting libraries (`plotly`, `kaleido`, etc.) to an optional dependency section to reduce the installation time and size for users who do not require visualization features.  

### Progress Overview
- **Understanding the Issue**: Spent time analyzing the current handling of decependencies in `requirements.txt` and `requirements-optional.txt` files.
- **Plan Development**: Developed a plan to relocate plotting libraries to a new section in `requirements-optional.txt` and adjust the `setup.py` file to expose these as optional dependencies.
- **Implementation**: 
    - Moved plotting dependencies to `requirements-optional.txt` file. 
    - Need to update the `setup.py` file to include a `"plots"` key in the `extras_require` disctionary for easy installation. 
- **Code Adjustments**: Need to add additional imports and cross validations in the codebase to handle cases where plotting libraries are not installed, ensuring user-friendly error message are raised when needed. 

### Challenges
- **Dependency Management**: Understanding the interaction between different parts of PyCaret that rely on plotting libraries.
- **Fix Reliability**: Ensuring no disruptions occur in workflows that do not require visualization. 
- **Codebase Familiarity**: Getting more familiar with the structure of PyCaret to identify where changes are needed and to match the structure in the fixes. 

### Timeline
- **Initital Research & Planning**: Completed
- **Implementation**: In progress
- **Testing & Documentation**: Upcoming
- **Pull Request Submission**: Targeting within week-13. 