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

  - block: markdown
    content:
      title: 'About Me'
      subtitle: ''
      text: |-
        I am an M.Sc. student in Mechatronics and Information Technology at Karlsruhe Institute of Technology (KIT), specializing in Robotics.

        My interests lie in **embodied AI, robot learning, vision-language-action models, and robotic perception**. I am particularly interested in enabling robots to understand visual and language instructions, adapt across different robotic embodiments, and perform manipulation tasks in real-world environments.

        My current Master's thesis focuses on **object-centric vision-language-action models for few-shot adaptation**, including simulation-based demonstration collection, robot data preprocessing, and policy training across multiple robotic platforms.

        Previously, I worked as a Research Assistant at KIT's Institute for Material Handling and Logistics, where I contributed to projects in **panoptic segmentation, LiDAR-based localization and mapping, and autonomous mobile robotics**.
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Research Interests'
      subtitle: ''
      text: |-
        **Embodied AI**  
        Learning systems that connect perception, language, and physical interaction.

        **Vision-Language-Action Models**  
        Generalist robot policies that map visual observations and language instructions to robot actions.

        **Robot Learning**  
        Learning manipulation skills from demonstrations and adapting learned policies across tasks and robot platforms.

        **Robotic Perception**  
        RGB-D perception, object segmentation, 6D pose estimation, tracking, and LiDAR-based environment understanding.
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Research Experience'
      subtitle: ''
      text: |-
        ## Research Assistant
        **Institute for Material Handling and Logistics, Karlsruhe Institute of Technology**  
        Karlsruhe, Germany · **Jun. 2025 – May 2026**

        ### Panoptic Segmentation for Robotic Perception
        Worked on panoptic segmentation for robotic perception using the ARIBIC dataset. Upgraded the CUDA and PyTorch environment for multiple segmentation baselines, adapted the training and evaluation pipelines to the ARIBIC dataset, and created a reproducible Docker-based development environment. Through hyperparameter tuning and model evaluation, improved panoptic quality (PQ) by up to **20% relative improvement**.

        ### Dual-LiDAR AGV Localization and Mapping
        Developed a dual-LiDAR perception and localization pipeline for an autonomous guided vehicle. Implemented time synchronization, coordinate transformation, and 360° scan resampling for front and rear LiDAR sensors in ROS and offline processing. Adapted an open-source FastSLAM implementation to process fused laser scans and odometry for simultaneous localization and occupancy-grid mapping. Built an alternative two-stage pipeline using **GMapping and AMCL**, and compared the resulting localization trajectories with FastSLAM using the same real-world AGV dataset.
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Selected Projects'
      subtitle: ''
      text: |-
        ## Object-Centric VLA for Few-Shot Adaptation
        **Master's Thesis · Aug. 2026 – Present**

        My current Master's thesis investigates object-centric representations for vision-language-action models and their ability to adapt across different robotic embodiments. I built simulation environments for **three robot platforms** and implemented data preprocessing and format conversion pipelines to support demonstration collection and robot policy training. My current work focuses on integrating **Isaac Lab teleoperation** for collecting demonstrations and preparing the resulting data for **GR00T-based policy training with object-centric conditioning**.

        ## Vision- and Language-Guided Robotic Grasping
        **ROS 2 · MuJoCo · VLM · Grounded-SAM2 · FoundationPose · MoveIt · Python**  
        **May 2026 – Aug. 2026**

        Developed an end-to-end robotic manipulation pipeline that converts natural-language or voice instructions into object grasping and semantic placement actions. The perception pipeline combines a vision-language model for target identification, **Grounded-SAM2** for instance segmentation, and **FoundationPose** for 6D object pose estimation from RGB-D observations.

        Designed a follow-then-grasp strategy combining optical-flow and depth feedback with loss-triggered re-detection and mask refresh before pose estimation. This increased tracking retention from **78.4% to 87.9%** and reduced the identity-switch rate from **16.7% to 6.7%** over 30 matched motion sequences per configuration. The complete system achieved **86.7% end-to-end language-to-placement success**.

        ## Multi-Robot Intralogistics Automation
        **ROS 1 · Gazebo · Python · Dec. 2024 – Feb. 2025**

        Developed a multi-station intralogistics automation system integrating **three 4-DoF robotic arms, a linear rail, and a conveyor belt**. Implemented inter-station task coordination through ROS nodes and validated suction-based pick-and-place operations both in **Gazebo simulation and on physical hardware**.
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Education'
      subtitle: ''
      text: |-
        ## Karlsruhe Institute of Technology
        **M.Sc. in Mechatronics and Information Technology**  
        Specialization in Robotics  
        Karlsruhe, Germany · **Apr. 2024 – Present**

        ## Qingdao University
        **B.Eng. in Electrical Engineering and Automation**  
        Qingdao, China · **Sep. 2018 – Jun. 2022**
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Technical Skills'
      subtitle: ''
      text: |-
        **Programming**  
        Python

        **Robotics**  
        ROS 1 / ROS 2 · Gazebo · MuJoCo · MoveIt · Isaac Lab

        **Perception & Machine Learning**  
        PyTorch · OpenCV · SAM2 · FoundationPose · RGB-D Processing · LiDAR Processing

        **Tools**  
        Git · Docker · Linux · LaTeX

        **Languages**  
        Mandarin Chinese — Native  
        English — IELTS 6.5  
        German — telc C1
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Contact'
      subtitle: ''
      text: |-
        I am interested in research topics related to **embodied AI, robot learning, vision-language-action models, and robotic perception**.

        **Email:** [uzhhj@student.kit.edu](mailto:uzhhj@student.kit.edu)  
        **Location:** Karlsruhe, Germany  
        **GitHub:** [W-Y-Zhang](https://github.com/W-Y-Zhang)
    design:
      columns: '1'
---
