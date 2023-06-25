# **Advanced OSPF**

## 1.**Areas**

![image-20230624205742496](images/image-20230624205742496.png)

![image-20230624205934343](images/image-20230624205934343.png)

![image-20230624210139837](images/image-20230624210139837.png)

![image-20230624210249049](images/image-20230624210249049.png)

![image-20230624210348249](images/image-20230624210348249.png)

#### **OSPF Route Types**

![image-20230624210713225](images/image-20230624210713225.png)

![image-20230624210811064](images/image-20230624210811064.png)



## 2. **Link-State Announcements**

![image-20230624212433919](images/image-20230624212433919.png)

#### **LSA Types**

1. **LSA Type 1: Router Link**

![image-20230624230341506](images/image-20230624230341506.png)

![image-20230624230646790](images/image-20230624230646790.png)

2. **LSA Type 2: Network Link**

![image-20230624230953844](images/image-20230624230953844.png)

![image-20230624231141257](images/image-20230624231141257.png)

3. **LSA Type 3: Summary Link**

![image-20230624231326980](images/image-20230624231326980.png)



## 3. **Discontiguous Networks**

![image-20230624232315621](images/image-20230624232315621.png)

![image-20230624232426238](images/image-20230624232426238.png)

**NOTE** Real-life scenarios of discontiguous networks involve Area 0 becoming partitioned due to hardware failures. Ensuring that multiple paths exist to keep the backbone contiguous is an important factor in network design.

## 4. **OSPF Path Selection**

![image-20230624232629560](images/image-20230624232629560.png)

#### **Intra-Area Routes**

![image-20230624233001384](images/image-20230624233001384.png)

<img src="images/image-20230624233020813.png" alt="image-20230624233020813" style="zoom:67%;" />

#### **Interarea Routes**

![image-20230624233140234](images/image-20230624233140234.png)

<img src="images/image-20230624233158337.png" alt="image-20230624233158337" style="zoom:67%;" />



## 5. **Summarization of Routes**

![image-20230624233827785](images/image-20230624233827785.png)

<img src="images/image-20230624233907978.png" alt="image-20230624233907978" style="zoom:67%;" />

![image-20230624234212270](images/image-20230624234212270.png)

![image-20230624234235374](images/image-20230624234235374.png)

![image-20230624234330277](images/image-20230624234330277.png)

![image-20230624234351563](images/image-20230624234351563.png)

![image-20230624234459732](images/image-20230624234459732.png)

![image-20230624234525176](images/image-20230624234525176.png)

## 6. **Route Filtering**

#### **Filtering with Summarization**

One of the easiest methodologies for filtering routes is to use the **not-advertise** keyword during prefix summarization. Using this keyword prevents creation of any type 3 LSAs for any networks in that range, thus making the subordinate routes visible only within the area where the route originates.

The full command structure is **area** area-id **range** network subnet-mask **not-advertise** under the OSPF process.

![image-20230625140757497](images/image-20230625140757497.png)

#### **Area Filtering**

![image-20230625141054775](images/image-20230625141054775.png)

![image-20230625141119587](images/image-20230625141119587.png)

![image-20230625141554008](images/image-20230625141554008.png)

![image-20230625141612424](images/image-20230625141612424.png)

#### **Local OSPF Filtering**

![image-20230625141826154](images/image-20230625141826154.png)

![image-20230625142143994](images/image-20230625142143994.png)

![image-20230625142201795](images/image-20230625142201795.png)
