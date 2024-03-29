This repository contains user documentation for the [EasyDiffraction application](https://github.com/easyscience/easyDiffractionApp).

## CI build status

* Develop branch  
  [![w3c-develop][90]][95] [![url-develop][70]][75]
* Master branch  
  [![w3c-master][80]][85] [![url-master][60]][65]

## Build locally

* Create virtual environment and activate it (*optional*)
```
python -m venv .venv
source .venv/bin/activate
```
* Upgrade pip (*optional*)
```
pip install --upgrade pip
```
* Install [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/getting-started/) documentation framework (*if not done already*)
```
pip install mkdocs-material
```
* Generate documentation from the files in _docs/_ and places it in _site/_
```
mkdocs build
```

      
<!---URLs--->

[60]: https://img.shields.io/badge/url--master-docs.easydiffraction.org/app-blue
[65]: https://docs.easydiffraction.org/app
[70]: https://img.shields.io/badge/url--develop-easyscience.github.io%2FEasyDiffractionAppDocs-blue
[75]: https://easyscience.github.io/EasyDiffractionAppDocs

<!---W3C validation--->

[80]: https://img.shields.io/w3c-validation/default?label=w3c-master&targetUrl=https://docs.easydiffraction.org/app
[85]: https://validator.w3.org/nu/?doc=https%3A%2F%2Fdocs.easydiffraction.org/app%2F
[90]: https://img.shields.io/w3c-validation/default?label=w3c-develop&targetUrl=https://easyscience.github.io/EasyDiffractionAppDocs
[95]: https://validator.w3.org/nu/?doc=https%3A%2F%2Feasyscience.github.io%2FEasyDiffractionAppDocs%2F
