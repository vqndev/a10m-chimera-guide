# A10M Chimera Conversion Guide

This guide will help you convert printer to use a chimera (2 in 2 out) style hotend. 

**I am not responsible if you screw something up or burn your house down.**

## Parts / Tools

  * Chimera (24V) w/ 2x Heater Cartridges and Thermistor
  * [Terminals Removal Key](https://www.amazon.com/gp/product/B07CHF74S9/) - I used this to remove wires from the molex connector
  * [MOLEX 43030-0001 CONTACT](https://www.amazon.com/gp/product/B00LQPGO8A) - I used this to connect wires to the molex connector
  
# Mount the Chimera
  * Print the [mount](https://www.thingiverse.com/thing:3488156): 
  * Remove the stock hotend
  * [Assemble the Chimera](https://e3d-online.dozuki.com/Guide/Chimera+Assembly/77?lang=en)
  * Install the mount on the carriage
  * I recommend [this](https://www.thingiverse.com/thing:2563670) fan duct 
  * [Level the nozzles](https://www.youtube.com/watch?v=7Bv5rPmiO0Q)
  * If you have all-metal heatbreaks, don't forget to [season your hotend](https://www.youtube.com/watch?v=shSfZxK-VUk)

## Wiring the Chimera
At this point. You have your Chimera mounted and none of the wires connected.
  * For the E0 (Left) heater and thermistor, use the same wires from the breakout board
  * For the E1 (Right) heater and thermistor, connect them to main board as shown in the picture below
    ![Wiring for E1](images/wiring-e1.jpg)

## Updating Firmware
  * Clone Marlin 1.1.8 to your computer 
  * Copy the files in this repository in the folder `Marlin` into the cloned Marlin 1.1.8 `Marlin` folder.
  * Make any changes you want to the configuration
  * Flash it

## Setting up the Chimera
  * Octoprint
  * PID Autotune
  * [X Offset](https://www.youtube.com/watch?v=aQbqc2br5yo)
