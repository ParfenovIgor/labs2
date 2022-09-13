# Time Checker

## Author

Igor Parfenov
Contact: @Igor_Parfenov

## Overview

This is a local web application, which prints the current datetime in Moscow.

## Local Build

The application requires `Python-3.8+` , `pip` and `Python Virtual Environment` package.
Author build in `Debian-11`:

* `cd app_python`
* `python3 -m venv venv`
* `source venv/bin/activate`
* `python3 -m pip install -r requirements.txt`
* `python3 main.py`

## Local Usage

After these operations, the web application can be seen through address `127.0.0.1:8080`.

## Docker Build

* Install [Docker](https://docs.docker.com/). The instruction depends on your OS.
* `cd app_python`
* `sudo docker build .` Use `ID` mentioned in last line of output in next command.
* `sudo docker run <ID>`

## Docker Usage

After these operations, the web application can be seen though address, which is
written in output of `Flask` in terminal.

## Docker Hub Image

* `sudo docker run -p 80:8080 igorparfenov/devops_lab2:app_python`