![image-20230704102940674](images/image-20230704102940674.png)

![image-20230704104647131](images/image-20230704104647131.png)

vManager - is the controller and cisco considers it the management plane 

vSmart - is the control plane. 

vEdge is the data plane. 

vBond is the orchestrator plane, and according to cisco it authenticates the vSmart controllers and the SD-WAN routers and orchestrates connectivity between them. 

It is the only device that must have a public IP address so that all SD-WAN devices in the network can connect to it. A vBond orchestrator is an SD-WAN router that only performs vBond orchestrator functions.

![image-20230704104940053](images/image-20230704104940053.png)

SD-Access Fabric Roles and Terminology Control Plane Node, Border Node, Edge Node, and other Fabric elements.

![image-20230704105346421](images/image-20230704105346421.png)

![image-20230704110400922](images/image-20230704110400922.png)

![image-20230704110946050](images/image-20230704110946050.png)

"Punt" is often used to describe the action of moving a packet from the fast path (CEF) to the route processor for handling. Cisco Express Forwarding (CEF) provides the ability to switch packets through a device in a very quick and efficient way while also keeping the load on the router‘s processor low. 

CEF is made up of two different main components: the Forwarding Information Base (FIB) and the Adjacency Table. Process switching is the slowest switching methods (compared to fast switching and Cisco Express Forwarding) because it must find a destination in the routing table. 

Process switching must also construct a new Layer 2 frame header for every packet. With process switching, when a packet comes in, the scheduler calls a process that examines the routing table, determines which interface the packet should be switched to and then switches the packet. The problem is, this happens for the every packet.

![image-20230704111722580](images/image-20230704111722580.png)

![image-20230704154421302](images/image-20230704154421302.png)

- onboard vEdge nodes into the SD-WAN fabric (vBond) 

- gather telemetry data from vEdge routers (vAnalytics) 

- distribute security information for tunnel establishment between vEdge routers (vSmart) - 
- manage, maintain, and gather configuration and status for nodes within the SD-WAN fabric (vManage)

![image-20230704154920081](images/image-20230704154920081.png)

![image-20230704155424243](images/image-20230704155424243.png)

![image-20230704160209241](images/image-20230704160209241.png)

![image-20230704160456534](images/image-20230704160456534.png)

![image-20230704161017583](images/image-20230704161017583.png)

![image-20230704184951732](images/image-20230704184951732.png)

![image-20230704185819600](images/image-20230704185819600.png)

![image-20230704190415938](images/image-20230704190415938.png)

![image-20230704190558438](images/image-20230704190558438.png)

![image-20230704190958782](images/image-20230704190958782.png)

![image-20230704192252065](images/image-20230704192252065.png)

![image-20230704192308654](images/image-20230704192308654.png)

![image-20230704194339664](images/image-20230704194339664.png)

![image-20230704194411115](images/image-20230704194411115.png)

![image-20230705111015731](images/image-20230705111015731.png)

![image-20230705111029935](images/image-20230705111029935.png)

![image-20230705112140246](images/image-20230705112140246.png)

![image-20230705112523269](images/image-20230705112523269.png)

![image-20230705125711608](images/image-20230705125711608.png)

![image-20230705130217350](images/image-20230705130217350.png)

![image-20230705130500884](images/image-20230705130500884.png)

![image-20230705130759512](images/image-20230705130759512.png)

![image-20230705131916968](images/image-20230705131916968.png)

![image-20230705134621749](images/image-20230705134621749.png)

![image-20230705135432720](images/image-20230705135432720.png)

Q89

![image-20230705140732651](images/image-20230705140732651.png)

![image-20230705154848971](images/image-20230705154848971.png)

![image-20230705203017511](images/image-20230705203017511.png)

Q168

![image-20230705215400831](images/image-20230705215400831.png)

![image-20230705222601102](images/image-20230705222601102.png)

Q139

![image-20230705223939557](images/image-20230705223939557.png)

![image-20230705225911877](images/image-20230705225911877.png)

Q119

![image-20230705231914139](images/image-20230705231914139.png)

![image-20230706092937707](images/image-20230706092937707.png)

![image-20230706093352464](images/image-20230706093352464.png)

![image-20230706093741259](images/image-20230706093741259.png)

![image-20230706094335431](images/image-20230706094335431.png)

![image-20230706094419322](images/image-20230706094419322.png)

![image-20230706101204186](images/image-20230706101204186.png)

![image-20230706105246088](images/image-20230706105246088.png)

![image-20230706110419120](images/image-20230706110419120.png)

![image-20230706110752966](images/image-20230706110752966.png)

![image-20230706111043832](images/image-20230706111043832.png)

![image-20230706140040895](images/image-20230706140040895.png)

![image-20230706140810493](images/image-20230706140810493.png)

![image-20230706141257037](images/image-20230706141257037.png)

Q259

![image-20230706144621393](images/image-20230706144621393.png)

