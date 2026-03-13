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
<p>For this project, I am utilizing Virtual Box. Virtual Box gives us the opportunity to run multiple machines in a sandbox environment. We can create Windows hosts, Linux hosts, etc. to create a lab environment for malware testing and learning tools safely. It is a great tool to use for simulating real threats and defending against them without causing harm to real systems.</p>
<p>I downloaded and installed Virtual Box on my machine to start creating my test machines and environment.</p>


<img width="955" height="537" alt="image" src="https://github.com/user-attachments/assets/66475b3d-cd4b-4908-8e49-a97c49fe827a" />


<h2>Create Lab Machines</h2>

  <h4>Machine 1: Attacker</h4>
  
  <table>
      <tr>
        <th>OS</th>
        <th>Purpose</th>
      </tr>
      <tr>
        <td>Kali Linux</td>
        <td>Simulate cyberattacks</td>
      </tr>
  </table>

  <p>Kali is a popular and powerful operating system built on Linux. It is primarily used for penetration testing offering a plethora of tools built right in to the operating system. I will use this machine as the "attacker" machine to simulate actual attacks like any enterprise could face in the real world.</p>

![Kali](screenshots/Kali.PNG)
    
  <h4>Machine 2: Victim</h4>

  <table>
      <tr>
        <th>OS</th>
        <th>Purpose</th>
      </tr>
      <tr>
        <td>Windows 11</td>
        <td>Generate logs from attack</td>
      </tr>
  </table>

  <p>The victim machine is a Windows 11 host. Windows is the most common operating system in the world and is widely used in private corporations as well as government environments. Using Windows as a victim machine provides valuable insight to what most machines could experience during a cyberattack.</p>
  
  <h4>Machine 3: SIEM</h4>

  <table>
      <tr>
        <th>OS</th>
        <th>Purpose</th>
      </tr>
      <tr>
        <td>Ubuntu Server</td>
        <td>Log collection and analysis</td>
      </tr>
  </table>

  <p>The machine I am using for a SIEM environment is Ubuntu. Ubuntu is one of the most popular LInux distros. It provides wide compatibility and a solid, reliable host for log ingestion. I will install Splunk on this machine for the SIEM.</p>
  
<h2>Configure the Network</h2>

<h2>Install Sysmon on Windows</h2>

<h2>Install Splunk on Ubuntu</h2>

<h2>Send Windows Log to Splunk</h2>

<h2>Perform Attacks (Red Team)</h2>
  <h4>Attack 1 - Network Scan</h4>
    <pre>
      <code>
        nmap -sS 192.168.56.20
      </code>
    </pre>
    
  <h4>Attack 2 - Brute Force Login</h4>
    <pre>
      <code>
        hydra -l administrator -P rockyou.txt smb://192.168.56.20
      </code>
    </pre>
    
  <h4>Attack 3 - Exploitation</h4>
      <pre>
      <code>
        msfconsole
      </code>
      <code>
        exploit/windows/smb/ms17_010_eternalblue    
      </code>
    </pre>
  
<h2>Detect Attacks (Blue Team)</h2>
  <h4>Detect Process Execution</h4>
  <h4>Detect Powershell Abuse</h4>
  <h4>Detect Network Connections</h4>
  <h4>Detect Suspicious Activity</h4>
  
<h2>Build a Detection Dashboard</h2>

<h2>Investigate the Attack</h2>
