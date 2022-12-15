<h1>Failed RDP to IP Geolocation Information</h1>


<h2>Description</h2>
<b>The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://imgur.com/si1KZG1.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer

- <b>Kusto Query Language:</b> Ingest logs and create visualizations in Azure

<h2>Utilities Used</h2>

- <b>ip-api:</b> IP Address to Geolocation API

<h2>World map of incoming attacks after 48 hours</h2>

<p align="center">
<img src="https://imgur.com/RTbyF9E.jpg" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>Additional username data from custom logs</h2>

<p align="center">
<img src="https://i.imgur.com/krRFrK5.jpg" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
