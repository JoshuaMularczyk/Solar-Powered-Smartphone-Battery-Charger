# Solar Smartphone Charger
This project applies skills of Power Electronics to create, deign, and construct a solar powered battery charger. My partner [Christian Williams](https://github.com/cwill713) and I were tasked by out professor [Dr. Rob Frohne](https://github.com/frohro) with coming up with a project for our Power Electronics class that incorporated what we were learning in the coursework. We decided to take what we were learning about step-down converters and design a charger for a smartphone in which the power source was a solar panel.

## Design Objectives:
- Output 5V from a higher input voltage
- Allow 1 amphere to be drawn into the smartphone
- Inexpensive to build ($20-$30 Budget)

## Overview
The power electronics project that [Christian Williams](https://github.com/cwill713) and I decided on was based around the specifications of new generation iPhone. We knew that Apple is picky with their products, so if we could get it to work with an iPhone it should, in theory, work with Android as well. I decided to use the [LM3478](https://www.ti.com/lit/ds/symlink/lm3478.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1654180125781&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm3478) High-Efficiency Low-Side N-Channel Controller for our Switching Regulator. This is the heart of our circuit and allows for a 2.97-40V input volage and a 1-A peak current capability. We used a 5W 12V Solar Panel to ensure that our smartphone would charge in average conditions.

## Rev 7 Design

<img width="814" alt="schematic2" src="https://user-images.githubusercontent.com/103919092/171946765-55e72f38-f459-4aac-95c0-715ab55abb05.PNG">

This is the most updated KiCad schematic for my circuit design. I used the Texas Instrument [Webench Power Designer](https://www.ti.com/design-resources/design-tools-simulation/webench-power-designer.html) to generate this step-down circuit. I specified a 5V minimum as well as a 12V maximum based on what would most likely be coming out of the solar panel. I also specified 1A for my maximum output current and 5V for my output voltage.

### Note on the voltages of the USB

<img width="231" alt="volatgefix2" src="https://user-images.githubusercontent.com/103919092/171946973-5ae8239b-4c4a-4da7-a379-1b64c578ddf0.PNG"><img width="638" alt="applereq" src="https://user-images.githubusercontent.com/103919092/171945713-fd5c0198-309d-4787-8156-a73bbe2ed5c6.PNG">

This was the added circuitry talked about in the testing section. For the pcb that we printed, we had to make this manually with throughhole resistors and soldered it to the underside of the board. *Note the Vbus pin needs 5V, the D- pin needs 2V, and the D+ pin needs 2.7V* This can be found in the following [documentation for iPhone](http://static.righto.com/files/charger-schematic.pdf) and [documentation for iPad](https://appleinsider.com/articles/12/09/25/apples_lightning_port_dynamically_assigns_pins_to_allow_for_reversible_use#:~:text=Some%20features%20of%20the%20Lightning,eight%20on%20the%20bottom%20row.).

## Rev 7 Simulation
I simulated our circuit in LTSpice

<img width="937" alt="sim" src="https://user-images.githubusercontent.com/103919092/171796889-ca19fa5c-3ef4-4bb1-9945-8d61918285da.PNG">

LTSpice has most of the components needed, but I had to 

### Voltage Outputs (5V 2.7V 2V)

<img width="960" alt="ThreeOutputVoltages" src="https://user-images.githubusercontent.com/103919092/171797195-8e6268f1-bec3-4a75-8258-a8a130c296d0.PNG">

### Input and Output Current

<img width="958" alt="currentsim" src="https://user-images.githubusercontent.com/103919092/171947246-d86cb5ba-57f3-49fe-8221-589e6aca34f5.PNG">


## Rev 7 PCB Design

<img width="730" alt="pcb2" src="https://user-images.githubusercontent.com/103919092/171952596-56a447e4-df71-455a-acbc-5d2364d089b8.PNG">


## Rev 6 Testing

## Rev 6 Results
