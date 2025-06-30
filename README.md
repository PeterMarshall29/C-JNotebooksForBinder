
[![Azure Pipelines](https://dev.azure.com/jupyter-xeus/jupyter-xeus/_apis/build/status/jupyter-xeus.xeus-cling?branchName=master)](https://dev.azure.com/jupyter-xeus/jupyter-xeus/_build/latest?definitionId=4&branchName=master)
[![Appveyor](https://ci.appveyor.com/api/projects/status/qn0wskxlvy52utuv?svg=true)](https://ci.appveyor.com/project/jupyter-xeus/xeus-cling)
[![Documentation Status](http://readthedocs.org/projects/xeus-cling/badge/?version=latest)](https://xeus-cling.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://img.shields.io/badge/launch-binder-brightgreen.svg)](https://mybinder.org/v2/gh/jupyter-xeus/xeus-cling/stable?filepath=notebooks/xcpp.ipynb)
[![Join the Gitter Chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/QuantStack/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

`xeus-cling` is a Jupyter kernel for C++ based on the C++ interpreter [cling](https://github.com/root-project/cling) and
the native implementation of the Jupyter protocol [xeus](https://github.com/jupyter-xeus/xeus).

## Documentation

To get started with using `xeus-cling`, check out the full documentation

http://xeus-cling.readthedocs.io/

## Usage

Launch the jupyter notebook with `jupyter notebook` and launch a new C++ notebook by selecting the **C++17** kernel in the *new* dropdown.

### Inline help and tab-completion

Quick help is shown on the pager with the special `?` magic.

![Help](help.png)

Content for the quick help is available for the standard library, and can be made available for third-party packages.

### Rendering of rich outputs

![Rich output](rich-output.png)

### Jupyter interactive widgets

A C++ backend for the Jupyter interactive widgets is available in the [`xwidgets`](https://github.com/jupyter-xeus/xwidgets/) package.

![Widgets](widgets.gif)

## Dependencies

``xeus-cling`` depends on

 - [xeus-zmq](https://github.com/jupyter-xeus/xeus-zmq)
 - [xtl](https://github.com/xtensor-stack/xtl)
 - [cling](https://github.com/root-project/cling)
 - [pugixml](https://github.com/zeux/pugixml)
 - [cpp-argparse](https://github.com/p-ranav/argparse)
 - [nlohmann_json](https://github.com/nlohmann/json)


| `xeus-cling` |   `xeus-zmq`    |      `xtl`      |     `cling`   |   `pugixml`   | `cppzmq` | `cpp-argparse`| `nlohmann_json` | `dirent` (windows only) |
|--------------|-----------------|-----------------|---------------|---------------|----------|---------------|-----------------|-------------------------|
|  main        |  >=1.1.0,<2.0.0 |  >=0.7.0,<0.8.0 | >=0.9,<0.10   | ~1.8.1        | ~4.3.0   |     ~3.0      | ~3.11.2         | >=2.3.2,<3              |
|  0.15.3      |  >=1.1.0,<2.0.0 |  >=0.7.0,<0.8.0 | >=0.9,<0.10   | ~1.8.1        | ~4.3.0   |     ~2.9      | >=3.6.1,<4.0    | >=2.3.2,<3              |
|  0.15.2      |  >=1.1.0,<2.0.0 |  >=0.7.0,<0.8.0 | >=0.9,<0.10   | ~1.8.1        | ~4.3.0   |     ~2.9      | >=3.6.1,<4.0    | >=2.3.2,<3              |
|  0.15.1      |  >=1.0.0,<2.0.0 |  >=0.7.0,<0.8.0 | >=0.9,<0.10   | ~1.8.1        | ~4.3.0   |     ~2.9      | >=3.6.1,<4.0    | >=2.3.2,<3              |
|  0.15.0      |  >=1.0.0,<2.0.0 |  >=0.7.0,<0.8.0 | >=0.9,<0.10   | ~1.8.1        | ~4.3.0   |     ~2.9      | >=3.6.1,<4.0    | >=2.3.2,<3              |



## License
XEUS-CLING use a shared copyright model that enables all contributors to maintain the copyright on their contributions.
This software is licensed under the BSD-3-Clause license. See the [LICENSE](LICENSE) file for details.
