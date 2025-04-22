# CapturingwithTcpdumpLab

<h2>Description</h2>
The purpose of this lab is to expose us to tcpdump and give us time to familiarize ourselves with the terminal and utilizing tools within it. We will practice various tcpdump basics such as reading from and writing to files, utilizing basic switches, and locating files in the terminal. While completing this labs, we can explore and practice using different switches and functionality within tcpdump. 
<h2>Languages and Utilities</h2>

- <b>Wireshark </b>
- <b>Linux </b>

<h2>Enviroments Used </h2>

- <b>Tcpdump</b> 
- <b>Hack the Box (HTB)</b>

<h2>Course of Action</h2>

- Validate tcpdump in Different Environments – Ensure tcpdump is properly installed and functional across various operating systems, reinforcing my ability to set up and troubleshoot network monitoring tools.
- Expand Capture Techniques – Experiment with different capture filters to refine packet collection, focusing on specific protocols and traffic patterns to improve efficiency.
- Analyze Real-World Traffic – Apply the techniques learned in the lab to analyze network traffic in controlled environments, identifying anomalies and potential security threats.
- Integrate Findings into Security Operations – Explore how packet captures can be leveraged in incident response and threat hunting, incorporating them into broader security workflows.
- Document & Share Insights – Publish findings and methodologies on GitHub to contribute to the cybersecurity community while refining technical documentation skills.

<h2>Lab walk-through:</h2>

<p align="center">
Confirming tcpdump is installed: <br/>
<img width= "776" alt="Confirming tcpdump is installed" src="https://i.imgur.com/mnXyZF6.png">
  
<p align="center">
Running the capture, This command captures network traffic on the eth0 interface. The output provides detailed packet information related to HTTP traffic between a local host and a remote server.

 <br/>
<img width="775" alt="creating users for power shell" src="https://i.imgur.com/E4Qb9TL.png">

<p align="center">
Designating & saving capture to a .PCAP file,I set up tcpdump to capture live network traffic on the eth0 interface. Initially, I encountered an error due to a missing directory, but after resolving it with mkdir -p /home/user/captures, I successfully captured 1681 packets in a .pcap file. The process confirmed that all packets were recorded without kernel drops, ensuring a complete and reliable dataset for further analysis.
 <br/>
<img width="774" alt="Running users" src="https://i.imgur.com/9jsD8Av.png">

<p align="center">
Reading the Capture from a .PCAP file,The output reveals traffic exchanges, including source and destination IPs, TCP flags, sequence numbers, and payload data. Using tcpdump -nnr, I efficiently parsed packet details, ensuring a comprehensive review of network activity for forensic analysis and troubleshooting.
 <br/>
<img width="774" alt="Running users" src="https://i.imgur.com/SpzpVHs.png">

<p align="center">
Read the Capture from a .PCAP file pt 2, This screenshot showcases tcpdump in action within Parrot Terminal on a Parrot Security OS system. The command used tcpdump -nnr /home/user/captures/network_capture.pcap
 <br/>
<img width="774" alt="Running users" src="https://i.imgur.com/dc3MVWM.png">

<h2> Reflection </h2>
The Capturing TCP Dump Lab on Hack The Box provided a practical scenario where I acted as a network administrator tasked with capturing and analyzing network traffic to baseline and validate the organization's network. Using tcpdump, I explored capturing traffic within a local broadcast domain, ensuring the tool was properly installed and functional. The lab emphasized adding verbosity to outputs, saving captures to .pcap files, and analyzing them for insights. This hands-on experience reinforced my ability to use tcpdump effectively for network traffic analysis, a critical skill for both offensive and defensive security operations.

<h2> Conclusion </h2>
The Capturing TCP Dump Lab on Hack The Box helped me better understand how to check and study the data flowing through a network. Using a tool called tcpdump, I practiced finding and capturing this data and then analyzing it to understand what's happening in a network. This lab showed me how important it is to keep an eye on the activity in a network, as it helps to spot any unusual behavior or issues. It was a great hands-on experience that taught me valuable skills I can use in real-world cybersecurity scenarios.



