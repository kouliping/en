# Infrastructure

    The Anti-DDoS Basic framework consists of three modules: management center equipment, detection equipment and cleaning equipment.
    
## Business Architecture

The Anti-DDoS Basic business structure is as shown in the following figure:

![Create instance](https://github.com/jdcloudcom/cn/blob/edit/image/Basic%20Anti-DDos/Infrastructure01.png)

Note: 1. Mirror traffic to the detection equipment 2. The detection device detects an attack, and notifies the management center of the attack information.
      3. After receiving the attack information, the management center shall notify the cleaning equipment to start cleaning.
      4. Drain the traffic to the cleaning equipment for traffic cleaning and reinject cleaned traffic.
      5. Normal traffic

| Name | Description |
| - | - |
The management center | is mainly responsible for receiving attack information and sending a cleaning strategy to the cleaning equipment to guide the cleaning equipment to carry out flow cleaning.
| Cleaning equipment | is mainly responsible for cleaning attack traffic according to the cleaning strategy issued by the management center and reinjecting the cleaned traffic.
| Detection Device | is mainly responsible for anayzing the traffic to to determine whether there is an attack or not, and sending attack information to the management center if attack occurs.

## Related Reference

- [What is Anti-DDoS-Basic](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Overview.md)
- [Core Concepts](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Core-Concepts.md)
- [Application Scenarios](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Application-Scenarios.md)
- [Basic Function](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Functions.md)
- [Use limit](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Restrictions.md)
