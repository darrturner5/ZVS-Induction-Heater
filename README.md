## Project Overview:

An Induction Heater is capable of heating and melting ferrous metals (Iron, Steel, etc). My Induction heater uses a ZVS Driver (Zero Voltage Switching) which is extremely efficient circuit which allow my IRLZ44N MOSFETS to switch high currents, causing minimal heating inside MOSFETS. The capacitor bank and work coil form the resonant circuit which allow for the classic heating of metals.

## System Architecture and Details
- Resonant at 78.7kHz
- Operating Voltage 8-10V
- 4uf 630V Metallized Polypropylene Capacitor Bank
- 1uH Work coil
- IRLZ44N MOSFETS
- 100uH 9A Sendust Core Toroid Inductors
- 12V Zener Diodes
- 400 Ohm Resistors
- IN4148 Switching diodes

![IMG_8076](https://github.com/user-attachments/assets/359aa7f7-909d-4ca2-874c-bb3f3ef62451)
![IMG_8162](https://github.com/user-attachments/assets/99b04a6a-1b4b-41a9-86e7-6fea46f35c58)


## Prototype:
![IMG_8068](https://github.com/user-attachments/assets/e8666c90-0ad0-453f-9f69-004d688ec5fa)
![IMG_8072](https://github.com/user-attachments/assets/b715d5a9-89ce-4895-95da-45b66f527150)
![IMG_8074](https://github.com/user-attachments/assets/a64c5788-e2aa-43f2-bfa0-d86fa07c4985)

## Work Coil Design Formulas
-  Wheelers Formula for Air Core Inductors
  <img width="176" height="55" alt="image" src="https://github.com/user-attachments/assets/6db39102-7615-4c9b-b643-c184b38d2eb5" />
  
  *Can be rearranged to find number of turns if you have a set inductance*
  ![IMG_8163](https://github.com/user-attachments/assets/4055de52-f478-40d5-ae83-edf8254e54e3)

  

- Resonant Frequency Formula
  <img width="135" height="56" alt="image" src="https://github.com/user-attachments/assets/8b3a7eba-a20a-4e10-aa3b-df35ab112dbb" />




## Results:
- Stable at 8V (10V pushes CC Mode of 5A)
- Heats small metals(Paperclips, Staples) to 278F+
- Capacitor heating (caused by High AC Ripple Current)
- Coil Heating
- Circuit hitting my Power Supply Current Limit
- Slightly Warm MOSFETS



![IMG_8085](https://github.com/user-attachments/assets/f69a0a92-0938-4d1c-be49-5642d6040851)
<img width="265" height="197" alt="image" src="https://github.com/user-attachments/assets/0ce54692-756a-467a-aa5b-919e04df8317" />


## What Id Improve:
- Several Capacitors in Parallel In the LC Tank (5 - 10 distributes the AC Current)
- Copper tubing coil with water cooling
- Smaller Value Capacitors for higher Resonant Frequency (Faster Heating)
- Better Power Supply 
- Increase Choke Inductor Value and Current Rating (Slower Inrush Current, better buffering and isolation)

