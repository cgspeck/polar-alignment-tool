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

Rerun init to add more boards

## Build / Clean / Upload

```
platformio run
platformio run -t clean
platformio run -t upload
```

## Find a library (indexed/community)

```
platformio lib search lsm9ds1 --framework=arduino
...
platformio lib install 1825
```

Then manually add it to `platformio.ini` under `[common_env_data]` (until
[this issue](https://github.com/platformio/platformio-core/issues/1028) is resolved).

