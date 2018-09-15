# Getting Started

Install [PlatformIO](https://docs.platformio.org/en/latest/installation.html#):

* install udev rule, add yourself to `dialup` group
* create a python2 virtualenv
* `pip install platformio`

On subsequent runs: `source ~/path/to/venv/bin/activate`.

# Platform IO cheatsheet

Also see [Quick Start](https://docs.platformio.org/en/latest/quickstart.html).

## Find / list supported boards

`platformio boards uno`

Also see [Embedded boards explorer](https://platformio.org/boards).

## Create a project

`platformio init --board ${boardid1} --board ${boardid2} ...`

e.g.

`platformio init --board uno`

