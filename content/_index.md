---
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: About Me
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: portfolio
    id: projects
    content:
      title: Selected Projects
      subtitle: Robotics, perception, and embodied AI projects
      count: 3
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
      default_button_index: 0
      archive:
        enable: false
    design:
      columns: 3
      fallback_icon: academic-cap
      status_badge:
        enable: true

  - block: features
    content:
      title: Research Experience
      subtitle: Research Assistant · Institute for Material Handling and Logistics (IFL), Karlsruhe Institute of Technology · Karlsruhe, Germany · Jun. 2025 – May 2026
      items:
        - name: Panoptic Segmentation for Robotic Perception
          description: Upgraded CUDA/PyTorch environments and adapted multiple panoptic-segmentation baselines to the ARIBIC dataset in a reproducible Docker pipeline. Benchmarked models and improved panoptic quality (PQ) by up to 20% through hyperparameter tuning and evaluation.
          icon: hero/squares-2x2
        - name: Dual-LiDAR AGV Localization and Mapping
          description: Developed synchronized front/rear LiDAR fusion with coordinate transforms and 360° scan resampling. Adapted a FastSLAM pipeline and built a GMapping + AMCL workflow to compare localization trajectories on the same real-world AGV dataset.
          icon: hero/map
    design:
      columns: '2'

  - block: features
    content:
      title: Technical Skills
      items:
        - name: Programming
          description: Python
          icon: hero/code-bracket
        - name: Robotics
          description: ROS 1/2 · Gazebo · MuJoCo · MoveIt · Isaac Lab
          icon: hero/cog-6-tooth
        - name: Perception & ML
          description: PyTorch · OpenCV · SAM2 · FoundationPose · RGB-D / LiDAR Processing
          icon: hero/eye
        - name: Tools
          description: Git · Docker · Linux · LaTeX
          icon: hero/wrench-screwdriver
    design:
      columns: '4'

  - block: markdown
    content:
      title: Contact
      subtitle: ''
      text: |-
        I am interested in research topics related to **embodied AI, robot learning, vision-language-action models, and robotic perception**.

        **Email:** [uzhhj@student.kit.edu](mailto:uzhhj@student.kit.edu)  
        **Location:** Karlsruhe, Germany  
        **GitHub:** [W-Y-Zhang](https://github.com/W-Y-Zhang)
    design:
      columns: '1'
---
