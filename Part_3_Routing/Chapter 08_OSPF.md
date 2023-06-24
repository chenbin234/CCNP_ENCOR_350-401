# OSPF

## 1. **OSPF Fundamentals**

![image-20230624143728379](images/image-20230624143728379.png)

![image-20230624144030009](images/image-20230624144030009.png)

![image-20230624144049466](images/image-20230624144049466.png)

![image-20230624144905294](images/image-20230624144905294.png)

![image-20230624145505609](images/image-20230624145505609.png)

![image-20230624145812438](images/image-20230624145812438.png)

![image-20230624145826617](images/image-20230624145826617.png)



## 2. **OSPF Configuration**

![image-20230624150043525](images/image-20230624150043525.png)

![image-20230624150100956](images/image-20230624150100956.png)

![image-20230624151008617](images/image-20230624151008617.png)

![image-20230624151219546](images/image-20230624151219546.png)

![image-20230624151306412](images/image-20230624151306412.png)

![image-20230624151503927](images/image-20230624151503927.png)

![image-20230624151549713](images/image-20230624151549713.png)

![image-20230624151611603](images/image-20230624151611603.png)

![image-20230624151631433](images/image-20230624151631433.png)

#### **Confirmation of Interfaces**

It is a good practice to verify that the correct interfaces are running OSPF after making changes to the OSPF configuration. The command **show ip ospf interface** [**brief** | interface-id] displays the OSPF-enabled interfaces.

![image-20230624151908749](images/image-20230624151908749.png)

![image-20230624151927471](images/image-20230624151927471.png)

![image-20230624151941815](images/image-20230624151941815.png)

![image-20230624152005940](images/image-20230624152005940.png)

#### **Verification of OSPF Neighbor Adjacencies**

![image-20230624152103479](images/image-20230624152103479.png)

![image-20230624152205491](images/image-20230624152205491.png)

#### **Verification of OSPF Routes**

![image-20230624153419521](images/image-20230624153419521.png)



## 3. **Default Route Advertisement**

![image-20230624153547900](images/image-20230624153547900.png)

![image-20230624153618884](images/image-20230624153618884.png)

![image-20230624153649692](images/image-20230624153649692.png)



## 4. **Common OSPF Optimizations**

![image-20230624154007360](images/image-20230624154007360.png)

![image-20230624154218268](images/image-20230624154218268.png)

The following sections explain the DR election process and how the DR role can be assigned to specific hardware.

![image-20230624154541876](images/image-20230624154541876.png)

![image-20230624154552912](images/image-20230624154552912.png)

![image-20230624154608255](images/image-20230624154608255.png)

**Setting an interface priority to 0 removes that inter- face from the DR/BDR election immediately. Raising the priority above the default value (1) makes that interface more favorable compared to interfaces with the default value.**

![image-20230624154731687](images/image-20230624154731687.png)

![image-20230624154743153](images/image-20230624154743153.png)

![image-20230624154758787](images/image-20230624154758787.png)

#### **OSPF Network Types**

![image-20230624154901804](images/image-20230624154901804.png)

**Broadcast**

The OSPF network type is set to broadcast by default for Ethernet interfaces. A DR is required for this OSPF network type because of the possibility that multiple nodes can exist on a segment, and LSA flooding needs to be controlled. The hello timer defaults to 10 seconds, as defined in RFC 2328.

The interface parameter command **ip ospf network broadcast** overrides the automatically configured setting and statically sets an interface as an OSPF broadcast network type.

**Point-to-Point Networks**

A network circuit that allows only two devices to communicate is considered a point-to- point (P2P) network. Because of the nature of the medium, point-to-point networks do not use Address Resolution Protocol (ARP), and broadcast traffic does not become the limiting factor.

The OSPF network type is set to point-to-point by default for serial interfaces (HDLC or PPP encapsulation), generic routing encapsulation (GRE) tunnels, and point-to-point Frame Relay subinterfaces. Only two nodes can exist on this type of network medium, so OSPF does not waste CPU cycles on DR functionality. The hello timer is set to 10 seconds on OSPF point-to-point network types.

![image-20230624161620520](images/image-20230624161620520.png)

![image-20230624161644704](images/image-20230624161644704.png)

**Loopback Networks**

The OSPF network type loopback is enabled by default for loopback interfaces and can be used only on loopback interfaces. 

The OSPF loopback network type states that the IP address is always advertised with a /32 prefix length, even if the IP address configured on the loopback interface does not have a /32 prefix length. It is possible to demonstrate this behavior by reusing Figure 8-11 and advertising a Loopback 0 interface.

![image-20230624161811200](images/image-20230624161811200.png)

![image-20230624161822395](images/image-20230624161822395.png)

![image-20230624161900270](images/image-20230624161900270.png)

![image-20230624161916507](images/image-20230624161916507.png)
