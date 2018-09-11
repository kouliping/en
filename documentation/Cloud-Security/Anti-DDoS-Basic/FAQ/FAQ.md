# FAQ

** 1, Q: What is the basic protection application scenario?**

A: JD Cloud Basic Anti-DDoS is applied to attack protection scenarios with the highest attack flow rate not exceeding 2G. Once the attack flow exceeds the basic protection capability of the machine room, the black hole will be triggered to limit the public IP of the black hole for a certain period of time.

** 2, Q: How do I start the basic protection? **

A: The basic protection does not need to be opened. As long as the public network IP of JD Cloud is purchased, the DDos defense is automatically started for each public network IP, providing 2G defense bandwidth.

** 3, Q: How to close the basic protection?**

A: The DDos basic protection is automatic opened and cannot be closed. The Basic Anti-DDoS protects your public network IP from DDos and does not have any impact on normal business access.

** 4, Q: What are the requirements for the defense's public network IP?**

A: Basic protection can only defend domains which are filed. If the domain is not filed, the defense will be stopped immediately, and a warning notification will be sent.

** # 5, Q: How long will the public IP that triggers a black hole stay in the black hole?**

A: The residence time of the public network IP triggering a black hole state in a black hole is 60 minutesat least , during which the IP of the public network is still monitored. Once an attack flow exceeding the basic protection capability of the machine root is monitored again, the black hole time is extended by 60 minutes at the last time the attack was monitored.
  
** 6, Q: What will happend when attack flow exceeds 2G?**

A: The black hole is triggered when the attack flow exceeds 2G, and the access to the IP is shielded for a certain period of time. It is recommended that you purchase JD Cloud [Advanced Anti-DDoS](https://www.jdcloud.com/products/ipanti) services from JD Cloud for greater defense ablity.

** 7, Q: What attack types are supported for basic defense **

A: Including but not limited to SYN Flood, ACK Floods, TCP Floods, UDP Flood, DNS reflection attacks, NTP reflection attacks, SSDP reflection attacks, and other common attacks.

If the above cannot solve your problem, please consult the after-sales of the product:[after-sales consultation](https://ticket.jdcloud.com/myorder/form?cateId=2&questionId=13)

# Related Documents

- [What is the foundation protection? ](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Overview.md)
- [Basic Protection Structure](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Basic-Infrastructure.md)
- [Quick Start](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Getting-Started/Basic-Anti-DDos-Started.md)
