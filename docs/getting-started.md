# Getting started

## Standard installation

### Downloading

To make the installation of EasyDiffraction as easy as possible, we prepared installers for three major operating systems: Windows, macOS and Linux (Ubuntu). You can download the latest version from the [EasyDiffraction home page](https://easydiffraction.org). All previous versions are available on the [GitHub releases page](https://github.com/easyscience/easyDiffractionApp/releases).

### Installing

Run EasyDiffraction installer and follow the instructions.

### Uninstalling

Run MaintenanceTool from the EasyDiffraction installation directory, select _Remove all components_ and follow the instructions.

## Installation from source

If the relevant EasyDiffraction installation does not work on your system, then please try running it from source.

* Clone EasyDiffractionBeta repo (master branch) from GitHub, e.g. using
```console
git clone https://github.com/EasyScience/EasyDiffractionBeta
```
* Go to EasyDiffractionBeta directory
```console
cd EasyDiffractionBeta
```  
* Create Python environment and activate it
```console
python3.11 -m venv .venv
source .venv/bin/activate
```  
* Upgrade pip and install dependences
```console
pip install --upgrade pip
pip install numpy lmfit numdifftools
pip install orjson jsbeautifier
pip install git+https://github.com/ikibalin/cryspy.git@beta
pip install git+https://github.com/easyscience/EasyApp.git@new-easy-app2
```  
* Launch EasyDiffraction application using Python
```console
cd easyDiffractionApp
python main.py
```

## Installation without user interaction

The following example demonstrates how to install EasyDiffraction v0.9.5 on Ubuntu 22.04 from the command line interface
without user interaction.

This can be useful, for example, to install EasyDiffraction on
[VISA](https://www.panosc.eu/services/data-analysis), the Virtual Infrastructure for Scientific Analysis. VISA
provides access to remote desktop environments, enabling users to remotely analyse data during or after the experiment.

* Download the required version of EasyDiffraction from GitHub releases
```console
wget -c https://github.com/EasyScience/EasyDiffractionBeta/releases/download/v0.9.5/EasyDiffraction_v0.9.5_ubuntu-22.04.zip
```
* Unpack downloaded file
```console
unzip EasyDiffraction_v0.9.5_ubuntu-22.04.zip
```  
* You can now install EasyDiffraction with options for unattended usage
```console
./EasyDiffraction_v0.9.5_ubuntu-22.04 install --verbose --confirm-command --default-answer --accept-licenses
```  
* Run the installed application from the command line
```console
~/EasyDiffraction/EasyDiffraction/EasyDiffraction
```  
