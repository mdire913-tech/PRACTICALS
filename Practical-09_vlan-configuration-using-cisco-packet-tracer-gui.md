# Practical 9 - VLAN Configuration

Source PDF: practical 9.pdf

--- Page 1 ---

Practical:8
AIM: VLAN Configuration Using Cisco Packet Tracer (GUI)

1. What is VLAN?

VLAN (Virtual Local Area Network) is a logical division of a physical network into separate networks. It
allows devices connected to the same physical switch to be grouped into different logical networks.

For example, a college network can be divided into:

   •      VLAN 10 – STUDENTS
   •      VLAN 20 – FACULTY
   •      VLAN 30 – ADMIN

Each VLAN works as a separate logical network.

2. Why do we use VLAN?

LANs are used to:

   •      Separate different groups of users.
   •      Improve network security by isolating users.

Implementation / Procedure Using GUI

Step 1: Add Devices
Open Cisco Packet Tracer.

Add:

   •      1 × Cisco 2960 Switch
   •      6 × PCs

We will keep 2 PCs in each VLAN.

VLAN 10         VLAN 20       VLAN 30
STUDENTS        FACULTY       ADMIN
PC0 PC1         PC2 PC3       PC4 PC5


Step 2: Connect PCs to Switch
Select:

Connections (⚡) → Copper Straight-Through

Wait for the connections to become green.

--- Page 2 ---

Step 3: Configure IP Addresses
Go to:

PC → Desktop → IP Configuration

VLAN 10 – STUDENTS

PC0

IP Address: 192.168.10.1
Subnet Mask: 255.255.255.0

PC1

IP Address: 192.168.10.2
Subnet Mask: 255.255.255.0

VLAN 20 – FACULTY

PC2

IP Address: 192.168.20.1
Subnet Mask: 255.255.255.0

PC3

IP Address: 192.168.20.2
Subnet Mask: 255.255.255.0

VLAN 30 – ADMIN

PC4

IP Address: 192.168.30.1
Subnet Mask: 255.255.255.0

PC5

IP Address: 192.168.30.2
Subnet Mask: 255.255.255.0

Default Gateway: Leave it blank because we are not configuring inter-VLAN routing.




Step 4: Create VLAN 10
Click:

Switch → Config → VLAN Database

--- Page 3 ---

Enter:

VLAN Number: 10
VLAN Name: STUDENTS

Click Add.




Step 5: Create VLAN 20
In the same VLAN Database, enter:

VLAN Number: 20
VLAN Name: FACULTY

Click Add.




Step 6: Create VLAN 30
Enter:

VLAN Number: 30
VLAN Name: ADMIN

Click Add.

Now three VLANs have been created.




Step 7: Assign Ports to VLAN 10
Go to:

Switch → Config → Interfaces → FastEthernet0/1

Set:

Port Status: On
VLAN: 10

Then select FastEthernet0/2 and set:

Port Status: On
VLAN: 10

Therefore:

PC0 → Fa0/1 → VLAN 10

--- Page 4 ---

PC1 → Fa0/2 → VLAN 10


Step 8: Assign Ports to VLAN 20
Select:

FastEthernet0/3

Set:

Port Status: On
VLAN: 20

Select FastEthernet0/4 and set:

Port Status: On
VLAN: 20

Therefore:

PC2 → Fa0/3 → VLAN 20
PC3 → Fa0/4 → VLAN 20


Step 9: Assign Ports to VLAN 30
Select:

FastEthernet0/5

Set:

Port Status: On
VLAN: 30

Select FastEthernet0/6 and set:

Port Status: On
VLAN: 30

Therefore:

PC4 → Fa0/5 → VLAN 30
PC5 → Fa0/6 → VLAN 30


Step 10: Verify Connectivity
Test VLAN 10

From PC0 → Desktop → Command Prompt:

--- Page 5 ---

ping 192.168.10.2

Expected:

Reply from 192.168.10.2

PC0 and PC1 can communicate because they are in the same VLAN.



Test VLAN 20

From PC2:

ping 192.168.20.2

Expected:

Reply from 192.168.20.2

PC2 and PC3 can communicate.



Test VLAN 30

From PC4:

ping 192.168.30.2

Expected:

Reply from 192.168.30.2

PC4 and PC5 can communicate.




Step 11: Test Communication Between Different VLANs
From PC0 (VLAN 10):

ping 192.168.20.1

Expected:

Request timed out.

Now test:

ping 192.168.30.1

Expected:

--- Page 6 ---

Request timed out.

This happens because VLAN 10, VLAN 20, and VLAN 30 are separate networks, and a normal Layer 2
switch cannot route traffic between them.
