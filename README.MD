# RDP Failed to locate IP Geolocation Information
![Sentinal_Lab_Image_1](https://github.com/kleeloy/Azure-Sentinal-Lab/blob/main/Diagrams/ipgeolocation.png)

## Description
#### This repository's powershell script is responsible for atomizing Windows event log information for failed RDP attacks and using an API (third party) to collect geographic information about the attackers location.


In this lab, the script is used in my setup with Azure Sentinel (SIEM) and connects it to a live virutal machine acting as a honey pot. I observed live attacks (RDP brute force) from all around the world. I used a custome powershell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map.
![Sentinal_Lab_Image_2](https://github.com/kleeloy/Azure-Sentinal-Lab/blob/main/Diagrams/sentinal%20part1.png)

## Languages Used:
Powershell: Extracted RDP failed logins that were logged from Windows Event Viewer.

## Utilities USed:
IPGEOLOCATION.io: IP address to geolocation API
