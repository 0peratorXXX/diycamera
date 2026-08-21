# diyCamera

A small DIY digital camera project built around a Raspberry Pi and a few cheap components.

The idea was to make something simple enough to understand from the ground up rather than relying on a ready-made camera system.

## Features

* Basic image capture
* Manual exposure settings
* Simple preview mode
* Timestamped image files
* Local storage
* Command-line controls
* Optional LCD display

## Hardware

The original prototype was built using:

* Raspberry Pi Zero
* Raspberry Pi Camera Module
* 3.5" SPI display
* MicroSD card
* Two push buttons
* Small Li-ion battery
* 3D-printed enclosure

Nothing particularly complicated.

## Software

The software is written in Python and is split into a few small modules.

```text
diycamera/
├── camera.py
├── display.py
├── controls.py
├── config.py
├── capture.py
└── main.py
```

Python 3.10+ is recommended.

## Installation

Clone the repository:

```bash
git clone https://github.com/example/diycamera.git
cd diycamera
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Then run:

```bash
python main.py
```

## Configuration

Most settings can be changed in `config.py`.

The default configuration is intended for the original prototype, so some values may need changing depending on the hardware being used.

```python
IMAGE_WIDTH = 1920
IMAGE_HEIGHT = 1080
IMAGE_DIRECTORY = "./photos"
PREVIEW_ENABLED = True
```

## Notes

This project has been through a few different versions.

Some of the older code is probably not very useful anymore, but I've left it in the repository because it might be useful for comparison later.

The camera was never intended to be particularly good. The main goal was to understand how the individual parts worked and how they communicated with each other.

## Known issues

* Preview occasionally freezes
* Battery readings aren't particularly accurate
* Images sometimes take a moment to save
* The LCD driver is a little temperamental
* Some older configuration options no longer work

If something doesn't work, check the configuration before assuming the camera is broken.

## Project status

**Archived**

The hardware was eventually replaced with a newer version, so this repository probably won't receive many updates.

Still, it was a fun project to build.

## License

<a href="https://github.com/yourusername/next-stage">My License</a> 
