# Mini 2D Plotter

A mini 2D plotter project that converts images into G-code using Python, Flask, ImageMagick, Potrace and vpype.

## Project Overview

The project currently provides a web interface where users can upload an image and convert it into G-code for a 2D plotter.

### How It Works

1. Upload an image through the Flask web interface.
2. ImageMagick processes the image.
3. Potrace converts the bitmap into an SVG vector.
4. vpype processes the SVG and generates G-code.

## Installation & Required Tools

### 1. Python
- **Required version:** Python 3.13.17
- [Download Python 3.13.17](https://www.python.org/downloads/release/python-31317/)

### 2. ImageMagick
- [Download ImageMagick](https://imagemagick.org/download/#gsc.tab=0)

### 3. vpype-gcode
- Used to generate G-code from SVG files.
- [GitHub repository](https://github.com/plottertools/vpype-gcode)

### 4. Potrace
- Used to convert bitmap images into SVG vector graphics.
- [Download Potrace](https://sourceforge.net/projects/potrace/)

### 5. GRBL
- Firmware resource for 28BYJ-48 stepper motors.
- [GRBL-28byj-48 GitHub repository](https://github.com/TGit-Tech/GRBL-28byj-48/tree/master/grbl)

## Hardware (Planned)

- ESP32-C3
- 2 × 28BYJ-48 stepper motors
- 2 × ULN2003 driver boards
- 1 × servo motor

## Project Progress

- [x] Image upload interface
- [x] Image-to-SVG conversion
- [x] SVG-to-G-code conversion
- [ ] ESP32-C3 firmware
- [ ] Stepper motor control
- [ ] Pen lift servo control
- [ ] USB serial communication
- [ ] Wi-Fi control

## Project Status

The image-to-G-code conversion pipeline is working. Hardware integration and plotter movement control are planned for future development.
