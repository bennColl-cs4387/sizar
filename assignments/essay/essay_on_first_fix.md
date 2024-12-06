I have written an essay on my pick for the first fix and solution proposal here:   
&rarr; [Sizar - CS4387-Essay-Picking-First-Issue](https://docs.google.com/document/d/1y63Nj9xfDUoSn9NVLLc2NCfYrLQRbkg7Me7EKZ3WW9I)


### Contributing to PyCaret
#### Mehedi Hasan Sizar

For my first open-source contribution, I have chosen PyCaret, a low-code machine-learning library in Python. PyCaret simplifies machine learning workflows utilizing libraries and frameworks, including scikit-learn, XGNBoost, CatBoost, and Hyperopt. This makes it a valuable tool for both experienced data scientists and those who may not have a strong background in coding. PyCaret allows easy and quick experimentation, reducing the need to write extensive code. (`PyCaret Docs`)

PyCaret is built using Python, which makes it an ideal project for me, as I am already familiar with Python, especially the libraries and frameworks related to data science. It is a deployment-ready library that serves as a wrapper around various machine-learning tools that can be run using simple commands. Contributing to this open-source project would be easier, as I would not need to learn additional languages or frameworks. (`PyCaret deployment capabilities`)

The main contributors to PyCaret include Moez Ali, the creator, along with a diverse community of developers. This project is solely open source and does not seem to be driven by any corporate agenda, making it a community-led project that values contributions from independent developers. It’s an ongoing project with thorough documentation and has the code of conduct outlined in the Github repository.  The project offers detailed API references, tutorials, use-case examples, and feature demonstrations, which make it easy to navigate and understand (`PyCaret Docs`). This aspect is particularly attractive to me because it means I am welcomed as a new contributor, have enough resources available to learn and contribute, and will receive feedback and guidance from experienced developers.

PyCaret is a perfect match for my background in data science using Python libraries like scikit-learn and matplotlib. Its low-code nature allows me to focus on improving its functionality rather than having to spend time understanding complex algorithms. The project being solely open source, its openness to new independent contributors, and its active community make it an ideal environment for my learning and contribution opportunities. I like how PyCaret aims to make machine learning more accessible, and would love to continue contributing to the initiative regularly. 

There are currently more than 350 open issues, which I can contribute to fixing. There are a number of interesting features and identified bugs that need to be worked on. However, to begin with, I have found an enhancement request related to the inclusion of optional plotting dependencies to enhance the installation size and time. Currently, PyCaret requires users to install large plotting libraries such as Plotly and Kaleido, irrespective of the user’s intention to use or not use visualization features from those libraries. This increases the size of the installation unnecessarily, especially for users who are only interested in running machine-learning models without generating visual plots (`PyCaret GitHub Issue #4066`). 

The `[ENH]: Make plotting dependencies optional #4066` issue is not dependent on other issues, and should be straightforward to resolve, as it may involve moving dependencies from the requirements.txt file to the requirements-optional.txt file and some modifications on the setup.py file. Although nobody has commented on the issue yet, it seems a reasonable adjustment to me which can enhance the installation process and storage usage. The author has filled out the template with detailed information about the issue and also proposed possible solutions. It’s been a while since the issue was raised, but it has not been addressed yet, making it a good first issue for me to tackle as a beginner. 

#### To address the issue, I propose the following solution:
1. **Move Plotting Dependencies to `requirements-optional.txt`:**   
The plotting-related dependencies currently in the requirements.txt file need to be moved to the requirements-optional.txt file. This would include libraries such as Plotly, Kaleido, Yellowbrick, and others related to visualization. With this, users who do not require plotting functionalities can avoid installing these large libraries, resulting in a smaller installation time and size.
2. **Modify setup.py to Reflect Optional Dependencies:**  
The setup.py file needs to be updated to include an extras_require section for plotting dependencies. This will allow users to install plotting-related libraries using a simple flag during installation (i.e. PyCaret with plotting dependencies can be installed by running `pip install pycaret[plots]`). 
3. **Adjust PyCaret’s Code to Handle Missing Dependencies:**  
The files in PyCaret that use plotting libraries need to be adjusted to handle cases where these libraries are not installed. This can be done by using try-except blocks, ensuring that users are informed if the required plotting libraries are missing, and providing instructions on how to install them. 

I am confident that I am well-suited to address this issue because of my familiarity with Python and package management. I have experience working with visualization tools like Plotly and Matplotlib, which gives me the necessary background to understand how to work with plotting-related dependencies. Working on this issue will provide me with a great opportunity to learn more about open-source contributions and dependency management, both of which are essential skills in software development. By solving this issue, I can contribute to making PyCaret more lightweight and user-friendly, benefiting the wider community of data scientists who use low-code libraries for machine learning. 


#### Work Cited
1. “PyCaret Docs.” PyCaret 3.0 | Docs, 19 March 2023, https://pycaret.gitbook.io/docs. Accessed 19 October 2024.
2. “PyCaret deployment capabilities.” PyCaret 3.0 | Docs, 19 March 2023, https://pycaret.gitbook.io/docs#pycaret-deployment-capabilities. Accessed 19 October 2024.
3. “PyCaret Code of Conduct.” PyCaret Github, https://github.com/pycaret/pycaret/blob/master/CODE_OF_CONDUCT.md. Accessed 19 October 2024.
4. “PyCaret GitHub Issue #4066.” PyCaret Github, 3 September 2024, https://github.com/pycaret/pycaret/issues/4066. Accessed 19 October 2024.

