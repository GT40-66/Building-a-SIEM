<h1>Building a SIEM - Microsoft Azure Sentinel </h1>


<h2>Description</h2>
This project demonstrates how to utilize Microsoft Sentintel to create a graphical display of RDP attempts on a honeypot VM. This lab utlizes a custom PowerShell script to extract metadata from Windows Event Viewer that is forwarded to a third party API in order to retrieve geolocation data. I configured a custom log within Log Analystics Workspace in Azure to ingest the data that is linked to the ProgramData file within the VM. Custom Fields were then created in order to properly label the data. I then created a workbook within Azure Sentinel (Microsoft's cloud SIEM) to display this data and create hot spots to demonstrate number of RDP attempts per region. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>ipgeolocation.io</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Custom Log: <br/>
<img src="<a href="https://imgur.com/BZpJtwH"><img src="https://i.imgur.com/BZpJtwH.png" height="80%" width="80%" alt="Custom Log"/>
<br />
<br />
Map Data:  <br/>
<img src="<a href="https://imgur.com/BlBrz3e"><img src="https://i.imgur.com/BlBrz3e.png" height="80%" width="80%" alt="Custom Log"/>
<br />
Example of PowerShell script running with failed attempts:  <br/>
<img src="<a href="https://imgur.com/1cgeeA5"><img src="https://i.imgur.com/1cgeeA5.png"  height="80%" width="80%" alt="Custom Log"/>
<br />
Log of geolocation data on the virtual machine:  <br/>
<img src="<a href="https://imgur.com/vF3hr5i"><img src="https://i.imgur.com/vF3hr5i.png"  height="80%" width="80%" alt="Custom Log"/>
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
