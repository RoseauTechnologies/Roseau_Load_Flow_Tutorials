# Modelling and Analysis of a Simple Unbalanced LV Network

## Introduction

This tutorial demonstrates how to model an unbalanced LV network with the _Roseau Load Flow_ solver. We use the simple
network from the tutorial of OpenDSS by [TeamNando](https://github.com/Team-Nando) called
`Tutorial-DERHostingCapacity-1-AdvancedTools_LV`. See
[here](https://github.com/Team-Nando/Tutorial-DERHostingCapacity-1-AdvancedTools_LV) for the original tutorial.

Before attempting this tutorial, you should have finished "Tutorial 1" in this repository for a basic knowledge of the
_Roseau Load Flow_ solver. We'll be using a modified form of the network in Tutorial 1. The network consists of an MV
bus, a MV/LV, $\Delta$-Y, transformer (11kV/0.4kV, 250 kVA) between the source bus and bus A, a 240 mm² 3-phase line
connecting buses A and B, and three 16 mm² single-phase lines connecting bus B with buses C, D and E each of which
serves as a connection point for a house.

The [original tutorial](https://github.com/Team-Nando/Tutorial-DERHostingCapacity-1-AdvancedTools_LV) uses OpenDSS to
model this LV network using an earth return system as shown in Figure 1.

!["Simple LV Network with Earth Return System"](../images/LV_Network_Without_Neutral.png)
**<div style="text-align: center;"> Figure 1. Simple LV Network with Earth Return System</div>**

The first tutorial allowed us to use _Roseau Load Flow_ to get the same results of the original OpenDSS tutorial by
modeling the network with earth-return without a neutral wire.

In the second tutorial, we add a neutral to the sale network as shown in Figure 2.

!["Simple LV Network with a Neutral"](../images/LV_Network_With_Neutral.png) **<div style="text-align: center;"> Figure
2\. Simple LV Network with a Neutral Wire</div>**

The following assumptions are made for the loads:

| Load Name | Phases | Connected bus | Peak Demand (kW) | PF   |
| :-------- | :----- | :------------ | :--------------- | :--- |
| Load_1    | 1      | C             | 7                | 0.95 |
| Load_2    | 1      | D             | 6                | 0.95 |
| Load_3    | 1      | E             | 8                | 0.95 |

Because this tutorial focuses on the _Roseau Load Flow_ solver, we only provide a brief overview of how to model the
above network in OpenDSS. For a detailed explanation of how to model this network in OpenDSS, we refer you to the
original tutorial by TeamNando [here](https://github.com/Team-Nando/Tutorial-DERHostingCapacity-1-AdvancedTools_LV).
