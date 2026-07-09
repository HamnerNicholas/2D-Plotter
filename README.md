# STM32 2D Plotter Final Project

This repo is our final project for a small 2D plotter built around an STM32 board, stepper drivers, an Ender 3 frame, limit switches, an I2C LCD, a rotary encoder, and a set of hardcoded drawing functions.

Group Members: Tajinderpal Gill, Nicholas Hamner, Dominique Kisantear, Louie Manlangit
Lab Instructor: Sean Kennedy

## Hardware summary

- STM32F303K8 based controller
- Stepper drivers for X, Y, and Z
- Ender 3 frame used as the plotter base
- Limit switches for homing
- I2C LCD for the menu
- Rotary encoder and push button for input
- Pen lift on the Y axis
  
## Hardware summary

- STM32F303K8 based controller
- Stepper drivers for X, Y, and Z
- Ender 3 frame used as the plotter base
- Limit switches for homing
- I2C LCD for the menu
- Rotary encoder and push button for input
- Pen lift on the Y axis

## Firmware notes

The GitHub version only keeps the final firmware source files. We are not using the full CubeIDE project here because the `.ioc` gets rewritten and is not the version we want to submit.

The firmware behavior was not changed:

- pin mappings stay the same
- stepper movement logic stays the same
- LCD menu flow stays the same
- encoder behavior stays the same
- homing and centering behavior stay the same

## Python helper tools

Image conversion:

```bash
cd image_to_draw_vectors
python src/draw_image.py input/image.png
```

Math function conversion:

```bash
cd function_to_draw_vectors
python src/draw_math.py "sin(x)" --xmin -3.14159 --xmax 3.14159 --samples 200 --width-mm 40 --height-mm 40
```

