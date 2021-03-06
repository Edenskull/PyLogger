<div align="center">
  <img src="https://raw.githubusercontent.com/Edenskull/KleenLogger/master/.github/_static/KleenLogger.jpg">
</div>

<div align="center">

[![GitHub license](https://img.shields.io/github/license/Edenskull/KleenLogger?color=blue&style=for-the-badge)](https://github.com/Edenskull/KleenLogger/blob/master/LICENSE)
![GitHub repo size](https://img.shields.io/github/repo-size/Edenskull/KleenLogger?color=green&style=for-the-badge)
![GitHub repo size](https://img.shields.io/badge/Python-3.6%20%7C%203.7-yellow?style=for-the-badge)

</div>

# Kleen-Logger
Simple python library that handle Logging of a script.

## Table of contents
* [Installation](#installation)
* [Documentation](#documentation)

## Installation

You can install the module via pip :  
`pip install kleenlogger`

or via wheel file [From PyPi](https://pypi.org/project/KleenLogger/#files) :  
```
pip install wheel
python -m wheel install wheel_file.whl
```

## Documentation

The aim of kleenlogger is to make it simple for the user to get script made logging.  
First import it to your script :
```PYTHON3
from kleenlogger import kleenlogger, KleenLogger
```

Then you can setup the logger format with the init_logger() function :
```PYTHON3
kleenlogger.init_logger(
    "AppName",
    KleenLogger.DEBUG,
    "[%(asctime)s][%(levelname)s] : [%(filename)s][%(funcName)s] : %(message)s",
    "%Y-%m-%d %H:%M:%S"
)
```

Now you can use the logger variable of kleentimer like a python logging : 
```PYTHON3
kleenlogger.logger.info("This is an info logging message")
kleenlogger.logger.error("Thiss is an error logging message")
```
