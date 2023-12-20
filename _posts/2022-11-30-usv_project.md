---
title: Bathymetric Unmanned Surface Vehicle
date: 2023-03-10 12:00:00 -500
categories: [projects]
tags: [projects, autonomous vehicle, bathymetric, qt]
---

Project: *Bathymetric Unmanned Surface Vehicle*  
Team members: *Nguyen Xuan Dung, Van Dinh Hoang, Cao Thi Quynh Tram, Vo Trung Kien and Tran Van Hoai*  
Supervised by: *Dr. Ha Manh Tuan, Hanoi University of Science and Technology*

This is a recap for the *Bathymetric Unmanned Surface Vehicle* project including our progress, what we have learned and some thoughts.

## Objectives  
The initial idea was to build an Unmanned Surface Vehicle (USV) (or simply autonomous boat), and figure out what applications it can be used for. After some market surveys, some simulation with the controller, field tests with the prototypes and taking our budget into account, we decided that we want to build a Bathymetric USV that
+ Autonomously plans and tracks pathways
+ Continously collects depth data points on its way
+ Comes with an interactive Ground Control Station (GCS) GUI
+ Transmits depth data, coordinates, attitudes and camera stream to the GCS
+ Recieves commands from the GCS (and responds with acceptable latency)
+ Recontruct a 3D mesh of the scanned terrains
+ Is built from scratch (no Pixhawk, ArduPilot, or any commercial auto-pilot controller)  

## Controll modes and pathway planning
Our approach to pathway planning is quite straight-forward and simple. 
Our GCS GUI offers 3 basic controll mode:
1. "Manual Mode": The user directly controlls the throttle and yawing moment.
2. "Single Point Mode": The user selects a single coordinates, that the USV navigate to   
3. "Bathymetric Scan Mode":  The user selects 4 coordinates specifying a polygonal area, in which the USV moves in a zigzag-ish grid pattern (with the user-defined spacing distance).

## Pathway tracking
The pathway tracking method derived from 




