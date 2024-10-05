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

<div style="max-height: 200px; overflow-y: auto; margin-bottom: 15px;"><pre><code>Collecting pytest==8.3.2 (from -r requirements-test.txt (line 1))
  Downloading pytest-8.3.2-py3-none-any.whl.metadata (7.5 kB)
Collecting moto<5.0.0 (from -r requirements-test.txt (line 2))
  Downloading moto-4.2.14-py2.py3-none-any.whl.metadata (12 kB)
Collecting fugue[dask] (from -r requirements-test.txt (line 4))
  Downloading fugue-0.9.1-py3-none-any.whl.metadata (18 kB)
Requirement already satisfied: dash[testing] in ./pycaret-env/lib/python3.9/site-packages (from -r requirements-test.txt (line 5)) (2.18.1)
Collecting iniconfig (from pytest==8.3.2->-r requirements-test.txt (line 1))
  Downloading iniconfig-2.0.0-py3-none-any.whl.metadata (2.6 kB)
Requirement already satisfied: packaging in ./pycaret-env/lib/python3.9/site-packages (from pytest==8.3.2->-r requirements-test.txt (line 1)) (24.1)
Collecting pluggy<2,>=1.5 (from pytest==8.3.2->-r requirements-test.txt (line 1))
  Downloading pluggy-1.5.0-py3-none-any.whl.metadata (4.8 kB)
Requirement already satisfied: exceptiongroup>=1.0.0rc8 in ./pycaret-env/lib/python3.9/site-packages (from pytest==8.3.2->-r requirements-test.txt (line 1)) (1.2.2)
Requirement already satisfied: tomli>=1 in ./pycaret-env/lib/python3.9/site-packages (from pytest==8.3.2->-r requirements-test.txt (line 1)) (2.0.2)
Collecting boto3>=1.9.201 (from moto<5.0.0->-r requirements-test.txt (line 2))
  Using cached boto3-1.35.34-py3-none-any.whl.metadata (6.6 kB)
Collecting botocore>=1.12.201 (from moto<5.0.0->-r requirements-test.txt (line 2))
  Using cached botocore-1.35.34-py3-none-any.whl.metadata (5.6 kB)
Collecting cryptography>=3.3.1 (from moto<5.0.0->-r requirements-test.txt (line 2))
  Downloading cryptography-43.0.1-cp39-abi3-macosx_10_9_universal2.whl.metadata (5.4 kB)
Requirement already satisfied: requests>=2.5 in ./pycaret-env/lib/python3.9/site-packages (from moto<5.0.0->-r requirements-test.txt (line 2)) (2.32.3)
Collecting xmltodict (from moto<5.0.0->-r requirements-test.txt (line 2))
  Downloading xmltodict-0.13.0-py2.py3-none-any.whl.metadata (7.7 kB)
Requirement already satisfied: werkzeug!=2.2.0,!=2.2.1,>=0.5 in ./pycaret-env/lib/python3.9/site-packages (from moto<5.0.0->-r requirements-test.txt (line 2)) (3.0.4)
Requirement already satisfied: python-dateutil<3.0.0,>=2.1 in ./pycaret-env/lib/python3.9/site-packages (from moto<5.0.0->-r requirements-test.txt (line 2)) (2.9.0.post0)
Collecting responses>=0.13.0 (from moto<5.0.0->-r requirements-test.txt (line 2))
  Downloading responses-0.25.3-py3-none-any.whl.metadata (46 kB)
Requirement already satisfied: Jinja2>=2.10.1 in ./pycaret-env/lib/python3.9/site-packages (from moto<5.0.0->-r requirements-test.txt (line 2)) (3.1.4)
Collecting triad>=0.9.7 (from fugue[dask]->-r requirements-test.txt (line 4))
  Using cached triad-0.9.8-py3-none-any.whl.metadata (6.3 kB)
Collecting adagio>=0.2.4 (from fugue[dask]->-r requirements-test.txt (line 4))
  Using cached adagio-0.2.6-py3-none-any.whl.metadata (1.8 kB)
