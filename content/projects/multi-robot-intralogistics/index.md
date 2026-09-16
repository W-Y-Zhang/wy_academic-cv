---
title: "Multi-Robot Intralogistics Automation"
date: 2024-12-01
summary: "ROS1/Gazebo multi-station intralogistics automation with coordinated robotic arms, conveyor handling, and suction-based pick-and-place."
tags:
  - Robotics
  - Automation
  - ROS
tech_stack:
  - ROS 1
  - Gazebo
  - Python
status: "Completed"
featured: true
---

## Overview

Developed a multi-station intralogistics automation system integrating **three 4-DoF robotic arms, a linear rail, and a conveyor belt**.

The system performed order-driven visual picking and downstream sorting through coordinated ROS nodes.

## Personal Contribution

I was responsible for integrating and controlling the three robotic arms, linear rail, conveyor belt, vision-based picking, suction grasping, and ROS-based coordination between workstations.

## Demonstration

<video controls playsinline preload="metadata" aria-label="Multi-robot intralogistics automation demonstration" style="display:block;width:100%;max-width:960px;margin:1.5rem auto;border-radius:0.75rem;box-shadow:0 10px 30px rgba(0,0,0,0.16);">
  <source src="demo.mp4" type="video/mp4">
  Your browser does not support embedded MP4 video.
</video>

## Validation

Implemented inter-station task coordination and validated suction-based pick-and-place operations both in **Gazebo simulation and on physical hardware**.

The system completed all recorded pick-and-place tests successfully. In the tested setup, a complete order required approximately **4.5 minutes**.

## Tools

**ROS 1 · Gazebo · Python**
