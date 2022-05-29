---
layout: default
title: Semi. Motor control, 2020
parent: Portfolio
nav_order: 9
---


## Semiconductor Production Machine Motor Control System, 2020 
    * Motor Start/Stop/Idle/... StateMachine control customizing
    -> Due to high level controller's interface limitations Motor Drive's function customizing

Jul 2020 ~ Sep 2020
Worked with Omron for Samsung Electronics. The engineer at Omron, he didn't want to change his program for reliability. Or I could guess he didn't know how to adapt "My company" Motor Drive to Omron PLC interfacing. We knew that it was big volume sales so I had to customize(trick) "My company" Motor Drive's StateMachine sequence.
By default, it was impossible to control mode change while Motor is Powered-up. For example, Speed control Mode to Torque control Mode or vice versa, it could make Motor Drive behavior unsafe. So I did some study and modify the default program. The trick was, by custom software I composed, when we need to change control mode, Just made Motor Drive Power-down and Power-up so that the Drive could change the mode.

![sample img](/assets/images/portfolio-2020-samsung-semicond.png)

- Developer: Taeung Ha
- Actual time for development: about 2 months
- Contribution rate: 100%
- Technologies used: Codesys(ST programming)