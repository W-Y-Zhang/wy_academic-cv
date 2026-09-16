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

  - block: resume-awards
    content:
      username: me
      title: Honors & Awards
    design:
      date_format: 'January 2006'

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
        I am seeking **Ph.D. opportunities starting in Fall 2027** in embodied AI, vision-language-action models, robot learning, and robotic manipulation.

        **Email:** [uzhhj@student.kit.edu](mailto:uzhhj@student.kit.edu)

        **Location:** Karlsruhe, Germany

        **GitHub:** [W-Y-Zhang](https://github.com/W-Y-Zhang)

        **LinkedIn:** [wenyuan-zhangkit](https://www.linkedin.com/in/wenyuan-zhangkit/)

        **CV available upon request.**
    design:
      columns: '1'
---
