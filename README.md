# SSN project: BlueBorne Impact Analysis
## Introduction

In this repository you will find all relevant files for a research project into BlueBorne Impact Analysis, done by Kees de Jong, Adrien Raulot, Shahrukh Zaidi and Kotaiba Alachkar in October 2017, for [Security of Systems and Networks](https://www.os3.nl/2017-2018/courses/ssn/start) course.

## Features

- MAC lookup (both online and offline via the EUI info in the csv Python module).
- Merge and process data from multiple csv files (with a MAC address column and a column with the BlueBorne vulnerability state, the file name of the csv should be the date of the scan).
- Output vulnerability state either numeral or in string format, for easier parsing.

## Examples

```
./mac_lookup.py -s 10-01-2017.csv -s 10-02-2017.csv -d /tmp/final.csv -n
```
## Usage

```
usage: mac_lookup.py [-h] -s SRC -d DST [-n]

Mac address details -> csv

optional arguments:
  -h, --help         show this help message and exit
  -s SRC, --src SRC  Provide source csv
  -d DST, --dst DST  Provide destination csv
  -n, --num          Insert numeral values instead of strings
  ```
