# Installation without user interaction

The following example demonstrates how to install **EasyDiffraction** v0.9.5 on Ubuntu 22.04 from the command line interface 
without user interaction.

This can be useful, for example, to install **EasyDiffraction** on 
[VISA](https://www.panosc.eu/services/data-analysis), the Virtual Infrastructure for Scientific Analysis. VISA 
provides access to remote desktop environments, enabling users to remotely analyse data during or after the experiment.

* Download the required version of **EasyDiffraction** from GitHub releases
```console
$ wget -c https://github.com/EasyScience/EasyDiffractionBeta/releases/download/v0.9.5/EasyDiffraction_v0.9.5_ubuntu-22.04.zip
```
* Unpack downloaded file
```console
$ unzip EasyDiffraction_v0.9.5_ubuntu-22.04.zip
```  
* You can now install **EasyDiffraction** with options for unattended usage
```console
$ ./EasyDiffraction_v0.9.5_ubuntu-22.04.zip install --verbose --confirm-command --default-answer --accept-licenses
```  
* Run the installed application from the command line
```console
$ ~/EasyDiffraction/EasyDiffraction/EasyDiffraction
```  
