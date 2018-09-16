# Signal Simulator Coordinates Calculator

## Overview

This is a simple Coordinates Calculator for the Signal Simulator game.
Due to the fact that Coordinate Calculation is not that simple, and it would be pretty slow to do it on-hand, I made this little calculator web page.

## Tutorial

When you capture a signal and your coordinates system starts generating random coordinates, you should monitor (watch) the coordinates and record:

* The **lowest azimuth** you've seen
* The **highest azimuth** you've seen
* The **lowest elevation** you've seen
* The **highest elevation** you've seen

You should **keep watching** the monitor **until you reach a point** at which you **hardly get any** values - **lower** than your **lowest** or **higher** than your **highest**.

Input your recorded values as follows:
* **Lowest recorded azimuth** - Minimum Azimuth
* **Highest recorded azimuth** - Maximum Azimuth
* **Lowest recorded elevation** - Minimum Elevation
* **Highest recorded elevation** - Maximum Elevation

The coordinates will then be calculated by the following formulas:

* **{signal-azimuth} = (({max-generated-azimuth} - {min-generated-azimuth}) / 2) + {min-generated-azimuth}**
* **{signal-elevation} = (({max-generated-elevation} - {min-generated-elevation}) / 2) + {min-generated-elevation}**


If you've done **everything correctly** you should receive an output below with values which should be **completely accurate**.
There is a chance of a slight precision loss, but it should be somewhere in the range of 0.1-0.2.
