# SERT Vision

[![Team 2521][team-img]][team-url]
[![Python 2.7][python-img]][python-url]
[![License][license-img]][license-url]
[![Travis][travis-img]][travis-url]

SERT's OpenCV vision code.

## Usage

Before starting the program, you must install OpenCV v2.4.x along with the
pip dependencies:

```bash
$ pip install -r requirements.txt
```

Then, you can run the program using:

```bash
$ python run.py
```

Full usage:

```text
usage: run.py [-h] [-i IMAGE] [-d] [-ip ROBORIO_IP] [-ma MIN_AREA]
              [-lt LOWER_COLOR [LOWER_COLOR ...]]
              [-ut UPPER_COLOR [UPPER_COLOR ...]] [-v]
```

## Configuration

All command-line arguments may be configured in the `config.ini` file
(located at `config/config.ini`). For example, the `--lower-rgb`
argument may be edited using the `lower-rgb` line in the `config.ini`.

```text
-h, --help            show this help message and exit
-i IMAGE, --image IMAGE
					  path to image
-d, --display         display results of processing in a new window
-ip ROBORIO_IP, --roborio-ip ROBORIO_IP
					  the ip address of the roboRIO
-ma MIN_AREA, --min-area MIN_AREA
					  minimum area for blobs
-lt LOWER_COLOR [LOWER_COLOR ...], --lower-color LOWER_COLOR [LOWER_COLOR ...]
					  lower color threshold for BGR values
-ut UPPER_COLOR [UPPER_COLOR ...], --upper-color UPPER_COLOR [UPPER_COLOR ...]
					  upper color threshold for BGR values
-v, --verbose         for debugging, prints useful values
```

<!-- Badge URLs -->

[team-img]:     https://img.shields.io/badge/team-2521-7d26cd.svg?style=flat-square
[team-url]:     https://sert2521.org
[python-img]:   https://img.shields.io/badge/python-2.7-blue.svg?style=flat-square
[python-url]:   https://www.python.org/downloads
[license-img]:  https://img.shields.io/github/license/andrewda/robotics-vision.svg?style=flat-square
[license-url]:  https://github.com/andrewda/robotics-vision/blob/master/LICENSE
[travis-img]:   https://img.shields.io/travis/andrewda/robotics-vision.svg?style=flat-square
[travis-url]:   https://travis-ci.org/andrewda/robotics-vision
