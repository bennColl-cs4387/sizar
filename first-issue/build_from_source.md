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

## Step 3: Set Up a Virtual Environment

To avoid conflicts with other packages, I set up a Python vitual environment:
```bash
➜  pycaret git:(build-from-source) python -m venv pycaret-env
➜  pycaret git:(build-from-source) ✗ source pycaret-env/bin/activate
(pycaret-env) ➜  pycaret git:(build-from-source) ✗ 
```

