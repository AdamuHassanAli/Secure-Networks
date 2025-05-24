# Network Protocol Analysis and DNS Failure Investigation for Client Website Access Issue
<h2>Project Description:</h2>
<p>In this project, I acted as a Cybersecurity Analyst tasked with investigating a service outage incident affecting a client website, www.yummyrecipesforme.com. Several end users reported an error message stating “destination port unreachable” when attempting to access the website. My role involved analyzing the incident to identify the affected network protocol and underlying cause of the disruption.</p>

![Image](https://github.com/user-attachments/assets/be16fa05-bdfc-4269-bb38-483972944150)

To begin the investigation, I attempted to replicate the issue and confirmed the error. I then utilized the tcpdump network analyzer to capture and inspect network traffic in real time during the attempted page load. Key steps of the analysis included:
<li>Observing the browser's DNS resolution process, where a UDP packet was sent to port 53 of the DNS server to resolve the domain name.</li><br>
<li>Analyzing captured packets that revealed ICMP error responses indicating “udp port 53 unreachable.”</li><br>
<li>Identifying that no service was listening on the DNS server's port 53, resulting in failure to resolve the domain and subsequently load the HTTPS website.</li><br>
<li>Confirming the root cause of the issue was a disruption in the DNS service, which uses the UDP protocol on port 53.</li><br><br>
Based on packet data analysis and timestamps, I compiled a technical report summarizing the findings, which was escalated to the security engineering team for resolution. This project demonstrates my ability to use network forensics to isolate protocol-level failures and effectively communicate incident impact to key stakeholders.

<h2>Skills Demonstrated:</h2>
<li>Network protocol analysis</li>
<li>DNS and UDP traffic inspection</li>
<li>Use of tcpdump for packet capture</li>
<li>ICMP error interpretation</li>
<li>Incident documentation and reporting</li>
<li>Communication with incident response teams</li>

<h2>Reports</h2>
