---
title: ''
summary: 'Robotics and embodied AI research by Wenyuan Zhang at KIT. Seeking Ph.D. opportunities starting in Fall 2027.'
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
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
        size: large
        shape: rounded

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

  - block: resume-experience
    id: research-experience
    content:
      username: me
    design:
      date_format: 'January 2006'
      css_class: homepage-research-only

  - block: markdown
    id: talks
    content:
      title: Talks & Presentations
      text: |-
        ### Foundation Models for Dynamic Role Assignment

        **H²T Seminar: Humanoid Robotics · KIT · Winter 2025/26**

        Wrote a seminar paper organizing foundation-model task allocation around two questions: *who should do a task* and *who can do a task*. Covered human–robot and multi-robot collaboration, capability and uncertainty modeling, conformal prediction, and centralized, decentralized, and hybrid LLM planners.

        Delivered a **15-minute research talk in English** as the sole presenter.

        **Supervisors:** Timo Birr and Prof. Tamim Asfour.
    design:
      columns: '1'

  - block: features
    content:
      title: Technical Skills
      items:
        - name: Learning & VLA
          description: Python · PyTorch · GR00T · LeRobot
          icon: hero/code-bracket
        - name: Robotics
          description: ROS 1/2 · Isaac Lab · MuJoCo · Gazebo · MoveIt · Teleoperation
          icon: hero/cog-6-tooth
        - name: Perception
          description: OpenCV · SAM2/SAM3 · GroundingDINO · FoundationPose · RGB-D / LiDAR
          icon: hero/eye
        - name: Tools
          description: Git · Docker · Linux · LaTeX
          icon: hero/wrench-screwdriver
    design:
      columns: '4'

  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        I am seeking **Ph.D. opportunities starting in Fall 2027** in embodied AI, vision-language-action models, robot learning, and robotic manipulation.

        **Email:** [uzhhj@student.kit.edu](mailto:uzhhj@student.kit.edu)

        **Location:** Karlsruhe, Germany

        **GitHub:** [W-Y-Zhang](https://github.com/W-Y-Zhang)

        **LinkedIn:** [wenyuan-zhangkit](https://www.linkedin.com/in/wenyuan-zhangkit/)

        **CV available upon request.**
    design:
      columns: '1'
---
