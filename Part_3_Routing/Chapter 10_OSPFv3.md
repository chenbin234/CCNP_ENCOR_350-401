# **OSPFv3**

## 1. **OSPFv3 Fundamentals**

![image-20230625172709834](images/image-20230625172709834.png)

![image-20230625172724160](images/image-20230625172724160.png)

#### **OSPFv3 Link-State Advertisement**

OSPFv3 packets use protocol ID 89, and routers communicate with each other using the local interface’s IPv6 link-local address. 

IP address information is advertised independently by two new LSA types:

- Intra-area prefix LSA
- Link-local LSA

Table 10-2 provides a brief description of each OSPFv3 LSA type.

![image-20230625173846669](images/image-20230625173846669.png)

#### **OSPFv3 Communication**

![image-20230625173935340](images/image-20230625173935340.png)

OSPFv3 uses the same five packet types and logic as OSPFv2. Table 10-3 shows the name, address, and purpose of each of the five packets types.

![image-20230625174027747](images/image-20230625174027747.png)



## 2. **OSPFv3 Configuration**

![image-20230625174235718](images/image-20230625174235718.png)

![image-20230625174309014](images/image-20230625174309014.png)

![image-20230625174449979](images/image-20230625174449979.png)

![image-20230625174622423](images/image-20230625174622423.png)

![image-20230625174542138](images/image-20230625174542138.png)

![image-20230625174648817](images/image-20230625174648817.png)



## 3. **OSPFv3 Verification**

![image-20230625175338784](images/image-20230625175338784.png)

![image-20230625175435671](images/image-20230625175435671.png)

![image-20230625175459481](images/image-20230625175459481.png)

![image-20230625175513108](images/image-20230625175513108.png)

#### **Passive Interface**

![image-20230625180525136](images/image-20230625180525136.png)

#### **Summarization**

![image-20230625180848984](images/image-20230625180848984.png)

#### **Network Type**

OSPFv3 supports the same OSPF network types as OSPFv2. Example 10-11 shows that R2’s Gi0/3 interface is set as a broadcast OSPF network type and is confirmed as being in a DR state.

![image-20230625181621122](images/image-20230625181621122.png)



## 4.IPv4 Support in OSPFv3

![image-20230625181805965](images/image-20230625181805965.png)

Using the topology shown in Figure 10-1, IPv4 addressing has been placed onto R1, R2, R3, and R4 using the conventions outlined earlier. Example 10-14 demonstrates the deployment of IPv4 using the existing OSPFv3 deployment.

![image-20230625181918404](images/image-20230625181918404.png)

![image-20230625182000828](images/image-20230625182000828.png)

![image-20230625182018280](images/image-20230625182018280.png)

![image-20230625182451652](images/image-20230625182451652.png)
