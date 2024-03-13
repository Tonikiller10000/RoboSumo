# RoboSumo

## Description:

This is a SUMO robot for comperitions. It pushes the opponent\`s robot out of the ring.
    
It uses:
- ATmega328p-AU as an microcontroller(used in arduino uno);
- 16 or 20Mhz crystal resonator;
- [TB6612FNG](https://github.com/Tonikiller10000/MotorDriver_1) DC motor driver;
- [VL53L0x](https://github.com/Tonikiller10000/VL53L0x_DistanceSensor) distance sensor;
- LI-PO battery (7.2V)
- 2x DC motors with low torque high speed gear box
- robot suport (Wood, 3d printed or any low weight matherial)

<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/p5.png" height = 450  ></td>
    <td><img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/p1.png" height = 450  ></td>
  </tr>
</table>

Schematic:
<img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/p3.png" >


### How it works:
The board is like a custom arduino UNO board powered from an 7.2V Li-Po battery trouth an 5V voltage regulator. 6 digital pins are used for the TB6612FNG motor driver witch is powered dirrectly from the battery to give more power to the motors. The reset pin has a 10K pullup resistor witch is pulled down by the reset button when it is pressed. The UART and ICSP pins wore pulled out to program the code and the bootloader of the IC.
For now I will try to use the VL53L0x I2C distance sensor, because [other sensors](https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/s1.png) are a little to slow.


### Programming:
Programming of the robot is done via UART protocoll with an [FTDI](https://github.com/Tonikiller10000/CH340G-FTDI-PROGRAMER) programming board. The code for the RoboSumo is not ready. 
 
### Design and mentions

This is The model I followed and some tips:
- to reach better torque on the wheels, it should be wider. 
- to mount the motors use molderd plastic motor holders, or be carefull when printing [it](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w1.jpg). 
- the case was made with autodesk fusion 360 at the 3d printer and with some M3 screws.

<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/r2.jpg"  height = 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/r1.jpg"  height = 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/RoboSumo/blob/main/PozeRoboSumo/r4.jpg"  height = 250 ></td>
  </tr>
</table>

The next version will have the motor driver soldered on the board and motors screwed dirrectly to it as the suport. Also I will try to make a smaller version


## Links: 
- ATmega328p-AU (microcontroller): 
- LM78L05 (5V voltage regulator):




