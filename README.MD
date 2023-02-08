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

## Attacks from Iran and Urkaine coming in; custom logs being output with geodata
![Sentinal_Lab_Image_4](https://github.com/kleeloy/Azure-Sentinal-Lab/blob/main/Diagrams/plotting%20senntinial%20lab.png)

## World map of incoming attacks after 1st hour (built custom logs including geodata)
![Sentinal_Lab_Image_5](https://github.com/kleeloy/Azure-Sentinal-Lab/blob/main/Diagrams/Sennital%20lab%2010%20minutes%20after%20exposed%20RDP.png)