![image-20230706144708669](images/image-20230706144708669.png)

![image-20230706145301992](images/image-20230706145301992.png)

Q253

![image-20230706153305987](images/image-20230706153305987.png)

![image-20230706153500827](images/image-20230706153500827.png)

![image-20230706153620340](images/image-20230706153620340.png)

![image-20230706154028773](images/image-20230706154028773.png)

![image-20230706160350590](images/image-20230706160350590.png)

![image-20230706162650626](images/image-20230706162650626.png)

![image-20230706165758086](images/image-20230706165758086.png)

![image-20230707120837811](images/image-20230707120837811.png)

![image-20230707121444968](images/image-20230707121444968.png)

![image-20230707123842532](images/image-20230707123842532.png)

![image-20230707125607144](images/image-20230707125607144.png)

Q381

Q380

Q360

![image-20230707152641468](images/image-20230707152641468.png)

![image-20230707154535506](images/image-20230707154535506.png)

![image-20230707160601947](images/image-20230707160601947.png)

![image-20230707161603358](images/image-20230707161603358.png)

![image-20230707162231919](images/image-20230707162231919.png)

![image-20230707165737624](images/image-20230707165737624.png)

![image-20230707171026865](images/image-20230707171026865.png)

![image-20230707172042982](images/image-20230707172042982.png)

![image-20230707172322318](images/image-20230707172322318.png)

![image-20230707174545186](images/image-20230707174545186.png)

  ![image-20230707174842491](images/image-20230707174842491.png)

![image-20230707175045020](images/image-20230707175045020.png)

![image-20230707175951371](images/image-20230707175951371.png)

![image-20230708091834341](images/image-20230708091834341.png)

![image-20230708091919786](images/image-20230708091919786.png)

![image-20230708092603729](images/image-20230708092603729.png)

![image-20230708092732087](images/image-20230708092732087.png)

![image-20230708092906871](images/image-20230708092906871.png)

![image-20230708093148122](images/image-20230708093148122.png)

![image-20230708093312941](images/image-20230708093312941.png)

![image-20230708094409217](images/image-20230708094409217.png)

![image-20230708094735756](images/image-20230708094735756.png)

![image-20230708095824318](images/image-20230708095824318.png)

![image-20230708100729737](images/image-20230708100729737.png)

Q463

Q461

![image-20230708103626440](images/image-20230708103626440.png)

![image-20230708103807677](images/image-20230708103807677.png)

![image-20230708104119787](images/image-20230708104119787.png)

![image-20230708104610928](images/image-20230708104610928.png)

![image-20230708105237945](images/image-20230708105237945.png)

![image-20230708105625735](images/image-20230708105625735.png)

![image-20230708110705142](images/image-20230708110705142.png)

![image-20230708113706187](images/image-20230708113706187.png)

Q435

![image-20230708154834411](images/image-20230708154834411.png)

Q428

![image-20230708160705260](images/image-20230708160705260.png)

![image-20230708161809863](images/image-20230708161809863.png)

![image-20230708161901678](images/image-20230708161901678.png)

![image-20230708164327166](images/image-20230708164327166.png)

![image-20230708165247136](images/image-20230708165247136.png)

![image-20230708221901379](images/image-20230708221901379.png)

![image-20230708222139834](images/image-20230708222139834.png)

![image-20230708223014121](images/image-20230708223014121.png)

Q582

![image-20230708232002081](images/image-20230708232002081.png)

![image-20230708233121653](images/image-20230708233121653.png)

Q575

![image-20230709152943899](images/image-20230709152943899.png)

![image-20230709154334518](images/image-20230709154334518.png)

Q558

Q556

![image-20230709162627949](images/image-20230709162627949.png)

Q553

![image-20230709163743017](images/image-20230709163743017.png)

![image-20230709170145892](images/image-20230709170145892.png)

![image-20230709170749780](images/image-20230709170749780.png)

![image-20230709171219157](images/image-20230709171219157.png)

Q531

![image-20230709175757524](images/image-20230709175757524.png)

![image-20230709175957321](images/image-20230709175957321.png)

![image-20230709180842280](images/image-20230709180842280.png)

Q520

![image-20230709181613818](images/image-20230709181613818.png)

Q518

![image-20230709183946594](images/image-20230709183946594.png)

![image-20230709184256269](images/image-20230709184256269.png)

![image-20230709184504144](images/image-20230709184504144.png)

![image-20230709213943672](images/image-20230709213943672.png)

![image-20230709214637720](images/image-20230709214637720.png)

![image-20230709214750167](images/image-20230709214750167.png)

![image-20230709215112991](images/image-20230709215112991.png)

![image-20230709215536643](images/image-20230709215536643.png)

![image-20230709220030024](images/image-20230709220030024.png)

![image-20230709222952851](images/image-20230709222952851.png)

Q677

![image-20230709224456181](images/image-20230709224456181.png)

