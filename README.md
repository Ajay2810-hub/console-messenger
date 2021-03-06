# console-messenger

[![Downloads](https://static.pepy.tech/personalized-badge/console-messenger?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/console-messenger)
[![Downloads/Week](https://static.pepy.tech/personalized-badge/console-messenger?period=week&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week)](https://pepy.tech/project/console-messenger)
[![Downloads/Month](https://static.pepy.tech/personalized-badge/console-messenger?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/Month)](https://pepy.tech/project/console-messenger)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Latest PyPI version](https://img.shields.io/pypi/v/console-messenger.svg)](https://pypi.org/project/console-messenger)
[![Supported Python versions](https://img.shields.io/pypi/pyversions/console-messenger.svg)](https://pypi.org/project/console-messenger)
[![Documentation Status](https://readthedocs.org/projects/console-messenger/badge/?version=main)](https://console-messenger.readthedocs.io/en/main/?badge=main)

## About
This package displays success, warning and info messages and errors on console with different colours using [rich](https://pypi.org/project/rich/) module. It also prints any error type without passing it as a parameter.

## Requirements
```shell
 python>=3.0
```

## Dependencies
```shell
 rich>=9.0.0
```

## Installation
```shell
 pip install console-messenger
```

## Usage
```python
 >>> from ConsoleMessenger import ConsoleMessage
 >>> console = ConsoleMessage()
```

**Print an error**
```python
 try:
     a = 5/0
 except Exception as e:
     console.danger(e)
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img.png)

**Display a custom error**
```python
 console.danger("this is a custom error", err_type="My Error")
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img1.png)

**Print a success message**
```python
 console.success("Success", "success method worked!")
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img2.png)

**Display a warning**
```python
 console.warning("Warning", "You are using pip version 20.2.4; however, version 20.3 is available.")
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img3.png)

**Display a info message**
```python
 console.info("INFO", "Hello User!")
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img4.png)

**Display a dark message**
```python
 console.dark("Dark", "This is a dark message!")
```

Output :-

![Broken Image](https://raw.githubusercontent.com/Ajay2810-hub/console-messenger/main/images/img5.png)
