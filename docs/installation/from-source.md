# Installation from source

If the relevant **EasyDiffraction** installation does not work on your system, then please try running it from source.

* Clone **easyDiffractionApp** repo from GitHub, e.g. using
```console
$ git clone --branch release-0.9.0 https://github.com/easyscience/easyDiffractionApp
```
* Go to **easyDiffractionApp** directory
```console
$ cd easyDiffractionApp
```  
* Create Python environment and activate it
```console
$ python3.11 -m venv .venv
$ source .venv/bin/activate
```  
* Upgrade PIP and install dependences
```console
$ pip install --upgrade pip
$ pip install lmfit orjson jsbeautifier
$ pip install git+https://github.com/ikibalin/cryspy.git@beta
$ pip install git+https://github.com/easyscience/EasyApp.git@new-easy-app2
```  
* Launch **EasyDiffraction** application using Python
```console
$ cd EasyDiffractionApp
$ python main.py
```

<!-- Abbreviations -->

*[PIP]: Package installer for Python.