![image-20230709225225304](images/image-20230709225225304.png)

![image-20230709225637264](images/image-20230709225637264.png)

![image-20230709230356307](images/image-20230709230356307.png)

![image-20230709230447901](images/image-20230709230447901.png)

![image-20230709230604386](images/image-20230709230604386.png)

![image-20230709230842470](images/image-20230709230842470.png)

![image-20230709231022766](images/image-20230709231022766.png)

![image-20230710090154289](images/image-20230710090154289.png)

![image-20230710090557865](images/image-20230710090557865.png)

![image-20230710090659020](images/image-20230710090659020.png)

![image-20230710090906736](images/image-20230710090906736.png)

![image-20230710091022802](images/image-20230710091022802.png)

![image-20230710091330403](images/image-20230710091330403.png)

![image-20230710091530574](images/image-20230710091530574.png)

![image-20230710091719594](images/image-20230710091719594.png)

![image-20230710091933288](images/image-20230710091933288.png)

![image-20230710092047041](images/image-20230710092047041.png)

![image-20230710092116133](images/image-20230710092116133.png)

![image-20230710092803113](images/image-20230710092803113.png)

![image-20230710093004912](images/image-20230710093004912.png)

![image-20230710093722782](images/image-20230710093722782.png)

![image-20230710094107988](images/image-20230710094107988.png)

![image-20230710094232195](images/image-20230710094232195.png)

![image-20230710094854482](images/image-20230710094854482.png)

![image-20230710095156142](images/image-20230710095156142.png)

![image-20230710095824130](images/image-20230710095824130.png)

![image-20230710100034989](images/image-20230710100034989.png)

Q611

Q609

![image-20230710102550376](images/image-20230710102550376.png)

Q603

![image-20230710103324674](images/image-20230710103324674.png)

![image-20230710111258615](images/image-20230710111258615.png)

![image-20230710111627446](images/image-20230710111627446.png)

![image-20230710112224088](images/image-20230710112224088.png)

Q714

Q715

![image-20230710113926677](images/image-20230710113926677.png)

![image-20230710114023713](images/image-20230710114023713.png)

Q719

Q722

![image-20230710132334405](images/image-20230710132334405.png)

Q727

![image-20230710133640947](images/image-20230710133640947.png)

![image-20230710134445719](images/image-20230710134445719.png)

Q743

![image-20230710143025664](images/image-20230710143025664.png)

![image-20230710143701848](images/image-20230710143701848.png)

![image-20230710144141449](images/image-20230710144141449.png)

![image-20230710144721861](images/image-20230710144721861.png)

![image-20230710144901254](images/image-20230710144901254.png)

Q767

![image-20230710145215239](images/image-20230710145215239.png)

![image-20230710145416699](images/image-20230710145416699.png)

## LAB 744 / 745 / 746 / 747 / 751 / 752 / 754 /

 

Q751

```shell
event manager applet int_loopback_Shutdown
event syslog pattern "Interface Loopback0, changed state to administratively down"
action 1.0 cli command "enable"
action 1.5 cli command "config ter"
action 2.0 cli command "interface loopback0"
action 2.5 cli command "no shutdown"
action 3.0 cli command "end"
```

Q752

<img src="images/image-20230712110700944.png" alt="image-20230712110700944" style="zoom:50%;" />

1. Configure a SPAN session on SW01 using these parameters:

• Session Number: 20
• Source Interface: VLAN 99
• Traffic Direction: Transmitted Traffic
• Destination Interface: Ethernet 0/1

2. Configure the NetFlow Top Talkers feature for outbound traffic on interface E0/2 of R01 with these parameters:

• Number of Top Talkers: 50
• Sort Type: Packets
• Cache Timeout: 30 seconds

3. Configure an IP SLA operation on SW02 and start the ICMP probe with these parameters:

• Entry Number: 10
• Target IP: 1.1.1.1
• Source IP: 172.16.2.2
• Frequency: 5 seconds
• Threshold: 250 milliseconds
• Timeout: 3000 milliseconds
• Lifetime: Forever

```shell
### Task1 ### 
SW1:
config ter
monitor session 20
source vlan 99 tx
destination interface ethernet 0/1

### Task2 ###
R01:
config ter
interface eth0/2
ip flow egress
ip flow-top-talkers
top 50
sort-by packets
cache-timeout 30000

### Task3 ###
SW02:
ip sla 10
icmp-echo 1.1.1.1 source-ip 172.16.2.2
frequency 5
threshold 250
timeout 3000

ip sla schedule 10 life forever start-time now
```



Q754 GLBP

```shell
Primary Switch:

interface vlan 100
ip address 192.168.1.2 255.255.255.0
glbp 30 ip 192.168.1.254
glbp 30 priority 130
glbp 30 preempt delay minimum 35
end

Secondary Switch:

interface vlan 100 
ip address 192.168.1.3 255.255.255.0
glbp 30 ip 192.168.1.254
```

