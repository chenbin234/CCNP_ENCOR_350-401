# **Understanding Wireless Roaming and Location Services**

## 1. **Roaming Overview**

#### **Roaming Between Autonomous APs**

![image-20230701093318302](images/image-20230701093318302.png)

![image-20230701093334032](images/image-20230701093334032.png)



#### **Intracontroller Roaming**

In a Cisco wireless network, lightweight APs are bound to a wireless LAN controller through CAPWAP tunnels. The roaming process is similar to that of autonomous APs; clients must still reassociate to new APs as they move about. The only real difference is that the controller handles the roaming process, rather than the APs, because of the split-MAC architecture.

![image-20230701093634770](images/image-20230701093634770.png)

![image-20230701093757734](images/image-20230701093757734.png)

Cisco controllers offer three techniques to minimize the time and effort spent on key exchanges during roams:

![image-20230701094011459](images/image-20230701094011459.png)



## 2. **Roaming Between Centralized Controllers**

The following sections cover intercontroller roaming, mobility groups, and the mechanisms used to coordinate roaming.

### **2.1 Layer 2 Roaming**

![image-20230701094319473](images/image-20230701094319473.png)

![image-20230701094338837](images/image-20230701094338837.png)

![image-20230701094450588](images/image-20230701094450588.png)

### 2.2 **Layer 3 Roaming**

 When a client initi- ates an intercontroller roam, the two controllers involved can compare the VLAN numbers that are assigned to their respective WLAN interfaces. If the VLAN IDs are the same, nothing special needs to happen; the client undergoes a Layer 2 intercontroller roam and can continue to use its original IP address on the new controller. If the two VLAN IDs differ, the controllers arrange a Layer 3 roam (also known as a local-to-foreign roam) that will allow the client to keep using its IP address.

![image-20230701110336803](images/image-20230701110336803.png)

![image-20230701110400439](images/image-20230701110400439.png)

![image-20230701110516871](images/image-20230701110516871.png)

![image-20230701110534214](images/image-20230701110534214.png)



### 2.3 **Scaling Mobility with Mobility Groups**

![image-20230701110752826](images/image-20230701110752826.png)

![image-20230701110910760](images/image-20230701110910760.png)



## 3. **Locating Devices in a Wireless Network**

![image-20230701111447173](images/image-20230701111447173.png)

![image-20230701112100203](images/image-20230701112100203.png)

![image-20230701112114530](images/image-20230701112114530.png)