Collecting dask>=2023.5.0 (from dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached dask-2024.8.0-py3-none-any.whl.metadata (3.8 kB)
Collecting pyarrow>=7.0.0 (from fugue[dask]->-r requirements-test.txt (line 4))
  Using cached pyarrow-17.0.0-cp39-cp39-macosx_11_0_arm64.whl.metadata (3.3 kB)
Requirement already satisfied: pandas>=2.0.2 in ./pycaret-env/lib/python3.9/site-packages (from fugue[dask]->-r requirements-test.txt (line 4)) (2.2.3)
Requirement already satisfied: Flask<3.1,>=1.0.4 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (3.0.3)
Requirement already satisfied: plotly>=5.0.0 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (5.24.1)
Requirement already satisfied: dash-html-components==2.0.0 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (2.0.0)
Requirement already satisfied: dash-core-components==2.0.0 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (2.0.0)
Requirement already satisfied: dash-table==5.0.0 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (5.0.0)
Requirement already satisfied: importlib-metadata in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (8.5.0)
Requirement already satisfied: typing-extensions>=4.1.1 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (4.12.2)
Requirement already satisfied: retrying in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (1.3.4)
Requirement already satisfied: nest-asyncio in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (1.6.0)
Requirement already satisfied: setuptools in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (75.1.0)
Collecting beautifulsoup4>=4.8.2 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading beautifulsoup4-4.12.3-py3-none-any.whl.metadata (3.8 kB)
Collecting lxml>=4.6.2 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading lxml-5.3.0-cp39-cp39-macosx_10_9_universal2.whl.metadata (3.8 kB)
Collecting percy>=2.0.2 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading percy-2.0.2-py2.py3-none-any.whl.metadata (821 bytes)
Collecting selenium<=4.2.0,>=3.141.0 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading selenium-4.2.0-py3-none-any.whl.metadata (6.5 kB)
Collecting waitress>=1.4.4 (from dash[testing]->-r requirements-test.txt (line 5))
  Using cached waitress-3.0.0-py3-none-any.whl.metadata (4.2 kB)
Collecting multiprocess>=0.70.12 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading multiprocess-0.70.17-py39-none-any.whl.metadata (7.2 kB)
Requirement already satisfied: psutil>=5.8.0 in ./pycaret-env/lib/python3.9/site-packages (from dash[testing]->-r requirements-test.txt (line 5)) (6.0.0)
Collecting dash-testing-stub>=0.0.2 (from dash[testing]->-r requirements-test.txt (line 5))
  Downloading dash_testing_stub-0.0.2-py3-none-any.whl.metadata (587 bytes)
Collecting soupsieve>1.2 (from beautifulsoup4>=4.8.2->dash[testing]->-r requirements-test.txt (line 5))
  Downloading soupsieve-2.6-py3-none-any.whl.metadata (4.6 kB)
Collecting jmespath<2.0.0,>=0.7.1 (from boto3>=1.9.201->moto<5.0.0->-r requirements-test.txt (line 2))
  Using cached jmespath-1.0.1-py3-none-any.whl.metadata (7.6 kB)
Collecting s3transfer<0.11.0,>=0.10.0 (from boto3>=1.9.201->moto<5.0.0->-r requirements-test.txt (line 2))
  Using cached s3transfer-0.10.2-py3-none-any.whl.metadata (1.7 kB)
Collecting urllib3<1.27,>=1.25.4 (from botocore>=1.12.201->moto<5.0.0->-r requirements-test.txt (line 2))
  Downloading urllib3-1.26.20-py2.py3-none-any.whl.metadata (50 kB)
Collecting cffi>=1.12 (from cryptography>=3.3.1->moto<5.0.0->-r requirements-test.txt (line 2))
  Downloading cffi-1.17.1-cp39-cp39-macosx_11_0_arm64.whl.metadata (1.5 kB)
Requirement already satisfied: click>=8.1 in ./pycaret-env/lib/python3.9/site-packages (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4)) (8.1.7)
Requirement already satisfied: cloudpickle>=1.5.0 in ./pycaret-env/lib/python3.9/site-packages (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4)) (3.0.0)
Collecting fsspec>=2021.09.0 (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached fsspec-2024.9.0-py3-none-any.whl.metadata (11 kB)
Collecting partd>=1.4.0 (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached partd-1.4.2-py3-none-any.whl.metadata (4.6 kB)
Collecting pyyaml>=5.3.1 (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached PyYAML-6.0.2-cp39-cp39-macosx_11_0_arm64.whl.metadata (2.1 kB)
Collecting toolz>=0.10.0 (from dask>=2023.5.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached toolz-1.0.0-py3-none-any.whl.metadata (5.1 kB)
Collecting distributed==2024.8.0 (from dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached distributed-2024.8.0-py3-none-any.whl.metadata (3.4 kB)
Collecting dask-expr<1.2,>=1.1 (from dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Downloading dask_expr-1.1.10-py3-none-any.whl.metadata (2.5 kB)
Collecting locket>=1.0.0 (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached locket-1.0.0-py2.py3-none-any.whl.metadata (2.8 kB)
Collecting msgpack>=1.0.0 (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached msgpack-1.1.0-cp39-cp39-macosx_11_0_arm64.whl.metadata (8.4 kB)
Requirement already satisfied: sortedcontainers>=2.0.5 in ./pycaret-env/lib/python3.9/site-packages (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4)) (2.4.0)
Collecting tblib>=1.6.0 (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached tblib-3.0.0-py3-none-any.whl.metadata (25 kB)
Collecting tornado>=6.0.4 (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached tornado-6.4.1-cp38-abi3-macosx_10_9_universal2.whl.metadata (2.5 kB)
Collecting zict>=3.0.0 (from distributed==2024.8.0->dask[dataframe,distributed]>=2023.5.0; extra == "dask"->fugue[dask]->-r requirements-test.txt (line 4))
  Using cached zict-3.0.0-py2.py3-none-any.whl.metadata (899 bytes)
Requirement already satisfied: itsdangerous>=2.1.2 in ./pycaret-env/lib/python3.9/site-packages (from Flask<3.1,>=1.0.4->dash[testing]->-r requirements-test.txt (line 5)) (2.2.0)
Requirement already satisfied: blinker>=1.6.2 in ./pycaret-env/lib/python3.9/site-packages (from Flask<3.1,>=1.0.4->dash[testing]->-r requirements-test.txt (line 5)) (1.8.2)
Requirement already satisfied: zipp>=3.20 in ./pycaret-env/lib/python3.9/site-packages (from importlib-metadata->dash[testing]->-r requirements-test.txt (line 5)) (3.20.2)
Requirement already satisfied: MarkupSafe>=2.0 in ./pycaret-env/lib/python3.9/site-packages (from Jinja2>=2.10.1->moto<5.0.0->-r requirements-test.txt (line 2)) (2.1.5)
Collecting dill>=0.3.9 (from multiprocess>=0.70.12->dash[testing]->-r requirements-test.txt (line 5))
  Using cached dill-0.3.9-py3-none-any.whl.metadata (10 kB)
Requirement already satisfied: numpy>=1.22.4 in ./pycaret-env/lib/python3.9/site-packages (from pandas>=2.0.2->fugue[dask]->-r requirements-test.txt (line 4)) (1.26.4)
Requirement already satisfied: pytz>=2020.1 in ./pycaret-env/lib/python3.9/site-packages (from pandas>=2.0.2->fugue[dask]->-r requirements-test.txt (line 4)) (2024.2)
Requirement already satisfied: tzdata>=2022.7 in ./pycaret-env/lib/python3.9/site-packages (from pandas>=2.0.2->fugue[dask]->-r requirements-test.txt (line 4)) (2024.2)
Requirement already satisfied: tenacity>=6.2.0 in ./pycaret-env/lib/python3.9/site-packages (from plotly>=5.0.0->dash[testing]->-r requirements-test.txt (line 5)) (9.0.0)
Requirement already satisfied: six>=1.5 in ./pycaret-env/lib/python3.9/site-packages (from python-dateutil<3.0.0,>=2.1->moto<5.0.0->-r requirements-test.txt (line 2)) (1.16.0)
Requirement already satisfied: charset-normalizer<4,>=2 in ./pycaret-env/lib/python3.9/site-packages (from requests>=2.5->moto<5.0.0->-r requirements-test.txt (line 2)) (3.3.2)
Requirement already satisfied: idna<4,>=2.5 in ./pycaret-env/lib/python3.9/site-packages (from requests>=2.5->moto<5.0.0->-r requirements-test.txt (line 2)) (3.10)
Requirement already satisfied: certifi>=2017.4.17 in ./pycaret-env/lib/python3.9/site-packages (from requests>=2.5->moto<5.0.0->-r requirements-test.txt (line 2)) (2024.8.30)
Requirement already satisfied: trio~=0.17 in ./pycaret-env/lib/python3.9/site-packages (from selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5)) (0.24.0)
Collecting trio-websocket~=0.9 (from selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Downloading trio_websocket-0.11.1-py3-none-any.whl.metadata (4.7 kB)
Collecting fs (from triad>=0.9.7->fugue[dask]->-r requirements-test.txt (line 4))
  Downloading fs-2.4.16-py2.py3-none-any.whl.metadata (6.3 kB)
Collecting pycparser (from cffi>=1.12->cryptography>=3.3.1->moto<5.0.0->-r requirements-test.txt (line 2))
  Using cached pycparser-2.22-py3-none-any.whl.metadata (943 bytes)
Requirement already satisfied: attrs>=20.1.0 in ./pycaret-env/lib/python3.9/site-packages (from trio~=0.17->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5)) (24.2.0)
Requirement already satisfied: outcome in ./pycaret-env/lib/python3.9/site-packages (from trio~=0.17->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5)) (1.3.0.post0)
Requirement already satisfied: sniffio>=1.3.0 in ./pycaret-env/lib/python3.9/site-packages (from trio~=0.17->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5)) (1.3.1)
Collecting wsproto>=0.14 (from trio-websocket~=0.9->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Downloading wsproto-1.2.0-py3-none-any.whl.metadata (5.6 kB)
Collecting PySocks!=1.5.7,<2.0,>=1.5.6 (from urllib3[secure,socks]~=1.26->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Downloading PySocks-1.7.1-py3-none-any.whl.metadata (13 kB)
Collecting pyOpenSSL>=0.14 (from urllib3[secure,socks]~=1.26->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Downloading pyOpenSSL-24.2.1-py3-none-any.whl.metadata (13 kB)
Collecting urllib3-secure-extra (from urllib3[secure,socks]~=1.26->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Downloading urllib3_secure_extra-0.1.0-py2.py3-none-any.whl.metadata (828 bytes)
Collecting appdirs~=1.4.3 (from fs->triad>=0.9.7->fugue[dask]->-r requirements-test.txt (line 4))
  Downloading appdirs-1.4.4-py2.py3-none-any.whl.metadata (9.0 kB)
Collecting h11<1,>=0.9.0 (from wsproto>=0.14->trio-websocket~=0.9->selenium<=4.2.0,>=3.141.0->dash[testing]->-r requirements-test.txt (line 5))
  Using cached h11-0.14.0-py3-none-any.whl.metadata (8.2 kB)
Downloading pytest-8.3.2-py3-none-any.whl (341 kB)
Downloading moto-4.2.14-py2.py3-none-any.whl (3.3 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.3/3.3 MB 42.5 MB/s eta 0:00:00
Downloading adagio-0.2.6-py3-none-any.whl (19 kB)
Downloading beautifulsoup4-4.12.3-py3-none-any.whl (147 kB)
Downloading boto3-1.35.34-py3-none-any.whl (139 kB)
Downloading botocore-1.35.34-py3-none-any.whl (12.6 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 12.6/12.6 MB 105.9 MB/s eta 0:00:00
Downloading cryptography-43.0.1-cp39-abi3-macosx_10_9_universal2.whl (6.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.2/6.2 MB 101.9 MB/s eta 0:00:00
Downloading dash_testing_stub-0.0.2-py3-none-any.whl (2.6 kB)
Downloading dask-2024.8.0-py3-none-any.whl (1.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 79.7 MB/s eta 0:00:00
Downloading distributed-2024.8.0-py3-none-any.whl (1.0 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.0/1.0 MB 76.8 MB/s eta 0:00:00
Downloading lxml-5.3.0-cp39-cp39-macosx_10_9_universal2.whl (8.1 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.1/8.1 MB 105.9 MB/s eta 0:00:00
Downloading multiprocess-0.70.17-py39-none-any.whl (133 kB)
Downloading percy-2.0.2-py2.py3-none-any.whl (12 kB)
Downloading pluggy-1.5.0-py3-none-any.whl (20 kB)
Downloading pyarrow-17.0.0-cp39-cp39-macosx_11_0_arm64.whl (27.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 27.2/27.2 MB 111.4 MB/s eta 0:00:00
Downloading responses-0.25.3-py3-none-any.whl (55 kB)
Downloading selenium-4.2.0-py3-none-any.whl (983 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 983.2/983.2 kB 75.2 MB/s eta 0:00:00
Downloading triad-0.9.8-py3-none-any.whl (62 kB)
Downloading waitress-3.0.0-py3-none-any.whl (56 kB)
Downloading fugue-0.9.1-py3-none-any.whl (278 kB)
Downloading iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Downloading xmltodict-0.13.0-py2.py3-none-any.whl (10.0 kB)
Downloading cffi-1.17.1-cp39-cp39-macosx_11_0_arm64.whl (178 kB)
Downloading dask_expr-1.1.10-py3-none-any.whl (242 kB)
Downloading dill-0.3.9-py3-none-any.whl (119 kB)
Downloading fsspec-2024.9.0-py3-none-any.whl (179 kB)
Downloading jmespath-1.0.1-py3-none-any.whl (20 kB)
Downloading partd-1.4.2-py3-none-any.whl (18 kB)
Downloading PyYAML-6.0.2-cp39-cp39-macosx_11_0_arm64.whl (172 kB)
Downloading s3transfer-0.10.2-py3-none-any.whl (82 kB)
Downloading soupsieve-2.6-py3-none-any.whl (36 kB)
Downloading toolz-1.0.0-py3-none-any.whl (56 kB)
Downloading trio_websocket-0.11.1-py3-none-any.whl (17 kB)
Downloading urllib3-1.26.20-py2.py3-none-any.whl (144 kB)
Downloading fs-2.4.16-py2.py3-none-any.whl (135 kB)
Downloading appdirs-1.4.4-py2.py3-none-any.whl (9.6 kB)
Downloading locket-1.0.0-py2.py3-none-any.whl (4.4 kB)
Downloading msgpack-1.1.0-cp39-cp39-macosx_11_0_arm64.whl (81 kB)
Downloading pyOpenSSL-24.2.1-py3-none-any.whl (58 kB)
Downloading PySocks-1.7.1-py3-none-any.whl (16 kB)
Downloading tblib-3.0.0-py3-none-any.whl (12 kB)
Downloading tornado-6.4.1-cp38-abi3-macosx_10_9_universal2.whl (435 kB)
Downloading wsproto-1.2.0-py3-none-any.whl (24 kB)
Downloading zict-3.0.0-py2.py3-none-any.whl (43 kB)
Using cached pycparser-2.22-py3-none-any.whl (117 kB)
Downloading urllib3_secure_extra-0.1.0-py2.py3-none-any.whl (1.4 kB)
Using cached h11-0.14.0-py3-none-any.whl (58 kB)
Installing collected packages: urllib3-secure-extra, dash-testing-stub, appdirs, zict, xmltodict, waitress, urllib3, tornado, toolz, tblib, soupsieve, pyyaml, PySocks, pycparser, pyarrow, pluggy, msgpack, lxml, locket, jmespath, iniconfig, h11, fsspec, fs, dill, wsproto, pytest, partd, multiprocess, cffi, botocore, beautifulsoup4, trio-websocket, triad, s3transfer, responses, percy, dask, cryptography, pyOpenSSL, distributed, dask-expr, boto3, adagio, moto, fugue, selenium
  Attempting uninstall: urllib3
    Found existing installation: urllib3 2.2.3
    Uninstalling urllib3-2.2.3:
      Successfully uninstalled urllib3-2.2.3
Successfully installed PySocks-1.7.1 adagio-0.2.6 appdirs-1.4.4 beautifulsoup4-4.12.3 boto3-1.35.34 botocore-1.35.34 cffi-1.17.1 cryptography-43.0.1 dash-testing-stub-0.0.2 dask-2024.8.0 dask-expr-1.1.10 dill-0.3.9 distributed-2024.8.0 fs-2.4.16 fsspec-2024.9.0 fugue-0.9.1 h11-0.14.0 iniconfig-2.0.0 jmespath-1.0.1 locket-1.0.0 lxml-5.3.0 moto-4.2.14 msgpack-1.1.0 multiprocess-0.70.17 partd-1.4.2 percy-2.0.2 pluggy-1.5.0 pyOpenSSL-24.2.1 pyarrow-17.0.0 pycparser-2.22 pytest-8.3.2 pyyaml-6.0.2 responses-0.25.3 s3transfer-0.10.2 selenium-4.2.0 soupsieve-2.6 tblib-3.0.0 toolz-1.0.0 tornado-6.4.1 triad-0.9.8 trio-websocket-0.11.1 urllib3-1.26.20 urllib3-secure-extra-0.1.0 waitress-3.0.0 wsproto-1.2.0 xmltodict-0.13.0 zict-3.0.0</code></pre></div>

## Step 5: Buidling PyCaret From Source

After installing the dependencies, I built PyCaret from source using the 'setup.py' file:

```bash
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ python setup.py install
```

<div style="max-height: 200px; overflow-y: auto; margin-bottom: 15px;"><pre><code>/Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/setuptools/_distutils/dist.py:261: UserWarning: Unknown distribution option: 'tests_require'
  warnings.warn(msg)
running install
/Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.
!!

        ********************************************************************************
        Please avoid running ``setup.py`` directly.
        Instead, use pypa/build, pypa/installer or other
        standards-based tools.

        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.
        ********************************************************************************

!!
  self.initialize_options()
/Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: EasyInstallDeprecationWarning: easy_install command is deprecated.
!!

        ********************************************************************************
        Please avoid running ``setup.py`` and ``easy_install``.
        Instead, use pypa/build, pypa/installer or other
        standards-based tools.

        See https://github.com/pypa/setuptools/issues/917 for details.
        ********************************************************************************

!!
  self.initialize_options()
running bdist_egg
running egg_info
creating pycaret.egg-info
writing pycaret.egg-info/PKG-INFO
writing dependency_links to pycaret.egg-info/dependency_links.txt
writing requirements to pycaret.egg-info/requires.txt
writing top-level names to pycaret.egg-info/top_level.txt
writing manifest file 'pycaret.egg-info/SOURCES.txt'
reading manifest file 'pycaret.egg-info/SOURCES.txt'
reading manifest template 'MANIFEST.in'
adding license file 'LICENSE'
writing manifest file 'pycaret.egg-info/SOURCES.txt'
installing library code to build/bdist.macosx-10.9-universal2/egg
running install_lib
running build_py
creating build/lib/pycaret
copying pycaret/datasets.py -> build/lib/pycaret
copying pycaret/__init__.py -> build/lib/pycaret
copying pycaret/distributions.py -> build/lib/pycaret
creating build/lib/pycaret/classification
copying pycaret/classification/__init__.py -> build/lib/pycaret/classification
copying pycaret/classification/functional.py -> build/lib/pycaret/classification
copying pycaret/classification/oop.py -> build/lib/pycaret/classification
creating build/lib/pycaret/anomaly
copying pycaret/anomaly/__init__.py -> build/lib/pycaret/anomaly
copying pycaret/anomaly/functional.py -> build/lib/pycaret/anomaly
copying pycaret/anomaly/oop.py -> build/lib/pycaret/anomaly
creating build/lib/pycaret/parallel
copying pycaret/parallel/fugue_backend.py -> build/lib/pycaret/parallel
copying pycaret/parallel/__init__.py -> build/lib/pycaret/parallel
creating build/lib/pycaret/loggers
copying pycaret/loggers/mlflow_logger.py -> build/lib/pycaret/loggers
copying pycaret/loggers/comet_logger.py -> build/lib/pycaret/loggers
copying pycaret/loggers/wandb_logger.py -> build/lib/pycaret/loggers
copying pycaret/loggers/dagshub_logger.py -> build/lib/pycaret/loggers
copying pycaret/loggers/__init__.py -> build/lib/pycaret/loggers
copying pycaret/loggers/base_logger.py -> build/lib/pycaret/loggers
copying pycaret/loggers/dashboard_logger.py -> build/lib/pycaret/loggers
creating build/lib/pycaret/clustering
copying pycaret/clustering/__init__.py -> build/lib/pycaret/clustering
copying pycaret/clustering/functional.py -> build/lib/pycaret/clustering
copying pycaret/clustering/oop.py -> build/lib/pycaret/clustering
creating build/lib/pycaret/internal
copying pycaret/internal/logging.py -> build/lib/pycaret/internal
copying pycaret/internal/metrics.py -> build/lib/pycaret/internal
copying pycaret/internal/persistence.py -> build/lib/pycaret/internal
copying pycaret/internal/memory.py -> build/lib/pycaret/internal
copying pycaret/internal/cuml_wrappers.py -> build/lib/pycaret/internal
copying pycaret/internal/cloudpickle_compat.py -> build/lib/pycaret/internal
copying pycaret/internal/__init__.py -> build/lib/pycaret/internal
copying pycaret/internal/tunable.py -> build/lib/pycaret/internal
copying pycaret/internal/distributions.py -> build/lib/pycaret/internal
copying pycaret/internal/pipeline.py -> build/lib/pycaret/internal
copying pycaret/internal/meta_estimators.py -> build/lib/pycaret/internal
copying pycaret/internal/validation.py -> build/lib/pycaret/internal
creating build/lib/pycaret/utils
copying pycaret/utils/_dependencies.py -> build/lib/pycaret/utils
copying pycaret/utils/generic.py -> build/lib/pycaret/utils
copying pycaret/utils/constants.py -> build/lib/pycaret/utils
copying pycaret/utils/__init__.py -> build/lib/pycaret/utils
copying pycaret/utils/_show_versions.py -> build/lib/pycaret/utils
copying pycaret/utils/datetime.py -> build/lib/pycaret/utils
creating build/lib/pycaret/time_series
copying pycaret/time_series/__init__.py -> build/lib/pycaret/time_series
creating build/lib/pycaret/containers
copying pycaret/containers/__init__.py -> build/lib/pycaret/containers
copying pycaret/containers/base_container.py -> build/lib/pycaret/containers
creating build/lib/pycaret/regression
copying pycaret/regression/__init__.py -> build/lib/pycaret/regression
copying pycaret/regression/functional.py -> build/lib/pycaret/regression
copying pycaret/regression/oop.py -> build/lib/pycaret/regression
creating build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/supervised_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/ts_supervised_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/non_ts_supervised_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/__init__.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/tabular_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/pycaret_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
copying pycaret/internal/pycaret_experiment/unsupervised_experiment.py -> build/lib/pycaret/internal/pycaret_experiment
creating build/lib/pycaret/internal/parallel
copying pycaret/internal/parallel/__init__.py -> build/lib/pycaret/internal/parallel
copying pycaret/internal/parallel/parallel_backend.py -> build/lib/pycaret/internal/parallel
creating build/lib/pycaret/internal/patches
copying pycaret/internal/patches/__init__.py -> build/lib/pycaret/internal/patches
copying pycaret/internal/patches/pyod.py -> build/lib/pycaret/internal/patches
copying pycaret/internal/patches/yellowbrick.py -> build/lib/pycaret/internal/patches
copying pycaret/internal/patches/sklearn.py -> build/lib/pycaret/internal/patches
creating build/lib/pycaret/internal/tests
copying pycaret/internal/tests/time_series.py -> build/lib/pycaret/internal/tests
copying pycaret/internal/tests/__init__.py -> build/lib/pycaret/internal/tests
copying pycaret/internal/tests/stats.py -> build/lib/pycaret/internal/tests
creating build/lib/pycaret/internal/preprocess
copying pycaret/internal/preprocess/transformers.py -> build/lib/pycaret/internal/preprocess
copying pycaret/internal/preprocess/__init__.py -> build/lib/pycaret/internal/preprocess
copying pycaret/internal/preprocess/preprocessor.py -> build/lib/pycaret/internal/preprocess
copying pycaret/internal/preprocess/iterative_imputer.py -> build/lib/pycaret/internal/preprocess
creating build/lib/pycaret/internal/display
copying pycaret/internal/display/__init__.py -> build/lib/pycaret/internal/display
copying pycaret/internal/display/display_backend.py -> build/lib/pycaret/internal/display
copying pycaret/internal/display/display.py -> build/lib/pycaret/internal/display
copying pycaret/internal/display/display_component.py -> build/lib/pycaret/internal/display
copying pycaret/internal/display/progress_bar.py -> build/lib/pycaret/internal/display
creating build/lib/pycaret/internal/plots
copying pycaret/internal/plots/time_series.py -> build/lib/pycaret/internal/plots
copying pycaret/internal/plots/__init__.py -> build/lib/pycaret/internal/plots
copying pycaret/internal/plots/helper.py -> build/lib/pycaret/internal/plots
copying pycaret/internal/plots/yellowbrick.py -> build/lib/pycaret/internal/plots
copying pycaret/internal/plots/residual_plots.py -> build/lib/pycaret/internal/plots
creating build/lib/pycaret/internal/preprocess/target
copying pycaret/internal/preprocess/target/TransformedTargetRegressor.py -> build/lib/pycaret/internal/preprocess/target
copying pycaret/internal/preprocess/target/__init__.py -> build/lib/pycaret/internal/preprocess/target
copying pycaret/internal/preprocess/target/utils.py -> build/lib/pycaret/internal/preprocess/target
copying pycaret/internal/preprocess/target/TransformedTargetClassifier.py -> build/lib/pycaret/internal/preprocess/target
creating build/lib/pycaret/internal/preprocess/time_series
copying pycaret/internal/preprocess/time_series/__init__.py -> build/lib/pycaret/internal/preprocess/time_series
creating build/lib/pycaret/internal/preprocess/time_series/forecasting
copying pycaret/internal/preprocess/time_series/forecasting/__init__.py -> build/lib/pycaret/internal/preprocess/time_series/forecasting
copying pycaret/internal/preprocess/time_series/forecasting/preprocessor.py -> build/lib/pycaret/internal/preprocess/time_series/forecasting
creating build/lib/pycaret/internal/plots/utils
copying pycaret/internal/plots/utils/time_series.py -> build/lib/pycaret/internal/plots/utils
copying pycaret/internal/plots/utils/__init__.py -> build/lib/pycaret/internal/plots/utils
creating build/lib/pycaret/utils/time_series
copying pycaret/utils/time_series/__init__.py -> build/lib/pycaret/utils/time_series
copying pycaret/utils/time_series/exceptions.py -> build/lib/pycaret/utils/time_series
creating build/lib/pycaret/utils/time_series/forecasting
copying pycaret/utils/time_series/forecasting/models.py -> build/lib/pycaret/utils/time_series/forecasting
copying pycaret/utils/time_series/forecasting/model_selection.py -> build/lib/pycaret/utils/time_series/forecasting
copying pycaret/utils/time_series/forecasting/__init__.py -> build/lib/pycaret/utils/time_series/forecasting
copying pycaret/utils/time_series/forecasting/pipeline.py -> build/lib/pycaret/utils/time_series/forecasting
creating build/lib/pycaret/time_series/forecasting
copying pycaret/time_series/forecasting/__init__.py -> build/lib/pycaret/time_series/forecasting
copying pycaret/time_series/forecasting/functional.py -> build/lib/pycaret/time_series/forecasting
copying pycaret/time_series/forecasting/oop.py -> build/lib/pycaret/time_series/forecasting
creating build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/regression.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/clustering.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/classification.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/time_series.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/__init__.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/base_metric.py -> build/lib/pycaret/containers/metrics
copying pycaret/containers/metrics/anomaly.py -> build/lib/pycaret/containers/metrics
creating build/lib/pycaret/containers/models
copying pycaret/containers/models/regression.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/clustering.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/classification.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/time_series.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/__init__.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/base_model.py -> build/lib/pycaret/containers/models
copying pycaret/containers/models/anomaly.py -> build/lib/pycaret/containers/models
creating build/bdist.macosx-10.9-universal2/egg
creating build/bdist.macosx-10.9-universal2/egg/pycaret
creating build/bdist.macosx-10.9-universal2/egg/pycaret/classification
copying build/lib/pycaret/classification/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/classification
copying build/lib/pycaret/classification/functional.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/classification
copying build/lib/pycaret/classification/oop.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/classification
creating build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly
copying build/lib/pycaret/anomaly/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly
copying build/lib/pycaret/anomaly/functional.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly
copying build/lib/pycaret/anomaly/oop.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly
creating build/bdist.macosx-10.9-universal2/egg/pycaret/parallel
copying build/lib/pycaret/parallel/fugue_backend.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/parallel
copying build/lib/pycaret/parallel/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/parallel
creating build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/mlflow_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/comet_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/wandb_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/dagshub_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/base_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
copying build/lib/pycaret/loggers/dashboard_logger.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/loggers
creating build/bdist.macosx-10.9-universal2/egg/pycaret/clustering
copying build/lib/pycaret/clustering/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/clustering
copying build/lib/pycaret/clustering/functional.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/clustering
copying build/lib/pycaret/clustering/oop.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/clustering
copying build/lib/pycaret/datasets.py -> build/bdist.macosx-10.9-universal2/egg/pycaret
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/supervised_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/ts_supervised_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/non_ts_supervised_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/tabular_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/pycaret_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/pycaret_experiment/unsupervised_experiment.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment
copying build/lib/pycaret/internal/logging.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/metrics.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/parallel
copying build/lib/pycaret/internal/parallel/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/parallel
copying build/lib/pycaret/internal/parallel/parallel_backend.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/parallel
copying build/lib/pycaret/internal/persistence.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/memory.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches
copying build/lib/pycaret/internal/patches/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches
copying build/lib/pycaret/internal/patches/pyod.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches
copying build/lib/pycaret/internal/patches/yellowbrick.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches
copying build/lib/pycaret/internal/patches/sklearn.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches
copying build/lib/pycaret/internal/cuml_wrappers.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests
copying build/lib/pycaret/internal/tests/time_series.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests
copying build/lib/pycaret/internal/tests/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests
copying build/lib/pycaret/internal/tests/stats.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests
copying build/lib/pycaret/internal/cloudpickle_compat.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess
copying build/lib/pycaret/internal/preprocess/transformers.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target
copying build/lib/pycaret/internal/preprocess/target/TransformedTargetRegressor.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target
copying build/lib/pycaret/internal/preprocess/target/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target
copying build/lib/pycaret/internal/preprocess/target/utils.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target
copying build/lib/pycaret/internal/preprocess/target/TransformedTargetClassifier.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target
copying build/lib/pycaret/internal/preprocess/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess
copying build/lib/pycaret/internal/preprocess/preprocessor.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess
copying build/lib/pycaret/internal/preprocess/iterative_imputer.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series
copying build/lib/pycaret/internal/preprocess/time_series/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/forecasting
copying build/lib/pycaret/internal/preprocess/time_series/forecasting/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/forecasting
copying build/lib/pycaret/internal/preprocess/time_series/forecasting/preprocessor.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/forecasting
copying build/lib/pycaret/internal/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/tunable.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/distributions.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/pipeline.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/internal/meta_estimators.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
copying build/lib/pycaret/internal/display/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
copying build/lib/pycaret/internal/display/display_backend.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
copying build/lib/pycaret/internal/display/display.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
copying build/lib/pycaret/internal/display/display_component.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
copying build/lib/pycaret/internal/display/progress_bar.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
copying build/lib/pycaret/internal/plots/time_series.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
copying build/lib/pycaret/internal/plots/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
creating build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/utils
copying build/lib/pycaret/internal/plots/utils/time_series.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/utils
copying build/lib/pycaret/internal/plots/utils/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/utils
copying build/lib/pycaret/internal/plots/helper.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
copying build/lib/pycaret/internal/plots/yellowbrick.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
copying build/lib/pycaret/internal/plots/residual_plots.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots
copying build/lib/pycaret/internal/validation.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/internal
copying build/lib/pycaret/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret
creating build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/utils/_dependencies.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/utils/generic.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/utils/constants.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/utils/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
creating build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series
copying build/lib/pycaret/utils/time_series/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series
copying build/lib/pycaret/utils/time_series/exceptions.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series
creating build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting
copying build/lib/pycaret/utils/time_series/forecasting/models.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting
copying build/lib/pycaret/utils/time_series/forecasting/model_selection.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting
copying build/lib/pycaret/utils/time_series/forecasting/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting
copying build/lib/pycaret/utils/time_series/forecasting/pipeline.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting
copying build/lib/pycaret/utils/_show_versions.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/utils/datetime.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/utils
copying build/lib/pycaret/distributions.py -> build/bdist.macosx-10.9-universal2/egg/pycaret
creating build/bdist.macosx-10.9-universal2/egg/pycaret/time_series
copying build/lib/pycaret/time_series/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/time_series
creating build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting
copying build/lib/pycaret/time_series/forecasting/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting
copying build/lib/pycaret/time_series/forecasting/functional.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting
copying build/lib/pycaret/time_series/forecasting/oop.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting
creating build/bdist.macosx-10.9-universal2/egg/pycaret/containers
creating build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/regression.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/clustering.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/classification.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/time_series.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/base_metric.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/metrics/anomaly.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics
copying build/lib/pycaret/containers/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers
copying build/lib/pycaret/containers/base_container.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers
creating build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/regression.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/clustering.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/classification.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/time_series.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/base_model.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
copying build/lib/pycaret/containers/models/anomaly.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models
creating build/bdist.macosx-10.9-universal2/egg/pycaret/regression
copying build/lib/pycaret/regression/__init__.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/regression
copying build/lib/pycaret/regression/functional.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/regression
copying build/lib/pycaret/regression/oop.py -> build/bdist.macosx-10.9-universal2/egg/pycaret/regression
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/classification/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/classification/functional.py to functional.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/classification/oop.py to oop.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly/functional.py to functional.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/anomaly/oop.py to oop.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/parallel/fugue_backend.py to fugue_backend.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/parallel/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/mlflow_logger.py to mlflow_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/comet_logger.py to comet_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/wandb_logger.py to wandb_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/dagshub_logger.py to dagshub_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/base_logger.py to base_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/loggers/dashboard_logger.py to dashboard_logger.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/clustering/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/clustering/functional.py to functional.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/clustering/oop.py to oop.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/datasets.py to datasets.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/supervised_experiment.py to supervised_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/ts_supervised_experiment.py to ts_supervised_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/non_ts_supervised_experiment.py to non_ts_supervised_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/tabular_experiment.py to tabular_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/pycaret_experiment.py to pycaret_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pycaret_experiment/unsupervised_experiment.py to unsupervised_experiment.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/logging.py to logging.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/metrics.py to metrics.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/parallel/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/parallel/parallel_backend.py to parallel_backend.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/persistence.py to persistence.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/memory.py to memory.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches/pyod.py to pyod.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches/yellowbrick.py to yellowbrick.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/patches/sklearn.py to sklearn.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/cuml_wrappers.py to cuml_wrappers.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests/time_series.py to time_series.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tests/stats.py to stats.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/cloudpickle_compat.py to cloudpickle_compat.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/transformers.py to transformers.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target/TransformedTargetRegressor.py to TransformedTargetRegressor.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target/utils.py to utils.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/target/TransformedTargetClassifier.py to TransformedTargetClassifier.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/preprocessor.py to preprocessor.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/iterative_imputer.py to iterative_imputer.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/forecasting/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/preprocess/time_series/forecasting/preprocessor.py to preprocessor.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/tunable.py to tunable.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/distributions.py to distributions.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/pipeline.py to pipeline.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/meta_estimators.py to meta_estimators.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display/display_backend.py to display_backend.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display/display.py to display.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display/display_component.py to display_component.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/display/progress_bar.py to progress_bar.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/time_series.py to time_series.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/utils/time_series.py to time_series.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/utils/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/helper.py to helper.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/yellowbrick.py to yellowbrick.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/plots/residual_plots.py to residual_plots.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/internal/validation.py to validation.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/_dependencies.py to _dependencies.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/generic.py to generic.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/constants.py to constants.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/exceptions.py to exceptions.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting/models.py to models.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting/model_selection.py to model_selection.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/time_series/forecasting/pipeline.py to pipeline.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/_show_versions.py to _show_versions.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/utils/datetime.py to datetime.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/distributions.py to distributions.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting/functional.py to functional.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/time_series/forecasting/oop.py to oop.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/regression.py to regression.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/clustering.py to clustering.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/classification.py to classification.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/time_series.py to time_series.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/base_metric.py to base_metric.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/metrics/anomaly.py to anomaly.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/base_container.py to base_container.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/regression.py to regression.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/clustering.py to clustering.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/classification.py to classification.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/time_series.py to time_series.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/base_model.py to base_model.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/containers/models/anomaly.py to anomaly.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/regression/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/regression/functional.py to functional.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-universal2/egg/pycaret/regression/oop.py to oop.cpython-39.pyc
creating build/bdist.macosx-10.9-universal2/egg/EGG-INFO
copying pycaret.egg-info/PKG-INFO -> build/bdist.macosx-10.9-universal2/egg/EGG-INFO
copying pycaret.egg-info/SOURCES.txt -> build/bdist.macosx-10.9-universal2/egg/EGG-INFO
copying pycaret.egg-info/dependency_links.txt -> build/bdist.macosx-10.9-universal2/egg/EGG-INFO
copying pycaret.egg-info/requires.txt -> build/bdist.macosx-10.9-universal2/egg/EGG-INFO
copying pycaret.egg-info/top_level.txt -> build/bdist.macosx-10.9-universal2/egg/EGG-INFO
zip_safe flag not set; analyzing archive contents...
creating dist
creating 'dist/pycaret-3.4.0-py3.9.egg' and adding 'build/bdist.macosx-10.9-universal2/egg' to it
removing 'build/bdist.macosx-10.9-universal2/egg' (and everything under it)
Processing pycaret-3.4.0-py3.9.egg
Copying pycaret-3.4.0-py3.9.egg to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Adding pycaret 3.4.0 to easy-install.pth file

Installed /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/pycaret-3.4.0-py3.9.egg
Processing dependencies for pycaret==3.4.0
Searching for wurlitzer==3.1.1
Best match: wurlitzer 3.1.1
Adding wurlitzer 3.1.1 to easy-install.pth file
detected new path './pycaret-3.4.0-py3.9.egg'

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pmdarima==2.0.4
Best match: pmdarima 2.0.4
Adding pmdarima 2.0.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for tbats==1.1.3
Best match: tbats 1.1.3
Adding tbats 1.1.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for sktime==0.33.1
Best match: sktime 0.33.1
Adding sktime 0.33.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for statsmodels==0.14.4
Best match: statsmodels 0.14.4
Adding statsmodels 0.14.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for plotly-resampler==0.10.0
Best match: plotly-resampler 0.10.0
Adding plotly-resampler 0.10.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for schemdraw==0.15
Best match: schemdraw 0.15
Adding schemdraw 0.15 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for kaleido==0.2.1
Best match: kaleido 0.2.1
Adding kaleido 0.2.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for plotly==5.24.1
Best match: plotly 5.24.1
Adding plotly 5.24.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for yellowbrick==1.5
Best match: yellowbrick 1.5
Adding yellowbrick 1.5 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for mljar-scikit-plot==0.3.12
Best match: mljar-scikit-plot 0.3.12
Adding mljar-scikit-plot 0.3.12 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for matplotlib==3.7.5
Best match: matplotlib 3.7.5
Adding matplotlib 3.7.5 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for trio==0.24.0
Best match: trio 0.24.0
Adding trio 0.24.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for xxhash==3.5.0
Best match: xxhash 3.5.0
Adding xxhash 3.5.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for deprecation==2.1.0
Best match: deprecation 2.1.0
Adding deprecation 2.1.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for cloudpickle==3.0.0
Best match: cloudpickle 3.0.0
Adding cloudpickle 3.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for nbformat==5.10.4
Best match: nbformat 5.10.4
Adding nbformat 5.10.4 to easy-install.pth file
Installing jupyter-trust script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for importlib-metadata==8.5.0
Best match: importlib-metadata 8.5.0
Adding importlib-metadata 8.5.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for MarkupSafe==2.1.5
Best match: MarkupSafe 2.1.5
Adding MarkupSafe 2.1.5 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for psutil==6.0.0
Best match: psutil 6.0.0
Adding psutil 6.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for requests==2.32.3
Best match: requests 2.32.3
Adding requests 2.32.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for numba==0.60.0
Best match: numba 0.60.0
Adding numba 0.60.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for lightgbm==4.5.0
Best match: lightgbm 4.5.0
Adding lightgbm 4.5.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for category-encoders==2.6.4
Best match: category-encoders 2.6.4
Adding category-encoders 2.6.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for imbalanced-learn==0.12.4
Best match: imbalanced-learn 0.12.4
Adding imbalanced-learn 0.12.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pyod==2.0.2
Best match: pyod 2.0.2
Adding pyod 2.0.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for scikit-learn==1.5.2
Best match: scikit-learn 1.5.2
Adding scikit-learn 1.5.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for joblib==1.3.2
Best match: joblib 1.3.2
Adding joblib 1.3.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for scipy==1.11.4
Best match: scipy 1.11.4
Adding scipy 1.11.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jinja2==3.1.4
Best match: jinja2 3.1.4
Adding jinja2 3.1.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pandas==2.2.3
Best match: pandas 2.2.3
Adding pandas 2.2.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for numpy==1.26.4
Best match: numpy 1.26.4
Adding numpy 1.26.4 to easy-install.pth file
Installing f2py script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for tqdm==4.66.5
Best match: tqdm 4.66.5
Adding tqdm 4.66.5 to easy-install.pth file
Installing tqdm script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for ipywidgets==8.1.5
Best match: ipywidgets 8.1.5
Adding ipywidgets 8.1.5 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for ipython==8.18.1
Best match: ipython 8.18.1
Adding ipython 8.18.1 to easy-install.pth file
Installing ipython script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing ipython3 script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for packaging==24.1
Best match: packaging 24.1
Adding packaging 24.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/setuptools/_vendor
Searching for setuptools==75.1.0
Best match: setuptools 75.1.0
Adding setuptools 75.1.0 to easy-install.pth file
detected new path './setuptools/_vendor'

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for urllib3==1.26.20
Best match: urllib3 1.26.20
Adding urllib3 1.26.20 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for Cython==3.0.11
Best match: Cython 3.0.11
Adding Cython 3.0.11 to easy-install.pth file
Installing cygdb script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing cython script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing cythonize script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for scikit-base==0.8.3
Best match: scikit-base 0.8.3
Adding scikit-base 0.8.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for patsy==0.5.6
Best match: patsy 0.5.6
Adding patsy 0.5.6 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for tsdownsample==0.1.3
Best match: tsdownsample 0.1.3
Adding tsdownsample 0.1.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for orjson==3.10.7
Best match: orjson 3.10.7
Adding orjson 3.10.7 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for dash==2.18.1
Best match: dash 2.18.1
Adding dash 2.18.1 to easy-install.pth file
Installing dash-generate-components script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing dash-update-components script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing renderer script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for tenacity==9.0.0
Best match: tenacity 9.0.0
Adding tenacity 9.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for cycler==0.12.1
Best match: cycler 0.12.1
Adding cycler 0.12.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for importlib-resources==6.4.5
Best match: importlib-resources 6.4.5
Adding importlib-resources 6.4.5 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for python-dateutil==2.9.0.post0
Best match: python-dateutil 2.9.0.post0
Adding python-dateutil 2.9.0.post0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pyparsing==3.1.4
Best match: pyparsing 3.1.4
Adding pyparsing 3.1.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pillow==10.4.0
Best match: pillow 10.4.0
Adding pillow 10.4.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for kiwisolver==1.4.7
Best match: kiwisolver 1.4.7
Adding kiwisolver 1.4.7 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for fonttools==4.54.1
Best match: fonttools 4.54.1
Adding fonttools 4.54.1 to easy-install.pth file
Installing fonttools script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing pyftmerge script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing pyftsubset script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing ttx script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for contourpy==1.3.0
Best match: contourpy 1.3.0
Adding contourpy 1.3.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for exceptiongroup==1.2.2
Best match: exceptiongroup 1.2.2
Adding exceptiongroup 1.2.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for sniffio==1.3.1
Best match: sniffio 1.3.1
Adding sniffio 1.3.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for outcome==1.3.0.post0
Best match: outcome 1.3.0.post0
Adding outcome 1.3.0.post0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for idna==3.10
Best match: idna 3.10
Adding idna 3.10 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for sortedcontainers==2.4.0
Best match: sortedcontainers 2.4.0
Adding sortedcontainers 2.4.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for attrs==24.2.0
Best match: attrs 24.2.0
Adding attrs 24.2.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for traitlets==5.14.3
Best match: traitlets 5.14.3
Adding traitlets 5.14.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jupyter-core==5.7.2
Best match: jupyter-core 5.7.2
Adding jupyter-core 5.7.2 to easy-install.pth file
Installing jupyter script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing jupyter-migrate script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin
Installing jupyter-troubleshoot script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jsonschema==4.23.0
Best match: jsonschema 4.23.0
Adding jsonschema 4.23.0 to easy-install.pth file
Installing jsonschema script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for fastjsonschema==2.20.0
Best match: fastjsonschema 2.20.0
Adding fastjsonschema 2.20.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for zipp==3.20.2
Best match: zipp 3.20.2
Adding zipp 3.20.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for certifi==2024.8.30
Best match: certifi 2024.8.30
Adding certifi 2024.8.30 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for charset-normalizer==3.3.2
Best match: charset-normalizer 3.3.2
Adding charset-normalizer 3.3.2 to easy-install.pth file
Installing normalizer script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for llvmlite==0.43.0
Best match: llvmlite 0.43.0
Adding llvmlite 0.43.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for threadpoolctl==3.5.0
Best match: threadpoolctl 3.5.0
Adding threadpoolctl 3.5.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for tzdata==2024.2
Best match: tzdata 2024.2
Adding tzdata 2024.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pytz==2024.2
Best match: pytz 2024.2
Adding pytz 2024.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jupyterlab-widgets==3.0.13
Best match: jupyterlab-widgets 3.0.13
Adding jupyterlab-widgets 3.0.13 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for widgetsnbextension==4.0.13
Best match: widgetsnbextension 4.0.13
Adding widgetsnbextension 4.0.13 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for comm==0.2.2
Best match: comm 0.2.2
Adding comm 0.2.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pexpect==4.9.0
Best match: pexpect 4.9.0
Adding pexpect 4.9.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for typing-extensions==4.12.2
Best match: typing-extensions 4.12.2
typing-extensions 4.12.2 is already the active version in easy-install.pth

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages/setuptools/_vendor
Searching for stack-data==0.6.3
Best match: stack-data 0.6.3
Adding stack-data 0.6.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pygments==2.18.0
Best match: pygments 2.18.0
Adding pygments 2.18.0 to easy-install.pth file
Installing pygmentize script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for prompt-toolkit==3.0.48
Best match: prompt-toolkit 3.0.48
Adding prompt-toolkit 3.0.48 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for matplotlib-inline==0.1.7
Best match: matplotlib-inline 0.1.7
Adding matplotlib-inline 0.1.7 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jedi==0.19.1
Best match: jedi 0.19.1
Adding jedi 0.19.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for decorator==5.1.1
Best match: decorator 5.1.1
Adding decorator 5.1.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for six==1.16.0
Best match: six 1.16.0
Adding six 1.16.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for nest-asyncio==1.6.0
Best match: nest-asyncio 1.6.0
Adding nest-asyncio 1.6.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for retrying==1.3.4
Best match: retrying 1.3.4
Adding retrying 1.3.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for dash-table==5.0.0
Best match: dash-table 5.0.0
Adding dash-table 5.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for dash-core-components==2.0.0
Best match: dash-core-components 2.0.0
Adding dash-core-components 2.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for dash-html-components==2.0.0
Best match: dash-html-components 2.0.0
Adding dash-html-components 2.0.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for werkzeug==3.0.4
Best match: werkzeug 3.0.4
Adding werkzeug 3.0.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for flask==3.0.3
Best match: flask 3.0.3
Adding flask 3.0.3 to easy-install.pth file
Installing flask script to /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/bin

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for platformdirs==4.3.6
Best match: platformdirs 4.3.6
Adding platformdirs 4.3.6 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for rpds-py==0.20.0
Best match: rpds-py 0.20.0
Adding rpds-py 0.20.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for referencing==0.35.1
Best match: referencing 0.35.1
Adding referencing 0.35.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for jsonschema-specifications==2023.12.1
Best match: jsonschema-specifications 2023.12.1
Adding jsonschema-specifications 2023.12.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for ptyprocess==0.7.0
Best match: ptyprocess 0.7.0
Adding ptyprocess 0.7.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for pure-eval==0.2.3
Best match: pure-eval 0.2.3
Adding pure-eval 0.2.3 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for asttokens==2.4.1
Best match: asttokens 2.4.1
Adding asttokens 2.4.1 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for executing==2.1.0
Best match: executing 2.1.0
Adding executing 2.1.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for wcwidth==0.2.13
Best match: wcwidth 0.2.13
Adding wcwidth 0.2.13 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for parso==0.8.4
Best match: parso 0.8.4
Adding parso 0.8.4 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for blinker==1.8.2
Best match: blinker 1.8.2
Adding blinker 1.8.2 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for click==8.1.7
Best match: click 8.1.7
Adding click 8.1.7 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Searching for itsdangerous==2.2.0
Best match: itsdangerous 2.2.0
Adding itsdangerous 2.2.0 to easy-install.pth file

Using /Users/mhsizar/Desktop/Class/pycaret/pycaret-env/lib/python3.9/site-packages
Finished processing dependencies for pycaret==3.4.0