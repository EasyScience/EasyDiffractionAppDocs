# User Interface

Here you can see what the program looks like. The application window is divided into parts that provide you with quick and easy access to everything you'll need. The parts are `Toolbar`, `Main Window`, `Sidebar` and `Status Bar` described in the following sections.

![](../assets/images/app-window_lightmode.png#gh-light-mode-only)
![](../assets/images/app-window_darkmode.png#gh-dark-mode-only)

## Toolbar

The `Toolbar` at the top of the application window contains three groups of buttons, indicated on the screenshot below.

![](../assets/images/app-toolbar-groups_lightmode.png#gh-light-mode-only)
![](../assets/images/app-toolbar-groups_darkmode.png#gh-dark-mode-only)

The left and right groups of buttons, **group A** and **group C**, allow you to call some basic application actions, such as saving the project state, undo/redo, open the application settings, etc.

The central group of buttons, **group B**, represents the data analysis workflow. After the application starts, all the toolbar workflow buttons except the `Home` button are disabled. When each step in the workflow is completed, the toolbar workflow button which corresponds to the next step becomes enabled.

![](../assets/images/app-toolbar-tabs_lightmode.png#gh-light-mode-only)
![](../assets/images/app-toolbar-tabs_darkmode.png#gh-dark-mode-only)

The following workflow buttons or workflow steps are present:

1. `Home` introduction page, links to about, help and contact.
2. `Project` to manage your project (create new, open existing, etc.)
3. `Model` to describe crystallographic phase models.
4. `Experiment` to load experimentally measured data files.
5. `Analysis` to perform refinement of structural parameters.
6. `Summary` to view and export summary report.

## Main window

The `Main Window` of the program is located below the `Toolbar` and it can contain several tabs depending on the current step in the data analysis workflow. An example of the `Main Window` for the analysis step is shown in the figure below.

![](../assets/images/mainwindow-tabs_lightmode.png#gh-light-mode-only)
![](../assets/images/mainwindow-tabs_darkmode.png#gh-dark-mode-only)

## Sidebar

The `Sidebar` is located at the right side of the application window, below the `Toolbar`. It has 2 tabs: `Basic controls` and `Advanced controls`. Their contents depend on the selected tab in the `Toolbar` and the respective tab in the `Main Window`. You can switch between them at any time clicking on the required tab.

![](../assets/images/sidebar-tabs_lightmode.png#gh-light-mode-only)
![](../assets/images/sidebar-tabs_darkmode.png#gh-dark-mode-only)

1. `Basic controls` tab provides an access to essential actions and information fields.
2. `Advanced controls` tab describes additional actions recommended for advanced users.
2. `Text mode` tab contains all controls in plain text, as STAR/CIF.

## Status bar

The `Status bar` is located at the very bottom of the application window. It contains some important information, such as project name, number of defined models and experimental data sets, selected calculation engine and minimization module, etc.

![](../assets/images/statusbar_lightmode.png#gh-light-mode-only)
![](../assets/images/statusbar_darkmode.png#gh-dark-mode-only)
