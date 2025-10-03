# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>

<img width="629" height="618" alt="image" src="https://github.com/user-attachments/assets/7fc01d68-7ed9-43c0-9443-7ac85f4c4a5d" />

<img width="627" height="617" alt="image" src="https://github.com/user-attachments/assets/b2cbb9a0-cd78-4446-8ee4-71d6e5923cba" />


•	PDU details for remote communication<br>

<img width="628" height="626" alt="image" src="https://github.com/user-attachments/assets/f19f2ba6-ec3b-4784-b074-54d09f8ec6cb" />

<img width="626" height="580" alt="image" src="https://github.com/user-attachments/assets/74ff2c67-65ba-403a-a071-15d65c4dc305" />


•	Tables showing MAC/IP changes through each device<br>

<img width="774" height="177" alt="image" src="https://github.com/user-attachments/assets/01d3966e-0eb2-415f-ade0-7315d7d58c20" />

<img width="766" height="227" alt="image" src="https://github.com/user-attachments/assets/178c7bb7-7778-4a2a-b317-1ba370fe9b4f" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

