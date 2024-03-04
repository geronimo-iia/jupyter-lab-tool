# Contributing

This project is based on [Geronimo-iaa's Python Module Template](https://github.com/geronimo-iia/python-module-template).
This is a cookiecutter template for a typical Python library following modern packaging conventions. 
It utilizes popular libraries to fully automate all development and deployment tasks.


## Setup

### Requirements

You will need:

* Python 3.9"+
* [Pyenv](https://github.com/pyenv/pyenv#installation)
* [poetry](https://python-poetry.org/)
* Make


### Make Installation

A powerfull tool:
* macOS: `$ xcode-select --install`
* Linux: [https://www.gnu.org/software/make](https://www.gnu.org/software/make)
* Windows: [https://mingw.org/download/installer](https://mingw.org/download/installer)

### Pyenv Installation

Pyenv will manage all our python version.
Follow [https://github.com/pyenv/pyenv#installation](https://github.com/pyenv/pyenv#installation)


### Python Installation

 `$ pyenv install 3.9`


### Poetry Installation: [https://poetry.eustace.io/docs/#installation](https://poetry.eustace.io/docs/#installation)

Poetry will manage our dependencies and create our virtual environment for us.



## Make Target list


| Name                    | Comment                                                                                         |
| ----------------------- | ----------------------------------------------------------------------------------------------- |
| make install            | Install project dependencies                                                                    |
| make configure          | Configure poetry                                                                                |
| make tag                | Create and push a tag based on current project version. This will launch github release action. |
| make next-patch-version | Increment patch version of the project.                                                         |
|                         |                                                                                                 |


## Poe Target list


| Name                    | Comment                                                                                  |
| ----------------------- | ---------------------------------------------------------------------------------------- |
| poetry poe clean        | Delete all generated and temporary files                                                 |
| poetry poe requirements | Generate requirements.txt                                                                |
|                         |                                                                                          |

You could retrieve those commands with `poetry poe`. 