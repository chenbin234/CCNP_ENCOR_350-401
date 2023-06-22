# **VLAN Trunks and EtherChannel Bundles**

<img src="images/image-20230622144617880.png" alt="image-20230622144617880" style="zoom:50%;" />

## 1. **VLAN Trunking Protocol**

Adding a VLAN might seem like a simple task, but in an environment with 100 switches, adding a VLAN required logging in to 100 switches to provision one VLAN. Thanks to VTP, switches that participate in the same VTP domain can have a VLAN created once on a VTP server and propagated to other VTP client switches in the same VTP domain.

![image-20230622145449458](images/image-20230622145449458.png)

Figure 5-1 shows a simple topology in which SW1 is the VTP server, and SW2, SW4, SW5, and SW6 are VTP clients. SW3 is in transparent mode and does not update its VLAN database as changes are propagated through the VTP domain. SW3 forwards VTP changes to SW6.

![image-20230622145644989](images/image-20230622145644989.png)

VTP supports having multiple VTP servers in a domain. These servers process updates from other VTP servers just as a client does. If a VTP domain is Version 3, the primary VTP server must be set with the executive command **vtp primary**.

### **VTP Communication**

![image-20230622150020803](images/image-20230622150020803.png)

### **VTP Configuration**

![image-20230622150051297](images/image-20230622150051297.png) 

![image-20230622150149275](images/image-20230622150149275.png)

![image-20230622150545353](images/image-20230622150545353.png)

![image-20230622150602978](images/image-20230622150602978.png)

### **VTP Verification**

![image-20230622150742743](images/image-20230622150742743.png)

![image-20230622151017739](images/image-20230622151017739.png)



## 2. **Dynamic Trunking Protocol**

![image-20230622151121339](images/image-20230622151121339.png)

![image-20230622151137843](images/image-20230622151137843.png)

A trunk link can successfully form in almost any combination of these modes **unless both ends are configured as dynamic auto.** Table 5-2 shows a matrix for successfully establishing a dynamic trunk link.

![image-20230622151316392](images/image-20230622151316392.png)

![image-20230622151352967](images/image-20230622151352967.png)

![image-20230622151414576](images/image-20230622151414576.png)

![image-20230622151427963](images/image-20230622151427963.png)

![image-20230622151540155](images/image-20230622151540155.png)

![image-20230622151617844](images/image-20230622151617844.png)



## 3. **EtherChannel Bundle**

Ideally, it would be nice to plug in a second cable and double the bandwidth between the switches. However, Spanning Tree Protocol (STP) will place one of the ports into a blocking state to prevent forwarding loops, as shown in Figure 5-2.

<img src="images/image-20230622151940738.png" alt="image-20230622151940738" style="zoom:50%;" />

Fortunately, the physical links can be aggregated into a logical link called an EtherChannel bundle. The industry-based term for an EtherChannel bundle is EtherChannel (for short), or port channel, which is defined in the IEEE 802.3AD link aggregation specification. The physical interfaces that are used to assemble the logical EtherChannel are called member interfaces. STP operates on a logical link and not on a physical link. The logical link would then have the bandwidth of any active member interfaces, and it would be load balanced across all the links. EtherChannels can be used for either Layer 2 (access or trunk) or Layer 3 (routed) forwarding.

![image-20230622152347842](images/image-20230622152347842.png)

### **Dynamic Link Aggregation Protocols**

Two common link aggregation protocols are Link Aggregation Control Protocol (LACP) and Port Aggregation Protocol (PAgP). PAgP is Cisco proprietary and was developed first, and then LACP was created as an open industry standard. All the member links must participate in the same protocol on the local and remote switches.

![image-20230622153347902](images/image-20230622153347902.png)

![image-20230622153408453](images/image-20230622153408453.png)

![image-20230622153424415](images/image-20230622153424415.png)

![image-20230622153701906](images/image-20230622153701906.png)

![image-20230622153828280](images/image-20230622153828280.png)

![image-20230622153842188](images/image-20230622153842188.png)

#### **Verifying Port-Channel Status**

![image-20230622153909901](images/image-20230622153909901.png)

![image-20230622153922528](images/image-20230622153922528.png)

![image-20230622154155707](images/image-20230622154155707.png)

![image-20230622154209402](images/image-20230622154209402.png)

![image-20230622154235081](images/image-20230622154235081.png)

#### **Viewing EtherChannel Neighbors**

![image-20230622154308737](images/image-20230622154308737.png)

![image-20230622154330341](images/image-20230622154330341.png)

![image-20230622154343175](images/image-20230622154343175.png)

#### **Verifying EtherChannel Packets**

![image-20230622154707273](images/image-20230622154707273.png)

#### **Advanced LACP Configuration Options**

**LACP Fast**

…

![image-20230622155027313](images/image-20230622155027313.png)

![image-20230622155122623](images/image-20230622155122623.png)

![image-20230622155216929](images/image-20230622155216929.png)

![image-20230622155228480](images/image-20230622155228480.png)

![image-20230622155356646](images/image-20230622155356646.png)

#### **Troubleshooting EtherChannel Bundles**

It is important to remember that a port channel is a logical interface, so all the member interfaces must have the same characteristics. If they do not, problems will occur.

#### **Load Balancing Traffic with EtherChannel Bundles**

![image-20230622155507869](images/image-20230622155507869.png)![image-20230622155521924](images/image-20230622155521924.png)
