# Home Networking Projects
Welcome to my networking projects repository. I will be doing writeups on the various networking projects I have undertaken at home to expand my knowledge and skills in networking and security practices!

## Table of Contents

1. [Project 1: Running Wires](#project-1-running-wires)
2. [Project 2: Network and Server Setup](#project-2-network-and-server-setup)
3. [Project 3: Home SIEM](#project-3-home-siem)

## Project 1: Running Wires

### Objective
Setting up fast and reliable connections throughout the house using Cat 6 UTP cabling to reduce signal drops and improve efficiency for high-bandwith devices.

### Components Used
- Cat 6 UTP Ethernet Cabling
- Outdoor Cat 6 Shielded FTP Cabling
- Wall Plates
- Keystone Jacks
- Passthrough Connectors
- Tools: Cable tester, crimping tool, punch-down tool, drill, drill extensions, cable ties, glow fish rod set

### Planning and Design 
- **Powerpoint**: Created a convincing powerpoint and gave a convincing presentation to get the go ahead to put holes in the walls of my parents house.
- **Centeralized Location**: Identified and decided on the optimal location of the server rack based on the proximity and floor difference of each run.  
- **Network Map**: Measured out specific lengths needed for each cable run based on the position of the room and how high the wall plate was from the floor.

### Setup and Configuration
- **Running Cables**: Used the drill to open up access to the desired runway locations and used the glow fish rods to run them through said locations.
- **Terminating Cables**: Hand terminated all runs with keystone jacks abd installed the keystone jacks into the wall plates. I also hand made all the patch cables for each connection.
- **Testing and Troubleshooting**: Used a cable tester to ensure proper connection and function.

### Challenges and Solutions
- **Challenge**: Running cables through difficult-to-access areas.
  **Solution**: Bought and used a right angel drill extension.
  - **Challenge**: Getting a line from the demarc point outside to the centeralized location.
  **Solution**: Purchased and used outdoor rated cable that was also shielded, along with drilling a hole in the attic wall to gain access to the outside before filling it up with weather resistant silicone caulk.

### Results
- Achieved a stable and high-speed Ethernet network throughout the house.
- Improved internet speeds and reduced latency.
- Enhanced performance for streaming, gaming, and work-from-home setups.
- No more complaining about lag from my brothers! =)

## Project 2: Network and Server Setup

### Objective
Setup all network devices, as well as setting up each server to do specific tasks on the network.

### Components Used
- Gateway/Router: [UDM Pro by Ubiquiti]
- Switch: USW Pro [24 POE by Ubiquiti]
- APs: [1x U6 In-Wall,2x U6 Extenders all by Ubiquiti]
- Server Units:[3x HP ProLiant DL360 Gen9 by HP]
- Firewall:[Classified]

### Setup and Configuration
- **Firewall Configuration**: Used software to configure the firewall and make an in-depth ACL to block or allow traffic.
- **AP Tweaking**: Used Ubiquitis built in software to configure the APs to ensure proper transmitting power to avoid overlapping signals.
- **Server Setup**: Gave static IPs to each in use server unit and installed software on them. (ProxMox and PiHole respectively)

### Challenges and Solutions
- **Challenge**: Struggled to isolate IoT devices from the rest of the network.
  **Solution**: Created and configured different VLANs to segment out the network to ensure isolation.
- **Challenge**: Certain devices were not able to connect to the PiHole server and thus were unable to complete DNS requests.
  **Solution**: Edited ACLs to allow certain VLANs to send traffic to the server unit running PiHole.

## Project 2: Home SIEM and Security

#CURRENTLY IN PROGRESS
