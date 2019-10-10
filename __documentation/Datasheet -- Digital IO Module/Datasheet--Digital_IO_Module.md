## Digital IO Module Datasheet
### CE-MD-001-0001

<p style="text-align:center;" ><img src="_media/VEN_Parts_CE-MD-001-0001_01.png" width="75%" height="75%"></p>

### Contents
[TOC]

### Overview
The Digital IO Module extends the functionality of the MachineMotion controller with 4 industrial 24V inputs and 4 industrial 24V outputs. It is a plug-&-play module that only requires a single connection to MachineMotion controller. It comes ready to use with its associated 5 meters M12 cable.

#### Features
- Configuration Free, Plug-&-Play
- Digital Communication with the MachineMotion Controller
- 4 x 24V Input Ports
- 4 x 24V Output Ports

### Technical Specifications

#### Input Ports
| Name                          | Specification                 | Units
|---                            |---                            |---    |
| Electrical Interface          | 10kohm pull-up resistor       | NA    |
| Voltage Range                 | 0 - 24                        | V     |
| Transition Voltage            | 9.025                         | V     |

#### Output Ports
| Name                          | Specification                 | Units
|---                            |---                            |---    |
| Electrical Interface          | Push-Pull Transistors         | NA    |
| High Voltage Range            | 23 - 24                       | V     |
| Low Voltage Range             | 0 - 1                         | V     |
| Sourcing Current Range        | 0 - 75                        | mA    |
| Sinking Current Range         | 0 - 100                       | mA    |

#### Pinout
The Digital IO Module contains 4 inputs and 4 outputs, each of which is grouped with a 24V and 0V supply connection for convenient wiring to external devices. The Digital IO Module is also equipped with 8 LED's to visualize the input and output signals. The LED's are located on the sides of the enclosure.

##### Input / Output
<p style="text-align:center;" ><img src="_media/digital_io_module_pinout_hq.png" width="60%" height="60%"></p>
<p style="text-align: center;"><span style="color: #808080; font-size: 11pt;"><em>Figure 2: Digital IO Module Pinout.</em></p>


##### Input LED's
| Signal Type   | State         | LED   |
|---            |---            |---    |
| Input         | High          |ON     |
| Input         | Low           |OFF    |
| Input         | Floating      |ON     |

##### Output LED's
| Signal Type   | State         | LED   |
|---            |---            |---    |
| Output        | High          |ON     |
| Output        | Low           |OFF    |
| Output        | Floating      |OFF    |

##### M12 Connector Pinout
| Pin Number    |Description        |
|---            |---                |
| 1             | 24V               |
| 2             | 0V                |
| 3             | RS485 A           |
| 4             | RS485 B           |
| 5             | Not Used          |
| 6             | Not Used          |
| 7             | Not Used          |
| 8             | shield / Earth    |


### Applications
The Digital IO Module can be used to interface with external systems and devices that utilize 24V digital input/output control. Among others, the devices listed below are typical use cases.

- Programmable Logic Controllers (PLC's)
- Digital Process Sensors
- Relays
- Robot Controllers
- Pneumatic Actuators
- Push-Buttons
- Lights and Indicators

### Connection to the MachineMotion Controller

The Digital IO Module can be connected to the MachineMotion controller via any one of the AUX ports (AUX1, AUX2, AUX3). See *Figure 3*.

<p style="text-align:center;" ><img src="_media/machine_motion_aux_connectors.png" width="60%" height="60%"></p>
<p style="text-align: center;"><span style="color: #808080; font-size: 11pt;"><em>Figure 3: AUX Ports on the MachineMotion Controller.</em></p>

Upon connection, the module will automatically be detected and become available for use. A maximum of three Digital IO Module can be connected to a MachineMotion controller.

### Control
The Digital IO Module has a fixed factory address. It is indicated on the back of the enclosure on its product information sticker. The correct address needs to be used when communication with the module.

#### Vention ControlCenter

The Digital IO module can be utilized via the Vention ControlCenter interface. The jogger App allows control of its outputs and visualization on its input states.

You can access it via your Chrome browser via the ControlCenter [Jogger](http://192.168.7.2/_pendant/jogger.html). Make sure that you are connected to your MachineMotion controller via the 192.168.7.2 port (formerly labelled DEFAULT ETHERNET). Click on the lower left icon (see *Figure 4*) to access the Digital IO Module control interface (*Figure 4*).

<p style="text-align:center;" ><img src="_media/control_center_io_control_edited.png" width="60%" height="60%"  <img style="border:1px solid grey;"> </p>

<p style="text-align: center;"><span style="color: #808080; font-size: 11pt;"><em>Figure 4: Accessing the Digital IO Module Control Interface.</em></p>

<p style="text-align:center;" ><img src="_media/" width="60%" height="60%"  <img style="border:1px solid grey;"> </p>

<p style="text-align: center;"><span style="color: #808080; font-size: 11pt;"><em>Figure 5: Digital IO Module Control Interface.</em></p>


The MachineLogic environment in ControlCenter also allows for control of the Digital IO Module.


#### MachineLogic
The [MachineLogic]() programming interface also allows for the Digital IO Module.

#### Python Programs
Refer to the latest [Python API](https://github.com/VentionCo/mm-python-api) for further details on how to control the Digital IO Module with Python programs.

### Notes
- Missing Figure 5
- Needs proof Reading