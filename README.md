# Multi-rail-power-supply-board
A power supply board draft which takes AC mains and gives multiple standard DC outputs (1.5v,3.3v,5v,12v,24v,48v). The project presents design and simulation of Ac mains powered DC outputs intended to serve prototyping and industrial applications

The system converts 230 VAC mains into a 48 V isolated DC backbone, from which multiple regulated rails are generated using a structured buck + LDO power tree architecture.The design follows a hierarchical power architecture in which a single isolated high-voltage DC backbone is generated first, and all lower-voltage rails are derived from it using staged regulation.

The key features of the system include 

1)cascaded high-efficiency buck converters 

2)Low-noise LDO rails for sensitive loads 

3)LTspice simulations with startup and load analysis 

4)Modular and scalable power tree 

5)Documentation of design trade-offs and safety considerations

The circuit flow follows the the equence:
AC Mains (EMI Filter + Fuse + MetalOxideVariester) Isolated SMPS (48 V DC) DC-DC Buck Rails(48 → 24 → 12 → 5 → 3.3 → 1.5)
