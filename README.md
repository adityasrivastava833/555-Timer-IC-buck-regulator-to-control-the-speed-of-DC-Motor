# 555-Timer-IC-buck-regulator-to-control-the-speed-of-DC-Motor

Components Required – 
555 Timer IC *1
8 pin IC base *1
Resistor 1KΩ *1
47 KΩ Potentiometer *1
10 µFarad Capacitor *1
470 µFarad Capacitor *1
PN Diode (1N4007) *3
N Channel MOSFET (IRFZ44N) *1
PCB Board (40*30 pins soldering) *1 
Power Supply (9V Battery with Battery Connector) *1 
DC Motor (5V) *1 
PBT Connector *1

A 555 Timer IC 
It is similar to an oscillator like monostable, which has only one stable state. It gets back to its 
original state when an external clock pulse is given to a monostable oscillator. Similarly, when 
555 timer generates an oscillating wave at output pin 3 it enters a stable state, in order to get back 
to its normal an external trigger is applied. The most important property of 555 Timer IC that we have used in our project is the duty cycle of the timer is adjustable. 
Buck Converter 
The buck converters employ PWM switching technique to step down the voltage. Since, a buck 
converter utilizes PWM signal to maintain the voltage, theoretically it is a 100% efficient system, 
but in real life these buck converters can be 90 - 95% efficient. 
Working Of the Model Buck Converter using 555 Timer 
In order to make the system work in real world application, we need to switch on and off the switch 
a lot faster than a human can perform. Therefore, we use a PWM pulse generator and a transistor 
as a switch to perform the task. A 555 timer IC in Astable mode can be used to generate the PWM 
output for our operation. The IC 555 generates around 30 KHz frequency with the help of passive 
and active components connected to it. 
Formula to Calculate PWM Frequency and Duty cycle on 555 Timer 
For designing the circuit, we used the IC 555 timer in Astable mode. Here, the output pulse is 
continuously switched between high and low states. To change the frequency of the oscillation, 
we can change the values of Resistor and capacitor (RC) network, connected with the 555 timer. 
The above values for our circuit was selected using the formula written below: 
ON time (sec) = 0.693 * (R1 + R2) * C 
OFF time (sec) = 0.693 * R2 * C 
Frequency = 1.44 / ((R1 + R2 + R2) * C) 
Duty cycle D = PW/T, 
Here, 
D is the duty cycle, PW is the pulse width (pulse active time), and T is the total period of the 
signal, all the values of resistors are in Ohm and values of capacitors are in Farads. 
<img width="169" alt="image" src="https://github.com/adityasrivastava833/555-Timer-IC-buck-regulator-to-control-the-speed-of-DC-Motor/assets/99532357/8798d8ae-78fe-4c5b-82df-ea2f63e60d96">

Circuit Diagram
<img width="323" alt="circuitdiagram" src="https://github.com/adityasrivastava833/555-Timer-IC-buck-regulator-to-control-the-speed-of-DC-Motor/assets/99532357/99ab70bf-8f73-40e4-98b8-a89cb2001580">


Result
The speed of DC motor is controlled using PWM technique. 
A 555 IC based converter is one of the simplest, yet efficient method to keep the complexity as 
well as the cost of your project low while achieving a high efficiency and improving lifespan of 
your components. This easy power electronics circuit can step down a DC voltage with 
efficiency as high as 95% compared to 40-60% efficiency of a linear voltage regulators. This 
driving technique is also useful for the speed control of a motor and dimming LEDs without 
effecting its lifespan, making it a very versatile voltage control option for electronics project.
