# FAQ

**1, Q: What is the Anti-DDoS Basic protection application scenario?**

A: JD Cloud Anti-DDoS Basic is applied to attack protection scenarios with the highest attack flow rate below 2G. Once the attack flow exceeds the basic protection capability of the machine room, the black hole will be triggered to limit the public IP of the black hole for a certain period of time.

**2, Q: How do I start the Anti-DDoS Basic?**

A: The Anti-DDoS Basic is automatically started for each public network IP purchased from JD Cloud, providing 2G defense bandwidth.

**3, Q: How to stop the Anti-DDoS Basic?**

A: The Anti-DDoS Basic is automatically started and cannot be stopped. Anti-DDoS Basic protects your public network IP from DDoS and has no impact on normal business access.

**4, Q: What are the requirements for the defensed public network IP?**

A: Anti-DDoS Basic can only defend filed domains. If the domain is not filed, defense will stop immediately, and the warning notification will be sent.

**5, Q: How long will the public IP that triggers a black hole stay in the black hole state?**

A: A public network IP triggering a black hole stays in black hole for at least 60 minutes, during which the public network IP is still monitored. Once another attack exceeding the basic protection capability of the machine room is monitored, the black hole time will be extended by 60 minutes at the last time the attack was monitored.
  
**6, Q: What will happend when attack traffic exceeds 2G?**

A: The black hole is triggered when the attack traffic exceeds 2G, and the access to the IP is shielded for a certain period of time. It is recommended that you purchase JD Cloud [Anti-DDoS Pro](https://www.jdcloud.com/products/ipanti) services from JD Cloud for stronger defense ability.

**7, Q: What attack types are supported for Anti-DDoS Basic**

A: Including but not limited to SYN Flood, ACK Floods, TCP Floods, UDP Flood, DNS reflection attacks, NTP reflection attacks, SSDP reflection attacks, and other common attacks.

If the above cannot solve your problem, please consult the after-sales of the product: [after-sales consultation](https://ticket.jdcloud.com/myorder/form?cateId=2&questionId=13)

# Related Documents

- [What is the Anti-DDoS Basic? ](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Overview.md)
- [Anti-DDoS Basic Structure](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Introduction/Basic-Infrastructure.md)
- [Quick Start](https://github.com/jdcloudcom/cn/blob/edit/documentation/Cloud-Security/Basic-Anti-DDoS/Getting-Started/Basic-Anti-DDos-Started.md)
