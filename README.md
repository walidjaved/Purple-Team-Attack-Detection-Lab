# Purple Team Attack & Detection Lab

<h2> Description</h2>
<p><b>This project simulates a cyberattack using Kali Linux and detects malicious activity using Splunk SIEM and Sysmon logs.</b></p>

<p>In this project:
<ol>
  <li>Launch Attack</li>
  <li>Collect Logs</li>
  <li>Detect suspicious activity</li>
  <li>Investigate the attack</li>
</ol>
</p>

<h2>Tools Used</h2>
<table>
  <tr>
    <th>Tool</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>Virtual Box</td>
    <td>Run Virtual Machines</td>
  </tr>
    <tr>
    <td>Kali Linux</td>
    <td>Attack Machine</td>
  </tr>
    <tr>
    <td>Windows 11 VM</td>
    <td>Victim Machine</td>
  </tr>
    <tr>
    <td>Splunk</td>
    <td>Log Analysis</td>
  </tr>
    <tr>
    <td>Sysmon</td>
    <td>Detailed Windows Logging</td>
  </tr>
    <tr>
    <td>Nmap</td>
    <td>Reconnaissance</td>
  </tr>
    <tr>
    <td>Metasploit</td>
    <td>Exploitation</td>
  </tr>
</table>

<h2>Virtualization</h2>
<p>For this project, I am utilizing Virtual Box. Virtual Box gives us the opportunity to run multiple machines in a sandbox environment. We can create Windows hosts, Linux hosts, etc. to create a safe lab environment for testing purposes. It is great tool to use for simulating real threats and defending against them without causing harm to real systems.</p>
<p>I downloaded and installed Virtual Box on my machine to start creating my test environment.</p>
<img width="955" height="537" alt="image" src="https://github.com/user-attachments/assets/66475b3d-cd4b-4908-8e49-a97c49fe827a" />
<h2>Create Lab Machines</h2>

  <h4>Machine 1: Attacker</h4>
  <h4>Machine 2: Victim</h4>
  <h4>Machine 3: SIEM</h4>
<h2>Configure the Network</h2>
<h2>Install Sysmon on Windows</h2>
<h2>Install Splunk on Ubuntu</h2>
<h2>Send Windows Log to Splunk</h2>
<h2>Perform Attacks (Red Team)</h2>
  <h4>Attack 1 - Network Scan</h4>
  <h4>Attack 2 - Brute Force Login</h4>
  <h4>Attack 3 - Exploitation</h4>
<h2>Detect Attacks (Blue Team)</h2>
  <h4>Detect Process Execution</h4>
  <h4>Detect Powershell Abuse</h4>
  <h4>Detect Network Connections</h4>
  <h4>Detect Suspicious Activity</h4>
<h2>Build a Detection Dashboard</h2>
<h2>Investigate the Attack</h2>
