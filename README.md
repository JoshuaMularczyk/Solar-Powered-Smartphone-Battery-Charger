# Solar Smartphone Charger
This project applies skills of Power Electronics to create, deign, and construct a solar powered battery charger. My partner [Christian Williams](https://github.com/cwill713) and I were tasked by out professor [Dr. Rob Frohne](https://github.com/frohro) with coming up with a project for our Power Electronics class that incorporated what we were learning in the coursework. We decided to take what we were learning about step-down converters and design a charger for a smartphone in which the power source was a solar panel.

## Design Objectives:
- Output 5V from a higher input voltage
- Allow 1 amphere to be drawn into the smartphone
- Inexpensive to build ($20-$30 Budget)

## Overview
The power electronics project that [Christian Williams](https://github.com/cwill713) and I decided on was based around the specifications of new generation iPhone. We knew that Apple is picky with their products, so if we could get it to work with an iPhone it should, in theory, work with Android as well. I decided to use the [LM3478](https://www.ti.com/lit/ds/symlink/lm3478.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1654180125781&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm3478) High-Efficiency Low-Side N-Channel Controller for our Switching Regulator. This is the heart of our circuit and allows for a 2.97-40V input volage and a 1-A peak current capability. We used a 5W 12V Solar Panel to ensure that our smartphone would charge in average conditions.

## Rev 7 Design
<img width="805" alt="schematic" src="https://user-images.githubusercontent.com/103919092/171796808-3db44315-7d83-4c79-971b-e4f8263e1bfc.PNG">

### Note on the voltages of the USB 
<img width="112" alt="voltagefix" src="https://user-images.githubusercontent.com/103919092/171797049-e7c6030b-2a28-40b2-b763-526aaf06bf85.PNG">


## Simulation
<img width="937" alt="sim" src="https://user-images.githubusercontent.com/103919092/171796889-ca19fa5c-3ef4-4bb1-9945-8d61918285da.PNG">

### Voltage Outputs (5V 2.7V 2V)
<img width="960" alt="ThreeOutputVoltages" src="https://user-images.githubusercontent.com/103919092/171797195-8e6268f1-bec3-4a75-8258-a8a130c296d0.PNG">

### Input and Output Current

## PCB Design
<img width="660" alt="pcb" src="https://user-images.githubusercontent.com/103919092/171798682-d67deb13-11dc-40d1-a506-84b779b9a644.PNG">

## Testing

## Results
