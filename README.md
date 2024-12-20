# Mehedi Hasan Sizar ([@mhsizar](https://github.com/mhsizar))  

Hi, I am Sizar, a rising senior (graduating December, 2025) at Bennington College concentrating in Computer Science and Mathematics. My primary areas of interest lie in data science, machine learning, and software development. Check out my [GitHub](https://github.com/mhsizar) and let's get connected on [LinkedIn](https://www.linkedin.com/in/mhsizar/)!  
 
---

## CS 4387:Open Source Software in Practice: 

&rarr; [Course Syllabus](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-03/class_syllabus.md)

I took this course to gain hands-on experience contributing to open-source projects (especially related to AI/ML), improve my programming skills, and learn how collaborative development can solve real-world problems. Here are some work I have done in this class: 

## Solo Fixes

### 1. [Making Plotting Dependencies Optional](https://github.com/pycaret/pycaret/issues/4066)  
Moved plotting-related dependencies in PyCaret to an optional section, making installation smaller and faster. This included editing `requirements.txt`, updating `setup.py`, and handling missing dependencies gracefully.  

Progress Reports: Progress Reports: [Week 11](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-11/week11_progress_report_solo_fix_pycaret_4066.md) | [Week 12](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-12/week12_progress_report_solo_fix_pycaret_4066.md) | [Week 13](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-13/week13_progress_report_solo_fix_pycaret_4066.md)  
Pull Request: [#4102](https://github.com/pycaret/pycaret/pull/4102)  
Documentation: [Solution to PyCaret Issue #4066](https://github.com/bennColl-cs4387/sizar/blob/main/assignments/solo-fixes/pycaret-4066/pycaret_4066.md)  

### 2. [Fixing Fold Number Calculation and Fold Validation in Time Series](https://github.com/pycaret/pycaret/issues/3011)  
Added a validation mechanism to PyCaret's `setup` function to ensure the `fold` parameter accepts only integers. Provided meaningful error messages to guide users when CV objects were passed incorrectly.  

Progress Report: [Week 14](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-14/week14_progress_report_solo_fix_pycaret_3011.md)  
Pull Request: [#4104](https://github.com/pycaret/pycaret/pull/4104)  
Documentation: [Solution to PyCaret Issue #3011 (Solo Fix)](https://github.com/bennColl-cs4387/sizar/blob/main/assignments/solo-fixes/pycaret-3011/pycaret_3011.md)


## Group Fix

For the group assignment, I worked with Arpon ([@abrararpon](https://github.com/abrararpon)) and Sinha ([@sinhabintebabul](https://github.com/sinhabintebabul)) on [PyCaret Issue #3011](https://github.com/pycaret/pycaret/issues/3011). Our task was to ensure that the fold number was displayed correctly in the setup summary when CV objects like `ExpandingWindowSplitter` were used. This involved debugging the `_set_fold_generator` function, testing various scenarios, and proposing changes to handle fold numbers accurately.  

From this group fix, I learned about the complexity of debugging large codebases and the importance of clear communication while working collaboratively. While the solution we proposed worked initially, my [solo fix](https://github.com/bennColl-cs4387/sizar/blob/main/assignments/solo-fixes/pycaret-3011/pycaret_3011.md) later refined this to align with PyCaret's documentation and ensure proper validation.

Progress Reports: [Build From Source](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-06/build_from_source.md) | [Week 9](https://github.com/bennColl-cs4387/sizar/blob/main/homework/week-09/group_fix_progress.md)  
Group Documentation: [Solution to PyCaret Issue #3011 (Group Fix)](https://github.com/bennColl-cs4387/sizar/blob/main/assignments/group-fix/pycaret-3011/pycaret_3011.md)


## Essay  

For my first solo fix, I wrote an essay detailing why I chose the issue and my proposed solution:  
&rarr; [Sizar - CS4387-Essay-Picking-First-Issue](https://github.com/bennColl-cs4387/sizar/blob/main/assignments/essay/essay_on_first_fix.md)

---

## Learnings

This course helped me better understand open-source development and how to contribute to large projects. By working on real-world issues in PyCaret, I gained a deeper understanding of how software is developed and maintained collaboratively.

### What I Learned
1. **Codebase Navigation**:  
   I learned how to navigate through large codebases like PyCaret, which required understanding interconnected modules and debugging complex issues without disrupting existing functionality.

2. **Error Validation**:  
   I implemented better error validation mechanisms, ensuring users receive clear feedback when they make mistakes. For example, ensuring the `fold` parameter accepts only integers and providing meaningful messages if it doesn't.

3. **Teamwork**:  
   Working on the group fix taught me how to divide tasks effectively and communicate clearly with teammates to solve problems collaboratively.

4. **Dependency Management**:  
   In my first solo fix, I moved plotting dependencies to an optional section. This taught me how to handle dependencies efficiently, making installations smaller and faster.

5. **Open-Source Contribution**:  
   I learned about GitHub workflows like creating pull requests, responding to feedback, and writing clean documentation.

### Challenges and Next Steps
- Debugging complex functionality was difficult, especially when dealing with edge cases. It pushed me to improve my problem-solving and Python skills.
- Merging changes and handling Git conflicts was challenging but helped me understand version control better.
- I will continue contributing to Machine Learning related projects. 
- I want to work on more system-level programming and explore contributing to Rust-based projects in the future.

As the term comes to the end, I want to express my heartfelt gratitude to Professor Michael Corey ([@mcorey](https://github.com/mcorey)) for his guidance and support throughout this course. This class has been an invaluable learning experience, allowing me to develop my skills, contribute to meaningful projects, and gain confidence in open-source collaboration. I am deeply thankful for the opportunity to learn, implement, and achieve under his mentorship.





