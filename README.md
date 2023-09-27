<h1>Setup SIEM in Azure</h1>

<h2>Description</h2>
Used custom PowerShell script to extract metadata from Windows Event Viewer to be forwarded to third party API in order to derive geolocation data. Configured Log Analytics Workspace in Azure to ingest custom logs containing geogrphic information (latitude, longitude, state/province, and country). Used KQL to parse log data and configured Azure Sentinel (Microsoft's cloud SIEM) workbook to display global attack data (RDP brute force) on world map according to physical location and magnitude of attacks.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>Azure</b>
- <b>Sentinel</b>
- <b>IPGeolocation.io</b>
- <b>KQL</b>

<h2>Environments Used </h2>

- <b>Windows 10 Virtual Machine</b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
