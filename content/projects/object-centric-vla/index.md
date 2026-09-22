---
title: "Object-Centric VLA for Few-Shot Adaptation"
date: 2026-08-01
summary: "Master's thesis on object-centric vision-language-action models for few-shot adaptation across robotic embodiments."
tags:
  - VLA
  - Embodied AI
  - Robot Learning
tech_stack:
  - Isaac Lab
  - GR00T
  - Python
status: "In Progress"
featured: true
---

## Overview

My Master's thesis investigates object-centric representations for vision-language-action models and their ability to adapt across different robotic embodiments.

**Supervisor:** [Prof. Dr.-Ing. Tamim Asfour](https://h2t.iar.kit.edu/tamim-asfour.php)

**Laboratory:** [High Performance Humanoid Technologies (H²T)](https://h2t.iar.kit.edu/), Institute for Anthropomatics and Robotics, Karlsruhe Institute of Technology

**Expected graduation:** March 2027

## Personal Contribution

I am independently responsible for the project. I built simulation environments for **three robot platforms** and implemented data preprocessing and format-conversion pipelines to support demonstration collection and robot policy training.

## Current Work

The current focus is integrating **Isaac Lab teleoperation** for demonstration collection and preparing the resulting data for **GR00T-based policy training with object-centric conditioning**.

The central research direction is to predict **object trajectories** as embodiment-independent representations of object motion. The goal is to investigate whether these representations can support few-shot policy adaptation and generalization across robots with different embodiments.

This work is in progress; no quantitative results are reported yet.

## Demonstration

<video controls playsinline preload="metadata" aria-label="FoundationPose 6D object pose tracking demonstration" style="display:block;width:100%;max-width:960px;margin:1.5rem auto;border-radius:0.75rem;box-shadow:0 10px 30px rgba(0,0,0,0.16);">
  <source src="demo.mp4" type="video/mp4">
  Your browser does not support embedded MP4 video.
</video>

The video shows FoundationPose pose estimates overlaid on an ARMar6 manipulation sequence at **1.5× playback speed**.

## Tools

**Isaac Lab · GR00T · Python · Robot Teleoperation · Dataset Preprocessing**
