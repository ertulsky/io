---
layout: post
title:  "2-Link Robot Manipulator"
date:   2025-07-8T14:25:52-05:00
author: Evan Tulsky
categories: Projects
tags: Robotics
permalink: /posts/robotarm/
---

## Joystick Control

Open-loop direct control to help prototyping. A simple analog joystick lets you drive the robot arm manually — perfect for calibration, testing, or just having fun.

- **X-Axis**: Controls the base joint (shoulder)
- **Y-Axis**: Controls the elbow joint
- **Platform**: Arduino or Raspberry Pi reads analog signals and sends angles to the motors

The joystick input is mapped to joint angles in real-time:

```python
theta1 = map(joystick.x, 0, 1023, -pi/2, pi/2)
theta2 = map(joystick.y, 0, 1023, -pi/2, pi/2)
set_joint_angles(theta1, theta2)

## Computer Vision
Work in progress

## Obstacle Avoidance with Sensors
Safety is non-negotiable when working with physical systems. This arm is equipped with two sensors for obstacle detection and thermal awareness:

- Ultrasonic Sensor

--Measures distance to nearby objects or humans.
--Mounted near the end-effector.
--Stops motion if something is too close.

if distance < 15:
    halt_motion()

- Temperature Sensor (IR)
--Scans the scene for hot objects (e.g. cookware, electronics).
--Flags objects over a temperature threshold (e.g., 50°C) as unsafe to touch.
