# QoS

## 1.The Need for QoS

The following are the leading causes of quality issues:

- Lack of bandwidth
- Latency and jitter
- Packet loss

Network latency can be broken down into fixed and variable latency:

- Propagation delay (fixed)
- Serialization delay (fixed)
- Processing delay (fixed)
- Delay variation (variable)

![image-20230628111745447](images/image-20230628111745447.png)

## 2. QoS Models

![image-20230628112007862](images/image-20230628112007862.png)

![image-20230628112738100](images/image-20230628112738100.png)

![image-20230628112757926](images/image-20230628112757926.png)

![image-20230628112856258](images/image-20230628112856258.png)

## 3. Classification and Marking

This section introduces the concepts of classification and marking, explains the different marking options that are available for Layer 2 frames and Layer 3 packets, and explains where classification and marking tools should be used in a network.

![image-20230628132938375](images/image-20230628132938375.png)

![image-20230628133241700](images/image-20230628133241700.png)

![image-20230628133345895](images/image-20230628133345895.png)

#### Layer 2 Marking

![image-20230628133727163](images/image-20230628133727163.png)

![image-20230628133755197](images/image-20230628133755197.png)

**One drawback of using CoS markings is that frames lose their CoS markings when traversing a non-802.1Q link or a Layer 3 network.** For this reason, packets should be marked with other higher-layer markings whenever possible so the marking values can be preserved end-to-end. This is typically accomplished by mapping a CoS marking into another marking. For example, the CoS priority levels correspond directly to IPv4’s IP Precedence Type of Service (ToS) values so they can be mapped directly to each other.

![image-20230628133948599](images/image-20230628133948599.png)

#### Layer 3 Marking

![image-20230628134152767](images/image-20230628134152767.png)

![image-20230628134814727](images/image-20230628134814727.png)

![image-20230628134847176](images/image-20230628134847176.png)

![image-20230628134903514](images/image-20230628134903514.png)

![image-20230628134929369](images/image-20230628134929369.png)

![image-20230628135114435](images/image-20230628135114435.png)

![image-20230628135251135](images/image-20230628135251135.png)

![image-20230628135308444](images/image-20230628135308444.png)

![image-20230628140141365](images/image-20230628140141365.png)

#### **A Practical Example: Wireless QoS**

![image-20230628140418524](images/image-20230628140418524.png)



## 4. Policing and Shaping

![image-20230628140643476](images/image-20230628140643476.png)

![image-20230628140721259](images/image-20230628140721259.png)

![image-20230628141005050](images/image-20230628141005050.png)

![image-20230628141034504](images/image-20230628141034504.png)

![image-20230628141246157](images/image-20230628141246157.png)

![image-20230628141652305](images/image-20230628141652305.png)

#### Single-Rate Two-Color Markers/Policers

![image-20230628141855539](images/image-20230628141855539.png)

#### Single-Rate Three-Color Markers/Policers (srTCM)

![image-20230628142537206](images/image-20230628142537206.png)

![image-20230628142736525](images/image-20230628142736525.png)

#### Two-Rate Three-Color Markers/Policers (trTCM)

![image-20230628142831906](images/image-20230628142831906.png)



## 5. Congestion Management and Avoidance

This section explores the queuing algorithms used for congestion management as well as packet drop techniques that can be used for congestion avoidance. These tools provide a way of managing excessive traffic during periods of congestion.

![image-20230628143455489](images/image-20230628143455489.png)

![image-20230628143519349](images/image-20230628143519349.png)

The current queuing algorithms recommended for rich-media networks (and supported by MQC) combine the best features of the legacy algorithms. These algorithms provide real-time, delay-sensitive traffic bandwidth and delay guarantees while not starving other types of traffic. The recommended queuing algorithms include the following:

![image-20230628143953260](images/image-20230628143953260.png)



![image-20230628144424804](images/image-20230628144424804.png)

![image-20230628144439684](images/image-20230628144439684.png)

#### **Congestion-Avoidance Tools**

![image-20230628144644098](images/image-20230628144644098.png)