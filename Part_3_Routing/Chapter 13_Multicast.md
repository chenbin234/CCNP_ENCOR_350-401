# **Multicast**

## 1. **Multicast Fundamentals**

![image-20230627220011595](images/image-20230627220011595.png)

Multicast communication is a technology that optimizes network bandwidth utilization and conserves system resources. It relies on **Internet Group Management Protocol (IGMP)** for its operation in Layer 2 networks and **Protocol Independent Multicast (PIM)** for its operation in Layer 3 networks.

![image-20230627220234057](images/image-20230627220234057.png)

![image-20230627220534928](images/image-20230627220534928.png)

## 2. **Multicast Addressing**

![image-20230627220854195](images/image-20230627220854195.png)

![image-20230627221115308](images/image-20230627221115308.png)

![image-20230627221143665](images/image-20230627221143665.png)

![image-20230627221710818](images/image-20230627221710818.png)

![image-20230627221742341](images/image-20230627221742341.png)

![image-20230627222056908](images/image-20230627222056908.png)

![image-20230627222112990](images/image-20230627222112990.png)



## 3. **Internet Group Management Protocol**

![image-20230627222647973](images/image-20230627222647973.png)

![image-20230627222925697](images/image-20230627222925697.png)

![image-20230627222946919](images/image-20230627222946919.png)

![image-20230627223153367](images/image-20230627223153367.png)

![image-20230627223539078](images/image-20230627223539078.png)

#### **IGMP Snooping**

![image-20230627224125880](images/image-20230627224125880.png)

![image-20230628091027531](images/image-20230628091027531.png)

![image-20230628091045776](images/image-20230628091045776.png)



## 4. **Protocol Independent Multicast**

![image-20230628091325390](images/image-20230628091325390.png)

![image-20230628091453684](images/image-20230628091453684.png)

![image-20230628091615911](images/image-20230628091615911.png)

![image-20230628091738768](images/image-20230628091738768.png)

![image-20230628091844105](images/image-20230628091844105.png)

![image-20230628092334526](images/image-20230628092334526.png)

![image-20230628093135141](images/image-20230628093135141.png)

![image-20230628093153367](images/image-20230628093153367.png)

![image-20230628093020505](images/image-20230628093020505.png)

#### **PIM Dense Mode**

![image-20230628094019042](images/image-20230628094019042.png)

Figure 13-15 shows the flood and prune operation of Dense Mode. The multicast traffic from the source is flooding throughout the entire network. As each router receives the multicast traffic from its upstream neighbor via its RPF interface, it forwards the multicast traffic to all its PIM-DM neighbors. This results in some traffic arriving via a non-RPF interface, as in the case of R3 receiving traffic from R2 on its non-RPF interface. Packets arriving via the non-RPF interface are discarded.

![image-20230628094232048](images/image-20230628094232048.png)

#### **PIM Sparse Mode**

![image-20230628094610817](images/image-20230628094610817.png)

**PIM Shared and Source Path Trees**

![image-20230628095214211](images/image-20230628095214211.png)

![image-20230628095229485](images/image-20230628095229485.png)

![image-20230628095456305](images/image-20230628095456305.png)

![image-20230628095520967](images/image-20230628095520967.png)

![image-20230628095724714](images/image-20230628095724714.png)

![image-20230628100432668](images/image-20230628100432668.png)

![image-20230628101517380](images/image-20230628101517380.png)

![image-20230628101654620](images/image-20230628101654620.png)

![image-20230628101903951](images/image-20230628101903951.png)



## 5. **Rendezvous Points**

![image-20230628102414030](images/image-20230628102414030.png)

![image-20230628102733492](images/image-20230628102733492.png)

![image-20230628102748457](images/image-20230628102748457.png)

![image-20230628102829189](images/image-20230628102829189.png)

![image-20230628102910605](images/image-20230628102910605.png)

![image-20230628103033513](images/image-20230628103033513.png)

![image-20230628103326156](images/image-20230628103326156.png)