# **Overlay Tunnels**

Examples of overlay tunneling technologies include the following:

- Generic Routing Encapsulation (GRE)
- IP Security (IPsec)
- Locator ID/Separation Protocol (LISP)
- Virtual Extensible LAN (VXLAN)
- Multiprotocol Label Switching (MPLS)

![image-20230629145102702](images/image-20230629145102702.png)

![image-20230629145034154](images/image-20230629145034154.png)

## 1. **Generic Routing Encapsulation (GRE) Tunnels**

![image-20230629145942581](images/image-20230629145942581.png)

### **GRE Tunnel Configuration**

![image-20230629150159437](images/image-20230629150159437.png)

![image-20230629150217853](images/image-20230629150217853.png)

![image-20230629150506715](images/image-20230629150506715.png)

![image-20230629150531835](images/image-20230629150531835.png)

![image-20230629150632489](images/image-20230629150632489.png)

![image-20230629150648318](images/image-20230629150648318.png)

#### **GRE Configuration Example**

![image-20230629150845302](images/image-20230629150845302.png)

![image-20230629150901367](images/image-20230629150901367.png)

![image-20230629151328299](images/image-20230629151328299.png)

![image-20230629151407861](images/image-20230629151407861.png)

![image-20230629151433040](images/image-20230629151433040.png)

![image-20230629151510801](images/image-20230629151510801.png)

#### **Problems with Overlay Networks: Recursive Routing**



## 2. **IPsec Fundamentals**

![image-20230629151843973](images/image-20230629151843973.png)

![image-20230629151907302](images/image-20230629151907302.png)

![image-20230629151939589](images/image-20230629151939589.png)

![image-20230629152000020](images/image-20230629152000020.png)

![image-20230629155151662](images/image-20230629155151662.png)

![image-20230629155332778](images/image-20230629155332778.png)

![image-20230629155357670](images/image-20230629155357670.png)

![image-20230629155418307](images/image-20230629155418307.png)

![image-20230629155531467](images/image-20230629155531467.png)

![image-20230629155546768](images/image-20230629155546768.png)

![image-20230629155747958](images/image-20230629155747958.png)

![image-20230629155847894](images/image-20230629155847894.png)

![image-20230629155906918](images/image-20230629155906918.png)

![image-20230629155922920](images/image-20230629155922920.png)

![image-20230629160019792](images/image-20230629160019792.png)

<img src="images/image-20230629160034752.png" alt="image-20230629160034752" style="zoom:67%;" />

### **IPsec VPNs**

![image-20230629160154697](images/image-20230629160154697.png)

![image-20230629160327020](images/image-20230629160327020.png)

![image-20230629160345636](images/image-20230629160345636.png)

![image-20230629160835961](images/image-20230629160835961.png)

![image-20230629160853019](images/image-20230629160853019.png)

### **Site-to-Site IPsec Configuration**

![image-20230629161644396](images/image-20230629161644396.png)

![image-20230629161949579](images/image-20230629161949579.png)

#### Site-to-Site GRE over IPsec

![image-20230629162827369](images/image-20230629162827369.png)

![image-20230629162850732](images/image-20230629162850732.png)

![image-20230629163245137](images/image-20230629163245137.png)

![image-20230629163305052](images/image-20230629163305052.png)



![image-20230629163332495](images/image-20230629163332495.png)

![image-20230629163354847](images/image-20230629163354847.png)



![image-20230629164704314](images/image-20230629164704314.png)



## 3. **Cisco Location/ID Separation Protocol (LISP)**

![image-20230629165108811](images/image-20230629165108811.png)

![image-20230630105358061](images/image-20230630105358061.png)

![image-20230630105703897](images/image-20230630105703897.png)

![image-20230630105721224](images/image-20230630105721224.png)

#### **LISP Architecture and Protocols**

![image-20230630110027271](images/image-20230630110027271.png)

![image-20230630110254483](images/image-20230630110254483.png)

#### **LISP Operation**

![image-20230630110449174](images/image-20230630110449174.png)



## 4. **Virtual Extensible Local Area Network (VXLAN)**

![image-20230630113049104](images/image-20230630113049104.png)

![image-20230630113138638](images/image-20230630113138638.png)

![image-20230630114412704](images/image-20230630114412704.png)

![image-20230630114431136](images/image-20230630114431136.png)

![image-20230630114456172](images/image-20230630114456172.png)

Devices that are not capable of supporting VXLAN and need to use traditional VLAN seg- mentation can be connected to VXLAN segments by using a VXLAN gateway. A VXLAN gateway is a VTEP device that combines a VXLAN segment and a classic VLAN segment into one common Layer 2 domain.

![image-20230630114730086](images/image-20230630114730086.png)

![image-20230630114750563](images/image-20230630114750563.png)

As illustrated in Figure 16-15, LISP encapsulation is only capable of performing IP-in-IP/ UDP encapsulation, which allows it to support Layer 3 overlays only, while VXLAN encap- sulation is capable of encapsulating the original Ethernet header to perform MAC-in-IP encapsulation, which allows it to support Layer 2 and Layer 3 overlays.
