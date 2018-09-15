# Polar Alignment Tool

## Objectives

* rugged enclosed stand-alone project
* display showing heading (magnetic & true), x-rotation
* nice to have a led indicate when N/S aligned, and when Altitude Align
* allow magnetic error to be set in the field

## Hardware

* Serial Enabled 16x2 LCD - Red on Black 5V
  * $37.97 https://core-electronics.com.au/serial-enabled-16x2-lcd-red-on-black-5v.html
  * serial interface, rx only, can up/down contrast
* SparkFun 9DoF Sensor Stick
  * i2c or spi
  * $16.63 https://core-electronics.com.au/sparkfun-9dof-sensor-stick.html
* 3 x buttons (OK, UP, DOWN)
* 3 x red indicator leds (power, N/S align, Altitude Align)
* Minimum Arduino to support this

## Menu Structure / Display

### Default

  0123456789012345
1 169.0*T  180.0*M
2 alt + 38.6*

* Pressing Up / Down on this screen will alter brightness
* Pressing Ok on this screen will bring up the menu

### Menu structure (on ok press)

* Set Mag. dec.
  * (display current value, set with up/down, save with OK)
* Set Altitude
  * (display current value, set with up/down, save with OK)
* Back

## Requirements for Ardunio

* 5V
* 3-4 interrupts
* Spi
* serial out

