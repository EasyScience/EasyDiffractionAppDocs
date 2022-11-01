# Getting Started

## Downloading

To make the installation of **EasyDiffraction** as easy as possible, we prepared installers for three major operating systems: Windows, macOS and Linux (Ubuntu). You can download the latest and previous versions from the [releases page](https://github.com/easyscience/easyDiffractionApp/releases).

## Installing

Run **EasyDiffraction** installer and follow the instructions.

### Common Issues

- On `macOS`, if you see the message _EasyDiffractionSetup.app can't be opened because it is from an unidentified developer_, do the following:
In the **Finder**, locate the **EasyDiffraction** installer application, then _control-click_ the installer icon, then choose _Open_ from the shortcut menu and finally click _Open_.
- On `Linux` based system there can be the following error on startup: _Failed to create OpenGL context for format QSurfaceFormat_. This is due to a system OpenGL driver problem. Please re-install your graphics card drivers.

## Uninstalling

Run **MaintenanceTool** from the **EasyDiffraction** installation directory, select _Remove all components_ and follow the instructions.

## Installation from source

If the relevant **EasyDiffraction** installation does not work on your system, then please try installation from source.

* Install [**Poetry**](https://python-poetry.org), the Python dependency manager, following the [official instructions](https://python-poetry.org/docs/#installation).
* Clone **easyDiffractionApp** repo from GitHub:
  ```
  git clone https://github.com/easyscience/easyDiffractionApp
  ```
* Go to **easyDiffractionApp** directory.
* Create virtual environment for **easyDiffractionApp** and install its dependences using **Poetry**:
  ```
  poetry install
  ```  
5. Launch **EasyDiffraction** application using **poetry**:
  ```
  poetry run easyDiffraction
  ```