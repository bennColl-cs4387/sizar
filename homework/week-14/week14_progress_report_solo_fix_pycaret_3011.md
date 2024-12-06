# Solo Fix Progress Report (Week-14)
*Author: Mehedi Hasan Sizar*
*Date: 12/05/2024*

## Project: [PyCaret](https://github.com/pycaret/pycaret)

&rarr; **Issue**: Fixing incorrect fold number calculation and validation of the `fold` parameter ([Issue #3011](https://github.com/pycaret/pycaret/issues/3011)).  
&rarr; **Goal**: Ensure `fold` parameter accepts only integers, and cross-validation objects are passed correctly to the `fold_strategy` parameter.

---