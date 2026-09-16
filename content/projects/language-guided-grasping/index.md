---
title: "Vision- and Language-Guided Robotic Grasping"
date: 2026-05-01
summary: "Language-conditioned robotic grasping with VLM-based target selection, instance segmentation, 6D pose estimation, tracking, and grasp execution."
tags:
  - Robotic Perception
  - Manipulation
  - VLM
tech_stack:
  - ROS 2
  - MuJoCo
  - Grounded-SAM2
  - FoundationPose
  - MoveIt
  - Python
status: "Completed"
featured: true
---

## Overview

Developed an end-to-end robotic manipulation pipeline that converts natural-language or voice instructions into object grasping and semantic placement actions.

The perception pipeline combines a vision-language model for target identification, **Grounded-SAM2** for instance segmentation, and **FoundationPose** for 6D object pose estimation from RGB-D observations.

## Tracking and Re-Detection

Designed a follow-then-grasp strategy combining optical-flow and depth feedback with loss-triggered re-detection and mask refresh before pose estimation.

This increased tracking retention from **78.4% to 87.9%** and reduced the identity-switch rate from **16.7% to 6.7%** over 30 matched motion sequences per configuration.

## End-to-End Performance

Integrated stability-gated pose estimation, stale-pose rejection, grasp execution, and semantic sorting, achieving **86.7% end-to-end language-to-placement success**.

## Tools

**ROS 2 · MuJoCo · VLM · Grounded-SAM2 · FoundationPose · MoveIt · Python**
