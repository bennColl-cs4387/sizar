# PyCaret Build From Source

I have followed the guidelines outlined in the [PyCaret Docs](https://pycaret.gitbook.io/docs/get-started/installation) to install PyCaret on my machine.

## Step 1: Forking the PyCaret Repository

I forked the PyCaret repository [here](https://github.com/mhsizar/pycaret).

## Step 2: Cloning the Forked Repository

After the repository was forked, I cloned it to my local machine: 
```bash
Class git clone https://github.com/mhsizar/pycaret.git
Cloning into 'pycaret'...
remote: Enumerating objects: 30102, done.
remote: Counting objects: 100% (468/468), done.
remote: Compressing objects: 100% (236/236), done.
remote: Total 30102 (delta 259), reused 411 (delta 227), pack-reused 29634 (from 1)
Receiving objects: 100% (30102/30102), 255.88 MiB | 78.83 MiB/s, done.
Resolving deltas: 100% (22162/22162), done.
➜  Class cd pycaret/       
```

## Step 3: Setting Up a Virtual Environment

To avoid conflicts with other packages, I set up a Python vitual environment:
```bash
➜  pycaret git:(build-from-source) python -m venv pycaret-env
➜  pycaret git:(build-from-source) ✗ source pycaret-env/bin/activate
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ 
```

## Step 4: Installing Dependencies
After activating the virtual environment, I installed the necessary dependencies:

```bash
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ pip install -r requirements.txt
```
<div style="max-height: 200px; overflow-y: auto; margin-bottom: 15px;"><pre><code>Ignoring setuptools: markers 'python_version >= "3.12"' don't match your environment
Collecting ipython>=5.5.0
  Using cached ipython-8.18.1-py3-none-any.whl (808 kB)
Collecting ipywidgets>=7.6.5
  Downloading ipywidgets-8.1.5-py3-none-any.whl (139 kB)
     |████████████████████████████████| 139 kB 3.8 MB/s 
Collecting tqdm>=4.62.0
  Downloading tqdm-4.66.5-py3-none-any.whl (78 kB)
     |████████████████████████████████| 78 kB 18.5 MB/s 
Collecting numpy<1.27,>=1.21
  Using cached numpy-1.26.4-cp39-cp39-macosx_11_0_arm64.whl (14.0 MB)
Collecting pandas>=2.2.0
  Downloading pandas-2.2.3-cp39-cp39-macosx_11_0_arm64.whl (11.3 MB)
     |████████████████████████████████| 11.3 MB 19.7 MB/s 
Collecting jinja2>=3
  Using cached jinja2-3.1.4-py3-none-any.whl (133 kB)
Collecting scipy<=1.11.4,>=1.6.1
  Downloading scipy-1.11.4-cp39-cp39-macosx_12_0_arm64.whl (29.7 MB)
     |████████████████████████████████| 29.7 MB 64.5 MB/s 
Collecting joblib<1.4,>=1.2.0
  Downloading joblib-1.3.2-py3-none-any.whl (302 kB)
     |████████████████████████████████| 302 kB 51.7 MB/s 
Collecting scikit-learn>1.4.0
  Downloading scikit_learn-1.5.2-cp39-cp39-macosx_12_0_arm64.whl (11.0 MB)
     |████████████████████████████████| 11.0 MB 60.0 MB/s 
Collecting pyod>=1.1.3
  Downloading pyod-2.0.2.tar.gz (165 kB)
     |████████████████████████████████| 165 kB 59.0 MB/s 
Collecting imbalanced-learn>=0.12.0
  Downloading imbalanced_learn-0.12.4-py3-none-any.whl (258 kB)
     |████████████████████████████████| 258 kB 65.0 MB/s 
Collecting category-encoders>=2.4.0
  Downloading category_encoders-2.6.4-py2.py3-none-any.whl (82 kB)
     |████████████████████████████████| 82 kB 1.0 MB/s 
Collecting lightgbm>=3.0.0
  Downloading lightgbm-4.5.0-py3-none-macosx_12_0_arm64.whl (1.6 MB)
     |████████████████████████████████| 1.6 MB 42.8 MB/s 
Collecting numba>=0.55.0
  Downloading numba-0.60.0-cp39-cp39-macosx_11_0_arm64.whl (2.7 MB)
     |████████████████████████████████| 2.7 MB 61.9 MB/s 
Collecting requests>=2.27.1
  Downloading requests-2.32.3-py3-none-any.whl (64 kB)
     |████████████████████████████████| 64 kB 25.9 MB/s 
Collecting psutil>=5.9.0
  Downloading psutil-6.0.0-cp38-abi3-macosx_11_0_arm64.whl (251 kB)
     |████████████████████████████████| 251 kB 66.6 MB/s 
Collecting markupsafe>=2.0.1
  Using cached MarkupSafe-2.1.5-cp39-cp39-macosx_10_9_universal2.whl (18 kB)
Collecting importlib_metadata>=4.12.0
  Downloading importlib_metadata-8.5.0-py3-none-any.whl (26 kB)
Collecting nbformat>=4.2.0
  Downloading nbformat-5.10.4-py3-none-any.whl (78 kB)
     |████████████████████████████████| 78 kB 36.3 MB/s 
Collecting cloudpickle
  Downloading cloudpickle-3.0.0-py3-none-any.whl (20 kB)
Collecting deprecation>=2.1.0
  Downloading deprecation-2.1.0-py2.py3-none-any.whl (11 kB)
Collecting xxhash
  Downloading xxhash-3.5.0-cp39-cp39-macosx_11_0_arm64.whl (30 kB)
Collecting wurlitzer
  Downloading wurlitzer-3.1.1-py3-none-any.whl (8.6 kB)
Collecting trio<0.25.0,>=0.22.0
  Downloading trio-0.24.0-py3-none-any.whl (460 kB)
     |████████████████████████████████| 460 kB 52.1 MB/s 
Collecting matplotlib<3.8.0
  Downloading matplotlib-3.7.5-cp39-cp39-macosx_11_0_arm64.whl (7.3 MB)
     |████████████████████████████████| 7.3 MB 56.3 MB/s 
Collecting mljar-scikit-plot
  Downloading mljar-scikit-plot-0.3.12.tar.gz (25 kB)
Collecting yellowbrick>=1.4
  Downloading yellowbrick-1.5-py3-none-any.whl (282 kB)
     |████████████████████████████████| 282 kB 60.2 MB/s 
Collecting plotly>=5.14.0
  Downloading plotly-5.24.1-py3-none-any.whl (19.1 MB)
     |████████████████████████████████| 19.1 MB 64.6 MB/s 
Collecting kaleido>=0.2.1
  Downloading kaleido-0.2.1-py2.py3-none-macosx_11_0_arm64.whl (85.8 MB)
     |████████████████████████████████| 85.8 MB 97.4 MB/s 
Collecting schemdraw==0.15
  Downloading schemdraw-0.15-py3-none-any.whl (106 kB)
     |████████████████████████████████| 106 kB 57.6 MB/s 
Collecting plotly-resampler>=0.8.3.1
  Downloading plotly_resampler-0.10.0-py3-none-any.whl (80 kB)
     |████████████████████████████████| 80 kB 33.2 MB/s 
Collecting statsmodels>=0.12.1
  Downloading statsmodels-0.14.4-cp39-cp39-macosx_11_0_arm64.whl (9.9 MB)
     |████████████████████████████████| 9.9 MB 60.2 MB/s 
Collecting sktime
  Downloading sktime-0.33.1-py3-none-any.whl (34.5 MB)
     |████████████████████████████████| 34.5 MB 63.9 MB/s 
Collecting tbats>=1.1.3
  Downloading tbats-1.1.3-py3-none-any.whl (44 kB)
     |████████████████████████████████| 44 kB 13.9 MB/s 
Collecting pmdarima>=2.0.4
  Downloading pmdarima-2.0.4-cp39-cp39-macosx_11_0_arm64.whl (630 kB)
     |████████████████████████████████| 630 kB 57.4 MB/s 
Collecting prompt-toolkit<3.1.0,>=3.0.41
  Downloading prompt_toolkit-3.0.48-py3-none-any.whl (386 kB)
     |████████████████████████████████| 386 kB 57.9 MB/s 
Collecting traitlets>=5
  Using cached traitlets-5.14.3-py3-none-any.whl (85 kB)
Collecting exceptiongroup
  Downloading exceptiongroup-1.2.2-py3-none-any.whl (16 kB)
Collecting matplotlib-inline
  Using cached matplotlib_inline-0.1.7-py3-none-any.whl (9.9 kB)
Collecting pygments>=2.4.0
  Using cached pygments-2.18.0-py3-none-any.whl (1.2 MB)
Collecting jedi>=0.16
  Using cached jedi-0.19.1-py2.py3-none-any.whl (1.6 MB)
Collecting decorator
  Using cached decorator-5.1.1-py3-none-any.whl (9.1 kB)
Collecting typing-extensions
  Downloading typing_extensions-4.12.2-py3-none-any.whl (37 kB)
Collecting stack-data
  Using cached stack_data-0.6.3-py3-none-any.whl (24 kB)
Collecting pexpect>4.3
  Using cached pexpect-4.9.0-py2.py3-none-any.whl (63 kB)
Collecting comm>=0.1.3
  Using cached comm-0.2.2-py3-none-any.whl (7.2 kB)
Collecting widgetsnbextension~=4.0.12
  Downloading widgetsnbextension-4.0.13-py3-none-any.whl (2.3 MB)
     |████████████████████████████████| 2.3 MB 43.2 MB/s 
Collecting jupyterlab-widgets~=3.0.12
  Downloading jupyterlab_widgets-3.0.13-py3-none-any.whl (214 kB)
     |████████████████████████████████| 214 kB 63.9 MB/s 
Collecting pytz>=2020.1
  Downloading pytz-2024.2-py2.py3-none-any.whl (508 kB)
     |████████████████████████████████| 508 kB 47.5 MB/s 
Collecting tzdata>=2022.7
  Downloading tzdata-2024.2-py2.py3-none-any.whl (346 kB)
     |████████████████████████████████| 346 kB 65.2 MB/s 
Collecting python-dateutil>=2.8.2
  Using cached python_dateutil-2.9.0.post0-py2.py3-none-any.whl (229 kB)
Collecting threadpoolctl>=3.1.0
  Using cached threadpoolctl-3.5.0-py3-none-any.whl (18 kB)
Collecting patsy>=0.5.1
  Downloading patsy-0.5.6-py2.py3-none-any.whl (233 kB)
     |████████████████████████████████| 233 kB 60.8 MB/s 
Collecting llvmlite<0.44,>=0.43.0dev0
  Downloading llvmlite-0.43.0-cp39-cp39-macosx_11_0_arm64.whl (28.8 MB)
     |████████████████████████████████| 28.8 MB 68.4 MB/s 
Collecting certifi>=2017.4.17
  Downloading certifi-2024.8.30-py3-none-any.whl (167 kB)
     |████████████████████████████████| 167 kB 77.6 MB/s 
Collecting urllib3<3,>=1.21.1
  Downloading urllib3-2.2.3-py3-none-any.whl (126 kB)
     |████████████████████████████████| 126 kB 67.8 MB/s 
Collecting charset-normalizer<4,>=2
  Using cached charset_normalizer-3.3.2-cp39-cp39-macosx_11_0_arm64.whl (120 kB)
Collecting idna<4,>=2.5
  Downloading idna-3.10-py3-none-any.whl (70 kB)
     |████████████████████████████████| 70 kB 48.9 MB/s 
Collecting zipp>=3.20
  Downloading zipp-3.20.2-py3-none-any.whl (9.2 kB)
Collecting jupyter-core!=5.0.*,>=4.12
  Using cached jupyter_core-5.7.2-py3-none-any.whl (28 kB)
Collecting fastjsonschema>=2.15
  Downloading fastjsonschema-2.20.0-py3-none-any.whl (23 kB)
Collecting jsonschema>=2.6
  Downloading jsonschema-4.23.0-py3-none-any.whl (88 kB)
     |████████████████████████████████| 88 kB 28.5 MB/s 
Collecting packaging
  Downloading packaging-24.1-py3-none-any.whl (53 kB)
     |████████████████████████████████| 53 kB 17.8 MB/s 
Collecting outcome
  Downloading outcome-1.3.0.post0-py2.py3-none-any.whl (10 kB)
Collecting sniffio>=1.3.0
  Downloading sniffio-1.3.1-py3-none-any.whl (10 kB)
Collecting sortedcontainers
  Downloading sortedcontainers-2.4.0-py2.py3-none-any.whl (29 kB)
Collecting attrs>=20.1.0
  Downloading attrs-24.2.0-py3-none-any.whl (63 kB)
     |████████████████████████████████| 63 kB 11.3 MB/s 
Collecting cycler>=0.10
  Using cached cycler-0.12.1-py3-none-any.whl (8.3 kB)
Collecting pyparsing>=2.3.1
  Downloading pyparsing-3.1.4-py3-none-any.whl (104 kB)
     |████████████████████████████████| 104 kB 67.9 MB/s 
Collecting fonttools>=4.22.0
  Downloading fonttools-4.54.1-cp39-cp39-macosx_11_0_arm64.whl (2.3 MB)
     |████████████████████████████████| 2.3 MB 70.9 MB/s 
Collecting pillow>=6.2.0
  Downloading pillow-10.4.0-cp39-cp39-macosx_11_0_arm64.whl (3.4 MB)
     |████████████████████████████████| 3.4 MB 56.3 MB/s 
Collecting kiwisolver>=1.0.1
  Downloading kiwisolver-1.4.7-cp39-cp39-macosx_11_0_arm64.whl (64 kB)
     |████████████████████████████████| 64 kB 17.4 MB/s 
Collecting contourpy>=1.0.1
  Downloading contourpy-1.3.0-cp39-cp39-macosx_11_0_arm64.whl (249 kB)
     |████████████████████████████████| 249 kB 73.0 MB/s 
Collecting importlib-resources>=3.2.0
  Downloading importlib_resources-6.4.5-py3-none-any.whl (36 kB)
Collecting tenacity>=6.2.0
  Downloading tenacity-9.0.0-py3-none-any.whl (28 kB)
Collecting orjson<4.0.0,>=3.8.0
  Downloading orjson-3.10.7-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl (251 kB)
     |████████████████████████████████| 251 kB 59.2 MB/s 
Collecting dash>=2.9.0
  Downloading dash-2.18.1-py3-none-any.whl (7.5 MB)
     |████████████████████████████████| 7.5 MB 64.3 MB/s 
Collecting tsdownsample>=0.1.3
  Downloading tsdownsample-0.1.3-cp39-cp39-macosx_11_0_arm64.whl (1.1 MB)
     |████████████████████████████████| 1.1 MB 66.9 MB/s 
Collecting scikit-base<0.9.0,>=0.6.1
  Downloading scikit_base-0.8.3-py3-none-any.whl (136 kB)
     |████████████████████████████████| 136 kB 59.1 MB/s 
Collecting Cython!=0.29.18,!=0.29.31,>=0.29
  Downloading Cython-3.0.11-py2.py3-none-any.whl (1.2 MB)
     |████████████████████████████████| 1.2 MB 64.0 MB/s 
Requirement already satisfied: setuptools!=50.0.0,>=38.6.0 in ./pycaret-env/lib/python3.9/site-packages (from pmdarima>=2.0.4->-r requirements.txt (line 43)) (58.0.4)
Collecting dash-table==5.0.0
  Using cached dash_table-5.0.0-py3-none-any.whl (3.9 kB)
Collecting dash-html-components==2.0.0
  Using cached dash_html_components-2.0.0-py3-none-any.whl (4.1 kB)
Collecting nest-asyncio
  Using cached nest_asyncio-1.6.0-py3-none-any.whl (5.2 kB)
Collecting dash-core-components==2.0.0
  Using cached dash_core_components-2.0.0-py3-none-any.whl (3.8 kB)
Collecting retrying
  Using cached retrying-1.3.4-py3-none-any.whl (11 kB)
Collecting Flask<3.1,>=1.0.4
  Using cached flask-3.0.3-py3-none-any.whl (101 kB)
Collecting Werkzeug<3.1
  Downloading werkzeug-3.0.4-py3-none-any.whl (227 kB)
     |████████████████████████████████| 227 kB 55.6 MB/s 
Collecting blinker>=1.6.2
  Using cached blinker-1.8.2-py3-none-any.whl (9.5 kB)
Collecting itsdangerous>=2.1.2
  Using cached itsdangerous-2.2.0-py3-none-any.whl (16 kB)
Collecting click>=8.1.3
  Using cached click-8.1.7-py3-none-any.whl (97 kB)
Collecting parso<0.9.0,>=0.8.3
  Using cached parso-0.8.4-py2.py3-none-any.whl (103 kB)
Collecting referencing>=0.28.4
  Using cached referencing-0.35.1-py3-none-any.whl (26 kB)
Collecting rpds-py>=0.7.1
  Downloading rpds_py-0.20.0-cp39-cp39-macosx_11_0_arm64.whl (311 kB)
     |████████████████████████████████| 311 kB 58.0 MB/s 
Collecting jsonschema-specifications>=2023.03.6
  Using cached jsonschema_specifications-2023.12.1-py3-none-any.whl (18 kB)
Collecting platformdirs>=2.5
  Downloading platformdirs-4.3.6-py3-none-any.whl (18 kB)
Collecting six
  Using cached six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting ptyprocess>=0.5
  Using cached ptyprocess-0.7.0-py2.py3-none-any.whl (13 kB)
Collecting wcwidth
  Using cached wcwidth-0.2.13-py2.py3-none-any.whl (34 kB)
Collecting pure-eval
  Downloading pure_eval-0.2.3-py3-none-any.whl (11 kB)
Collecting asttokens>=2.1.0
  Using cached asttokens-2.4.1-py2.py3-none-any.whl (27 kB)
Collecting executing>=1.2.0
  Downloading executing-2.1.0-py2.py3-none-any.whl (25 kB)
Using legacy 'setup.py install' for pyod, since package 'wheel' is not installed.
Using legacy 'setup.py install' for mljar-scikit-plot, since package 'wheel' is not installed.
Installing collected packages: six, zipp, tzdata, rpds-py, pytz, python-dateutil, numpy, markupsafe, attrs, Werkzeug, wcwidth, urllib3, traitlets, threadpoolctl, tenacity, scipy, referencing, pure-eval, ptyprocess, patsy, parso, pandas, packaging, joblib, jinja2, itsdangerous, importlib-metadata, idna, executing, click, charset-normalizer, certifi, blinker, asttokens, typing-extensions, statsmodels, stack-data, scikit-learn, retrying, requests, pyparsing, pygments, prompt-toolkit, plotly, platformdirs, pillow, pexpect, nest-asyncio, matplotlib-inline, llvmlite, kiwisolver, jsonschema-specifications, jedi, importlib-resources, fonttools, Flask, exceptiongroup, decorator, dash-table, dash-html-components, dash-core-components, Cython, cycler, contourpy, widgetsnbextension, tsdownsample, sortedcontainers, sniffio, scikit-base, pmdarima, outcome, orjson, numba, matplotlib, jupyterlab-widgets, jupyter-core, jsonschema, ipython, fastjsonschema, dash, comm, yellowbrick, xxhash, wurlitzer, trio, tqdm, tbats, sktime, schemdraw, pyod, psutil, plotly-resampler, nbformat, mljar-scikit-plot, lightgbm, kaleido, ipywidgets, imbalanced-learn, deprecation, cloudpickle, category-encoders
    Running setup.py install for pyod ... done
    Running setup.py install for mljar-scikit-plot ... done
Successfully installed Cython-3.0.11 Flask-3.0.3 Werkzeug-3.0.4 asttokens-2.4.1 attrs-24.2.0 blinker-1.8.2 category-encoders-2.6.4 certifi-2024.8.30 charset-normalizer-3.3.2 click-8.1.7 cloudpickle-3.0.0 comm-0.2.2 contourpy-1.3.0 cycler-0.12.1 dash-2.18.1 dash-core-components-2.0.0 dash-html-components-2.0.0 dash-table-5.0.0 decorator-5.1.1 deprecation-2.1.0 exceptiongroup-1.2.2 executing-2.1.0 fastjsonschema-2.20.0 fonttools-4.54.1 idna-3.10 imbalanced-learn-0.12.4 importlib-metadata-8.5.0 importlib-resources-6.4.5 ipython-8.18.1 ipywidgets-8.1.5 itsdangerous-2.2.0 jedi-0.19.1 jinja2-3.1.4 joblib-1.3.2 jsonschema-4.23.0 jsonschema-specifications-2023.12.1 jupyter-core-5.7.2 jupyterlab-widgets-3.0.13 kaleido-0.2.1 kiwisolver-1.4.7 lightgbm-4.5.0 llvmlite-0.43.0 markupsafe-2.1.5 matplotlib-3.7.5 matplotlib-inline-0.1.7 mljar-scikit-plot-0.3.12 nbformat-5.10.4 nest-asyncio-1.6.0 numba-0.60.0 numpy-1.26.4 orjson-3.10.7 outcome-1.3.0.post0 packaging-24.1 pandas-2.2.3 parso-0.8.4 patsy-0.5.6 pexpect-4.9.0 pillow-10.4.0 platformdirs-4.3.6 plotly-5.24.1 plotly-resampler-0.10.0 pmdarima-2.0.4 prompt-toolkit-3.0.48 psutil-6.0.0 ptyprocess-0.7.0 pure-eval-0.2.3 pygments-2.18.0 pyod-2.0.2 pyparsing-3.1.4 python-dateutil-2.9.0.post0 pytz-2024.2 referencing-0.35.1 requests-2.32.3 retrying-1.3.4 rpds-py-0.20.0 schemdraw-0.15 scikit-base-0.8.3 scikit-learn-1.5.2 scipy-1.11.4 six-1.16.0 sktime-0.33.1 sniffio-1.3.1 sortedcontainers-2.4.0 stack-data-0.6.3 statsmodels-0.14.4 tbats-1.1.3 tenacity-9.0.0 threadpoolctl-3.5.0 tqdm-4.66.5 traitlets-5.14.3 trio-0.24.0 tsdownsample-0.1.3 typing-extensions-4.12.2 tzdata-2024.2 urllib3-2.2.3 wcwidth-0.2.13 widgetsnbextension-4.0.13 wurlitzer-3.1.1 xxhash-3.5.0 yellowbrick-1.5 zipp-3.20.2</code></pre></div>


```bash
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ pip install -r requirements-dev.txt
```

<div style="max-height: 200px; overflow-y: auto; margin-bottom: 15px;"><pre><code>Collecting black>=24.8.0 (from -r requirements-dev.txt (line 1))
  Downloading black-24.8.0-cp39-cp39-macosx_11_0_arm64.whl.metadata (78 kB)
Collecting isort>=5.13.2 (from -r requirements-dev.txt (line 2))
  Downloading isort-5.13.2-py3-none-any.whl.metadata (12 kB)
Collecting flake8>=7.1.1 (from -r requirements-dev.txt (line 3))
  Downloading flake8-7.1.1-py2.py3-none-any.whl.metadata (3.8 kB)
Collecting setuptools>=71.1.0 (from -r requirements-dev.txt (line 4))
  Downloading setuptools-75.1.0-py3-none-any.whl.metadata (6.9 kB)
Collecting mypy>=0.11.1 (from -r requirements-dev.txt (line 5))
  Downloading mypy-1.11.2-cp39-cp39-macosx_11_0_arm64.whl.metadata (1.9 kB)
Requirement already satisfied: click>=8.0.0 in ./pycaret-env/lib/python3.9/site-packages (from black>=24.8.0->-r requirements-dev.txt (line 1)) (8.1.7)
Collecting mypy-extensions>=0.4.3 (from black>=24.8.0->-r requirements-dev.txt (line 1))
  Downloading mypy_extensions-1.0.0-py3-none-any.whl.metadata (1.1 kB)
Requirement already satisfied: packaging>=22.0 in ./pycaret-env/lib/python3.9/site-packages (from black>=24.8.0->-r requirements-dev.txt (line 1)) (24.1)
Collecting pathspec>=0.9.0 (from black>=24.8.0->-r requirements-dev.txt (line 1))
  Downloading pathspec-0.12.1-py3-none-any.whl.metadata (21 kB)
Requirement already satisfied: platformdirs>=2 in ./pycaret-env/lib/python3.9/site-packages (from black>=24.8.0->-r requirements-dev.txt (line 1)) (4.3.6)
Collecting tomli>=1.1.0 (from black>=24.8.0->-r requirements-dev.txt (line 1))
  Downloading tomli-2.0.2-py3-none-any.whl.metadata (10.0 kB)
Requirement already satisfied: typing-extensions>=4.0.1 in ./pycaret-env/lib/python3.9/site-packages (from black>=24.8.0->-r requirements-dev.txt (line 1)) (4.12.2)
Collecting mccabe<0.8.0,>=0.7.0 (from flake8>=7.1.1->-r requirements-dev.txt (line 3))
  Downloading mccabe-0.7.0-py2.py3-none-any.whl.metadata (5.0 kB)
Collecting pycodestyle<2.13.0,>=2.12.0 (from flake8>=7.1.1->-r requirements-dev.txt (line 3))
  Downloading pycodestyle-2.12.1-py2.py3-none-any.whl.metadata (4.5 kB)
Collecting pyflakes<3.3.0,>=3.2.0 (from flake8>=7.1.1->-r requirements-dev.txt (line 3))
  Downloading pyflakes-3.2.0-py2.py3-none-any.whl.metadata (3.5 kB)
Downloading black-24.8.0-cp39-cp39-macosx_11_0_arm64.whl (1.5 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.5/1.5 MB 21.9 MB/s eta 0:00:00
Downloading isort-5.13.2-py3-none-any.whl (92 kB)
Downloading flake8-7.1.1-py2.py3-none-any.whl (57 kB)
Downloading setuptools-75.1.0-py3-none-any.whl (1.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 55.2 MB/s eta 0:00:00
Downloading mypy-1.11.2-cp39-cp39-macosx_11_0_arm64.whl (10.1 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 10.1/10.1 MB 92.8 MB/s eta 0:00:00
Downloading mccabe-0.7.0-py2.py3-none-any.whl (7.3 kB)
Downloading mypy_extensions-1.0.0-py3-none-any.whl (4.7 kB)
Downloading pathspec-0.12.1-py3-none-any.whl (31 kB)
Downloading pycodestyle-2.12.1-py2.py3-none-any.whl (31 kB)
Downloading pyflakes-3.2.0-py2.py3-none-any.whl (62 kB)
Downloading tomli-2.0.2-py3-none-any.whl (13 kB)
Installing collected packages: tomli, setuptools, pyflakes, pycodestyle, pathspec, mypy-extensions, mccabe, isort, mypy, flake8, black
  Attempting uninstall: setuptools
    Found existing installation: setuptools 58.0.4
    Uninstalling setuptools-58.0.4:
      Successfully uninstalled setuptools-58.0.4
Successfully installed black-24.8.0 flake8-7.1.1 isort-5.13.2 mccabe-0.7.0 mypy-1.11.2 mypy-extensions-1.0.0 pathspec-0.12.1 pycodestyle-2.12.1 pyflakes-3.2.0 setuptools-75.1.0 tomli-2.0.2</code></pre></div>

```bash
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ pip install -r requirements-test.txt
```

<div style="max-height: 200px; overflow-y: auto; margin-bottom: 15px;"><pre><code></code></pre></div>
