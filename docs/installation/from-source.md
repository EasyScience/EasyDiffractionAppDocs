# Installation from source

If the relevant **EasyDiffraction** installation does not work on your system, then please try running it from source.

* Clone **EasyDiffractionBeta** repo (master branch) from GitHub, e.g. using
```console
$ git clone https://github.com/easyscience/EasyDiffractionBeta
```
* Go to **EasyDiffractionBeta** directory
```console
$ cd EasyDiffractionBeta
```  
* Create Python environment and activate it
```console
$ python3.11 -m venv .venv
$ source .venv/bin/activate
```  
* Upgrade PIP and install dependences
```console
$ pip install --upgrade pip
$ pip install numpy lmfit numdifftools
$ pip install orjson jsbeautifier
$ pip install git+https://github.com/ikibalin/cryspy.git@beta
$ pip install git+https://github.com/easyscience/EasyApp.git@new-easy-app2
```  
* Launch **EasyDiffraction** application using Python
```console
$ cd easyDiffractionApp
$ python main.py
```

<!-- Abbreviations -->

*[PIP]: Package installer for Python.
