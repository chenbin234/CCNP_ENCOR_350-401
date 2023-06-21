# **Packet Forwarding**

## 1. **Network Device Communication**

### VLAN

![image-20230621152411801](images/image-20230621152411801.png)

![image-20230621152436401](images/image-20230621152436401.png)

### Access Ports

![image-20230621152632095](images/image-20230621152632095.png)

### Trunk Ports

![image-20230621152804464](images/image-20230621152804464.png)

### MAC address

![image-20230621153357463](images/image-20230621153357463.png)

### ARP

![image-20230621153621295](images/image-20230621153621295.png)

### Packet Routing 

![image-20230621153835610](images/image-20230621153835610.png)

### IP Address Assignment

![image-20230621154033656](images/image-20230621154033656.png)



## 2. **Forwarding Architectures**

![image-20230621154453355](images/image-20230621154453355.png)

![image-20230621155013928](images/image-20230621155013928.png)

![image-20230621155443667](images/image-20230621155443667.png)

![image-20230621155459436](images/image-20230621155459436.png)

#### Centralized Vs. Distributed Forwarding Architectures

![image-20230621155832005](images/image-20230621155832005.png)

![image-20230621155942465](images/image-20230621155942465.png)

![image-20230621160120299](images/image-20230621160120299.png)

Upon receipt of an IP packet, the FIB is checked for a valid entry. If an entry is missing, it is a “glean” adjacency in CEF, which means the packet should go to the CPU because CEF is unable to handle it. Valid FIB entries continue processing by checking the adjacency table for each packet’s destination IP address. Missing adjacency entries invoke the ARP process. Once ARP is resolved, the complete CEF entry can be created.

![image-20230621160919644](images/image-20230621160919644.png)
