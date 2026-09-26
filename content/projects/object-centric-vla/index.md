---
title: "Cross-Embodiment Bimanual VLA Adaptation"
date: 2026-08-01
lastmod: 2026-09-26
summary: "Master’s thesis across ARMAR-6, ARMAR-7, and bimanual Franka: approximately 10 hours of ARMAR-6 demonstrations, a trained GR00T baseline, and object-centered task representations under investigation."
tags:
  - VLA
  - Embodied AI
  - Robot Learning
tech_stack:
  - Isaac Lab
  - GR00T
  - LeRobot
  - SAM3
  - FoundationPose
status: "In Progress"
featured: true
---

## Research Question

Can object-centered task representations improve the adaptation of bimanual vision-language-action (VLA) policies across robots with different embodiments?

My master's thesis, *Cross-Embodiment Bimanual VLA Adaptation with Object-centered Task Representations*, investigates this question across **ARMAR-6, ARMAR-7, and bimanual Franka**.

**Supervisor:** [Prof. Dr.-Ing. Tamim Asfour](https://h2t.iar.kit.edu/tamim-asfour.php)

**Advisor:** Dr.-Ing. David Schneider

**Laboratory:** [High Performance Humanoid Technologies (H²T)](https://h2t.iar.kit.edu/), KIT

**Period:** August 2026 – present · Expected graduation: March 2027

## Work Completed

- **Real-robot data:** Collected approximately **10 hours of ARMAR-6 demonstrations** through teleoperation and converted them to LeRobot format for policy fine-tuning.
- **Reference policy:** Trained a **GR00T N1.7 baseline on 80 ARMAR-6 demonstrations for 10,000 training steps**, without object-pose inputs.
- **Object trajectories:** Built an offline **SAM3 + FoundationPose** pipeline for YCB objects in calibrated real-robot RGB-D recordings. The extracted 6D object trajectories are intended for subsequent integration as object-centered task representations.
- **Simulation:** Built **three Isaac Lab environments**, one per embodiment, with pick-and-place, stacking, and pouring tasks, including domain randomization.
- **Evaluation design:** Defined a cross-embodiment protocol using task success rates, paired-bootstrap 95% confidence intervals, and human-annotated failure analysis.

## Baseline: Offline Action Prediction

| Setting | Current baseline |
| --- | --- |
| Policy | GR00T N1.7 |
| Robot | ARMAR-6 |
| Training data | 80 demonstrations |
| Training duration | 10,000 steps |
| Offline evaluation | Six training trajectories from a single task |
| Object-pose inputs | Not included |

The offline evaluation compares predicted actions with recorded demonstration actions on **trajectories seen during training**. Here, `h` is the action-chunk horizon: the policy executes `h` predicted steps before re-inference. These results are a fitting check for the baseline; held-out generalization, closed-loop task success, and the effect of object-centered representations remain to be evaluated.

| Action-chunk horizon (`h`) | Average unnormalized action MAE | Average unnormalized action MSE |
| ---: | ---: | ---: |
| 4 | **0.00495** | **0.000391** |
| 8 | 0.00586 | 0.000464 |
| 40 | 0.01187 | 0.001395 |

The table shows the expected trade-off in this training-trajectory check: longer open-loop execution between re-inference steps produces larger offline action error.

![GR00T N1.7 baseline: predicted and recorded actions on training trajectory 5](/wy_academic-cv/media/projects/gr00t-baseline-traj-5.jpeg)

*Representative training-trajectory check (`h=4`). The image shows predicted and recorded actions for one of the six training trajectories.*

## Object-Pose Demonstration

<video controls playsinline preload="metadata" aria-label="FoundationPose 6D object pose tracking demonstration" style="display:block;width:100%;max-width:960px;margin:1.5rem auto;border-radius:0.75rem;box-shadow:0 10px 30px rgba(0,0,0,0.16);">
  <source src="demo-v2.mp4" type="video/mp4">
  Your browser does not support embedded MP4 video.
</video>

*FoundationPose 6D object-pose tracking on recorded data. This illustrates the perception pipeline; object-pose inputs are not included in the baseline above.*

## Ongoing Work

Demonstration collection on **ARMAR-7 and bimanual Franka** is ongoing. The next stage is to integrate object trajectories into the policy and evaluate adaptation across embodiments against the reference policy.

## Tools

**Isaac Lab · GR00T · LeRobot · PyTorch · SAM3 · FoundationPose · Python · Teleoperation**
