---
layout: default
title: Semi. Motor control, 2020
parent: Portfolio
nav_order: 9
---


## Semiconductor Production Machine Motor Control System, 2020 
    * Motor Start/Stop/Idle/... StateMachine control customizing.
    -> Due to high-level controller's interface limitations, I customized the Motor Drive's functions.

Jul 2020 ~ Sep 2020

A project for Samsung Electronics involving Omron PLCs. The Omron engineer preferred not to alter their code, so I had to get creative. I customized our motor drive's state machine to handle on-the-fly mode changes (e.g., speed to torque control) by briefly power-cycling the drive logic in software—a neat trick to bypass interface limitations safely.

![sample img](/assets/images/portfolio-2020-samsung-semicond.png)

- Developer: Taeung Ha
- Actual time for development: about 2 months
- Contribution rate: 100%
- Technologies used: Codesys(ST programming)