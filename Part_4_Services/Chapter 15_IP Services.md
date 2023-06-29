# **IP Services**

## 1. **Time Synchronization**

![image-20230628151948018](images/image-20230628151948018.png)

![image-20230628152153369](images/image-20230628152153369.png)

### **NTP Configuration**

![image-20230628152324236](images/image-20230628152324236.png)

![image-20230628152421309](images/image-20230628152421309.png)

![image-20230628152635666](images/image-20230628152635666.png)

![image-20230628152716808](images/image-20230628152716808.png)

In the topology shown in Figure 15-2, R4 will always use R1 for synchronizing its time because it is a stratum 1 server. If R2 crashes, as shown at the bottom of Figure 15-2, preventing R4 from reaching R1, it synchronizes with R3’s time (which may or may not be different due to time drift) and turns into a stratum 4 time device. When R2 recovers, R4 synchronizes with R1 and becomes a stratum 2 device again.

![image-20230628153407952](images/image-20230628153407952.png)

![image-20230628153419866](images/image-20230628153419866.png)



## 2. **First-Hop Redundancy Protocol**

![image-20230628153606530](images/image-20230628153606530.png)

#### **Object Tracking**

Object tracking offers a flexible and customizable mechanism for linking with FHRPs and other routing components (for example, conditional installation of a static route). With this feature, users can track specific objects in the network and take necessary action when any object’s state change affects network traffic.

![image-20230628155924722](images/image-20230628155924722.png)

![image-20230628160009092](images/image-20230628160009092.png)

![image-20230628160100365](images/image-20230628160100365.png)

### 2.1 **Hot Standby Router Protocol**

![image-20230628160203592](images/image-20230628160203592.png)

**NOTE** HSRP does not support preemption by default, so when a router with lower priority becomes active, it does not automatically transfer its active status to a superior router.

![image-20230628160450966](images/image-20230628160450966.png)

![image-20230628160543922](images/image-20230628160543922.png)

![image-20230628160556161](images/image-20230628160556161.png)

![image-20230628160648459](images/image-20230628160648459.png)

![image-20230628160741411](images/image-20230628160741411.png)

![image-20230628161649225](images/image-20230628161649225.png)

![image-20230628161754930](images/image-20230628161754930.png)

![image-20230628161829796](images/image-20230628161829796.png)

### 2.2 **Virtual Router Redundancy Protocol**

![image-20230628162008003](images/image-20230628162008003.png)

![image-20230628162109788](images/image-20230628162109788.png)

![image-20230628162143479](images/image-20230628162143479.png)

![image-20230628162206223](images/image-20230628162206223.png)

![image-20230628162313991](images/image-20230628162313991.png)

### 2.3 **Global Load Balancing Protocol**

![image-20230629124136076](images/image-20230629124136076.png)

![image-20230629124940455](images/image-20230629124940455.png)

![image-20230629125503873](images/image-20230629125503873.png)

![image-20230629125803505](images/image-20230629125803505.png)

![image-20230629130026012](images/image-20230629130026012.png)

![image-20230629130044337](images/image-20230629130044337.png)

![image-20230629130126470](images/image-20230629130126470.png)

![image-20230629130145608](images/image-20230629130145608.png)

![image-20230629130529005](images/image-20230629130529005.png)



## 3. **Network Address Translation (NAT)**

![image-20230629130833122](images/image-20230629130833122.png)

![image-20230629130920546](images/image-20230629130920546.png)

![image-20230629130939428](images/image-20230629130939428.png)

![image-20230629131337877](images/image-20230629131337877.png)

![image-20230629131403585](images/image-20230629131403585.png)

![image-20230629132207893](images/image-20230629132207893.png)

### 3.1 **Static NAT**

![image-20230629132635491](images/image-20230629132635491.png)

![image-20230629132714375](images/image-20230629132714375.png)

![image-20230629132728505](images/image-20230629132728505.png)

![image-20230629132828502](images/image-20230629132828502.png)

![image-20230629134658516](images/image-20230629134658516.png)

![image-20230629135045293](images/image-20230629135045293.png)

![image-20230629135147045](images/image-20230629135147045.png)

![image-20230629135256504](images/image-20230629135256504.png)

![image-20230629135317741](images/image-20230629135317741.png)

![image-20230629135520455](images/image-20230629135520455.png)

![image-20230629135705726](images/image-20230629135705726.png)

![image-20230629135722441](images/image-20230629135722441.png)

![image-20230629135737704](images/image-20230629135737704.png)

![image-20230629135926333](images/image-20230629135926333.png)

![image-20230629135956460](images/image-20230629135956460.png)

![image-20230629140527793](images/image-20230629140527793.png)

![image-20230629140841409](images/image-20230629140841409.png)

![image-20230629140859340](images/image-20230629140859340.png)

![image-20230629141018014](images/image-20230629141018014.png)

![image-20230629141055986](images/image-20230629141055986.png)

![image-20230629141119916](images/image-20230629141119916.png)

![image-20230629141201013](images/image-20230629141201013.png)

![image-20230629141234027](images/image-20230629141234027.png)

![image-20230629141303500](images/image-20230629141303500.png)

![image-20230629141354671](images/image-20230629141354671.png)
