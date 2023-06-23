# **IP Routing Essentials**

## 1. **Routing Protocol Overview**

![image-20230623111750465](images/image-20230623111750465.png)

With the exception of BGP, the protocols in this list are designed and optimized for routing within an autonomous system and are known as Interior Gateway Protocols (IGPs). Exterior Gateway Protocols (EGPs) route between autonomous systems. BGP is an EGP protocol but can also be used within an autonomous system. If BGP exchanges routes within an autono- mous system, it is known as an interior BGP (iBGP) session. If it exchanges routes between different autonomous systems, it is known as an exterior BGP (eBGP) session.

![image-20230623112240147](images/image-20230623112240147.png)

A distance vector protocol selects paths purely based on distance. It does not account for link speeds or other factors. In Figure 6-2, the link between R1 and R7 is a serial link with only 64 Kbps of bandwidth, and all of the other links are 1 Gbps Ethernet links. RIP does not take this into consideration and forwards traffic across this link, which will result in packet loss when that link is oversubscribed.

![image-20230623112443920](images/image-20230623112443920.png)

![image-20230623112714039](images/image-20230623112714039.png)

![image-20230623112743111](images/image-20230623112743111.png)

![image-20230623112844560](images/image-20230623112844560.png)

![image-20230623112942403](images/image-20230623112942403.png)

![image-20230623113102599](images/image-20230623113102599.png)

![image-20230623113124718](images/image-20230623113124718.png)

![image-20230623113507695](images/image-20230623113507695.png)

<img src="images/image-20230623113525034.png" alt="image-20230623113525034" style="zoom: 67%;" />

## 2. **Path Selection**

![image-20230623113630237](images/image-20230623113630237.png)

**Administrative Distance**

![image-20230623113900153](images/image-20230623113900153.png)

![image-20230623113958093](images/image-20230623113958093.png)

![image-20230623114104504](images/image-20230623114104504.png)

![image-20230623114119118](images/image-20230623114119118.png)

![image-20230623114502811](images/image-20230623114502811.png)

**Metrics**

The logic for selecting the best path for a routing protocol can vary. Most IGPs prefer internally learned routes over external routes and further prioritize the path with the lowest metric.

![image-20230623115017030](images/image-20230623115017030.png)

![image-20230623115037819](images/image-20230623115037819.png)

![image-20230623115134512](images/image-20230623115134512.png)

![image-20230623115201025](images/image-20230623115201025.png)

## 3. **Static Routing**

![image-20230623115354070](images/image-20230623115354070.png)

![image-20230623120853891](images/image-20230623120853891.png)

![image-20230623120913180](images/image-20230623120913180.png)

![image-20230623121101542](images/image-20230623121101542.png)

![image-20230623121136186](images/image-20230623121136186.png)

![image-20230623121315110](images/image-20230623121315110.png)

![image-20230623121334403](images/image-20230623121334403.png)

![image-20230623121622839](images/image-20230623121622839.png)

![image-20230623121820220](images/image-20230623121820220.png)

![image-20230623121949769](images/image-20230623121949769.png)

![image-20230623122028617](images/image-20230623122028617.png)

![image-20230623140118727](images/image-20230623140118727.png)

![image-20230623140306085](images/image-20230623140306085.png)

![image-20230623140553777](images/image-20230623140553777.png)

![image-20230623140642308](images/image-20230623140642308.png)

![image-20230623140655575](images/image-20230623140655575.png)

## 4. **Virtual Routing and Forwarding**

Virtual routing and forwarding (VRF) is a technology that creates separate virtual routers on a physical router. Router interfaces, routing tables, and forwarding tables are completely isolated between VRFs, preventing traffic from one VRF from forwarding into another VRF. All router interfaces belong to the global VRF until they are specifically assigned to a user-defined VRF. The global VRF is identical to the regular routing table of non-VRF routers.

<img src="images/image-20230623140950018.png" alt="image-20230623140950018" style="zoom:67%;" />

![image-20230623141140386](images/image-20230623141140386.png)

 ![image-20230623141201095](images/image-20230623141201095.png)

![image-20230623141214062](images/image-20230623141214062.png)
