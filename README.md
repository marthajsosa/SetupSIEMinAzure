# Setup SIEM in Azure

<h2>Description</h2>
In a Windows 10 virtual machine, used custom PowerShell script to extract metadata from Windows Event Viewer to be forwarded to third party API in order to derive geolocation data. Configured Log Analytics Workspace in Azure to ingest custom logs containing geogrphic information (latitude, longitude, state/province, and country). Used KQL to parse log data and configured Azure Sentinel (Microsoft's cloud SIEM) workbook to display global attack data (RDP brute force) on world map according to physical location and magnitude of attacks.
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
Create virtual machine & turn off all Firewalls: <br/><img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/28b076db-cad1-4b90-8df3-3c17ea8ee6d0"/>

<br />
<br />
Create Log Analytics Workspace in Azure:  <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/577fc67b-e425-4e00-aaf6-1f15f43eeb0c"/>
<br />
<br />
Setup Microsoft Sentinel: <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/7947a029-de16-409a-a36b-356a49f9baae"/>
<br />
<br />
Use Geolocation.io API Key in Powershell Script to capture failed login attempts in Windows Event Viewer including latitude and longitude of the IP addresses attempting to attack brute force:  <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/20848687-be4c-4ea0-94fc-0829b525bd5b"/>
<br />
<br />
Create Log Analytics Workspace:  <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/8535c0c8-fe45-4a65-8082-dadeb80a4c5f"/>
<br />
<br />
Connect custom log and extract fields from raw data with KQL: <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/8f94d8d4-8308-4549-8c92-6739ce5bb031"/>
<br />
<br />
Visualize data on a map according to attack concentration :  <br/>
<img src="https://github.com/urmomtookurscreentime/SetupSIEMinAzure/assets/146014829/e97931e0-762a-49ad-bd90-8883881522b0"/>
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
