# Incident Response Analysis

A simulated ICMP flood incident analysed through the five NIST CSF functions used in the original exercise: Identify, Protect, Detect, Respond and Recover.

**Skills:** Incident response, network security, recovery planning

## Project context

This repository presents an educational exercise. References to organisations and incidents describe the exercise scenario, not professional employment or a client engagement.

> ## Scenario
>You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced >a DDoS attack, which compromised the internal network for two hours until it was resolved.
>
>During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident >management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 
>
>The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This >vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 
>
>To address this security event, the network security team implemented: 
>
> - A new firewall rule to limit the rate of incoming ICMP packets
>
> - Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
>
> - Network monitoring software to detect abnormal traffic patterns
>
> - An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics
>
>As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) >Cybersecurity Framework (CSF). You will use the CSF to help you navigate through the different steps of analyzing this cybersecurity event and integrate your analysis into a general security strategy. We have >broken the analysis into different parts in the template below. You can explore them here:
>
>  - **Identify** security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 
>
> - **Protect** internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 
>
> - **Detect** potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 
>
> - **Respond** to contain, neutralize, and analyze security incidents; implement improvements to the security process. 
>
> - **Recover** affected systems to normal operation and restore systems data and/or assets that have been affected by an incident. 

___


| Summary |
| ------- |
| The company experienced a **Distributed Denial of Service (DDoS) attack** characterized by a flood of ICMP packets targeting the internal network. The attack exploited an **unconfigured firewall**, overwhelming network resources and causing network services to become unresponsive for approximately **two hours**. The source of the attack was traced to **multiple malicious external IP addresses** flooding the network with ICMP packets. The incident was mitigated by **blocking all incoming ICMP traffic** and restoring critical network functions. |

---

| Identify |
| -------- |
| **Attack Type:** Distributed Denial of Service (DDoS) via ICMP flood  
 **Affected Systems:** Internal network services, including critical and non-critical servers, were unavailable.  
 **Attack Vector:** Exploited an unconfigured firewall rule allowing unlimited ICMP traffic.  
 **Business Impact:** Network downtime for two hours affected productivity and client service, potentially impacting revenue and reputation.  
 **Users Affected:** All internal employees and systems reliant on network services experienced outages. |

---

| Protect |
| ------- |
  Update firewall configurations to **block or rate-limit ICMP packets** by default.  
  Implement **source IP verification (ingress filtering)** to prevent IP spoofing.  
  Establish **regular firewall audit policies**.  
  Provide **cybersecurity awareness training** for staff.  
  Deploy **Intrusion Prevention Systems (IPS)**.  
  Ensure all devices have **latest patches and updates**.  
  Implement **network segmentation** to reduce attack impact. 

---

| Detect |
| ------ |
|  Deploy **network monitoring tools** (e.g., SIEM).  
  Use **IDS/IPS** to detect/block unusual ICMP patterns.  
 Continuously monitor **firewall logs and traffic flows**.  
 Track **authorized vs unauthorized activities**.  
 Implement **automated alerting systems** for IT staff. |

---

| Respond |
| ------- |
|  **Contain** by blocking suspicious traffic and isolating affected segments.  
 **Neutralize** using firewall rules and IPS signatures.  
 Conduct **post-incident analysis** with logs and captures.  
 Communicate **incident status** to teams and management.  
 Update **response playbooks and firewall policies**.  
 Plan **regular drills** to improve readiness. |

---

| Recover |
| ------- |
|  Restore **critical services** after confirming threats are neutralized.  
Ensure all devices follow **updated firewall policies**.  
 Validate **system/data integrity**.  
 Document **incident and recovery process**.  
Review **disaster recovery/continuity plans**.  
 Communicate **recovery status** to stakeholders. |

---

| Reflections / Notes |
| ------------------ |
|  Highlights the **need for proactive firewall configuration** and audits.  
 Combines **technical controls** (firewalls, IDS/IPS) and **processes** (training, monitoring, response planning).  
Future investments in **traffic analysis and automated mitigation** will strengthen resilience.  
 **Continuous improvement** ensures defenses evolve against emerging threats. |

[Back to my portfolio](https://github.com/aaraf18)
