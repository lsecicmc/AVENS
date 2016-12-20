# AVENS

**AVENS** (**A**erial **VE**hicle **N**etwork **S**imulator) is part of a research project that aims to provide a simulation test bed for virtual experiments of network coverage and connectivity among Unmaned Aerial Vehicles (UAVs) flying in cooperation or sharing the same airspace. This is achieved by integrating LARISSA, X-Plane Flight Simulator and OMNeT++ Network Simulator.

In this demonstration, two software projects are available. PluginXPlane.zip contains a Visual Studio 2012 project used to build a X-Plane plugin that both controls extra planes and send position information to an XML file. OMNETProject is a OMNeT++ 4.6 project that reads position information in XML file and uptades the planes position in network simulation. ArbitraryMobility.zip is an extension of INET framework used to place the nodes in arbitrary positions that do not follow any INET available mobility models. Its files must be inserted at *inet/src/inet/mobility/single* INET path. For the communication to work, the file path must be set correctly on both projects (XML_FILENAME directive at file PluginXPlaneOMNET.cpp in X-Plane project and FANET.handler.filename parameter in OMNeT++ project).

Both projects were built and used in Windows 8 OS. For help, please contact rodrigues.mariana@usp.br
