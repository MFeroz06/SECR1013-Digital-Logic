# Group Project : Elevator Controller System

## Group Members (False 9) :
1. Nasaaie bin Noriskamar
2. Muhammad Fairuz bin Herman
3. Muhammad Najmi Shahmi bin Mohd Latpi
4. Akmal Rafique bin Ahmad Raphaie

## Case Study
---
- To design an electronic controller for elevator / lift in a hotel building
---
## Scenario
---
- A hotel visitor will use the elevator to go up / down from one level to another
- The visitor will key in the desired level to go, tag the visitor room card, close the elevator door and push UP / DOWN button
- Then the elevator will go UP / DOWN by counting UP / DOWN one level to another until it reaches to desired level

  | Lift UP                     | Lift DOWN                     | 
  |-----------------------------|-------------------------------|
  | Key in level up             | Tag in card hotel             |
  | Tag in card hotel           | Tag in card hotel             |
  | Door Close                  | Door Close                    |
  | Lift goes up to destination | Lift goes down to destination |
  | Door Open                   | Door Open                     |
---
## Basic Design
---
-  4 floor elevator system– For level 0, 1, 2, and 3
– Use 2-bit up/down counter
  - 0 = count UP
  - 1 = count DOWN
– Function in synchronous mode
- Uses D flip flop
---
## Basic Design in DEEDS
---
- Flip-flop using D Flip-flop
- Comparator for current state and targeted level floor using XNOR and NAND
- Pattern detector for clock enabler using AND gate.
  – If output AND gate is HIGH, clock is enabled, and counter can run.
- Use push button instead of clock generator.
  - This is to eliminate undesirable state during states transition

## Our Job
- To enhance the previous design to 3-bit synchronous counter ( count UP/DOWN ) to support 8 floors hotel elevator.
- Thus, must show 4 inputs K-map, i.e., X, Q2, Q1, Q0 to design the counter circuit and related states / flip flop transition tables.
-  Use JK flip flop in your circuit design
-  Introduce these features to the input controller:
  - to detect visitor card hotel
  - to indicate door open / close
  - to use passcode


