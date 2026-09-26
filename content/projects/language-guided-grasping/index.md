---
title: "Language-Guided Pick-and-Place with Dynamic Target Tracking"
date: 2026-05-01
lastmod: 2026-09-26
summary: "Perception, tracking, and task integration for language-guided manipulation, achieving 86.7% (26/30) end-to-end language-to-placement success in a two-person project."
tags:
  - Robotic Perception
  - Manipulation
  - VLM
tech_stack:
  - ROS 2
  - MuJoCo
  - GroundingDINO
  - SAM2
  - FoundationPose
  - MoveIt
status: "Completed"
featured: true
---

## Overview

Built a pipeline that converts text or speech instructions into target selection, object tracking, and semantic placement on a **UR10e** setup.

**Course project:** AIR group, Institute for Material Handling and Logistics (IFL), KIT

**Period:** May – August 2026 · **Team:** 2

## Personal Contribution

I was responsible for **perception, dynamic target tracking, and the task pipeline**. I integrated language-conditioned target selection, segmentation, 6D pose estimation, semantic sorting, and RGB-D bin localization with **my teammate's grasp subsystem**.

## Demonstration

<video controls playsinline preload="metadata" aria-label="Vision- and language-guided robotic grasping demonstration" style="display:block;width:100%;max-width:960px;margin:1.5rem auto;border-radius:0.75rem;box-shadow:0 10px 30px rgba(0,0,0,0.16);">
  <source src="demo.mp4" type="video/mp4">
  Your browser does not support embedded MP4 video.
</video>

*Demonstration of the integrated language-guided pick-and-place system.*

## Language-to-Target Pipeline

Combined **Whisper**, YCB-validated VLM outputs, **GroundingDINO/SAM2** segmentation, and **FoundationPose** 6D pose estimation.

Target-selection accuracy was **93.3–100%** across English text, Chinese text, and Chinese speech, and **86.7%** for English speech, with **15 trials per condition**.

## Tracking and Pose Handover

Designed a tracking/position-based visual servoing (PBVS) state machine with **SAM2 re-detection after target loss** and **mask refresh in the stable state before pose estimation**.

| Metric | Before | After |
| --- | --- | --- |
| Tracking retention | 78.4% | **87.9%** |
| Pose-handover success | 73.3% | **93.3%** |
| Identity-switch rate | 16.7% | **6.7%** |

Evaluated over **30 matched motion sequences per configuration**.

## Diagnosing RGB-D Desynchronization

Traced approximately **0.9 m single-frame depth jumps** to RGB-D desynchronization. Tightened the RGB–depth pairing threshold from **1.0 s to 0.10 s** and added a latched **Lost** state to prevent inconsistent observations from driving the robot.

## End-to-End Evaluation

Integrated semantic sorting and RGB-D bin localization with the grasp subsystem, achieving **86.7% (26/30) language-to-placement success**. Each failure was attributed to its first blocking stage in the pipeline.

## Tools

**ROS 2 · MuJoCo · UR10e · MoveIt · Whisper · VLM · GroundingDINO · SAM2 · FoundationPose · Python**
