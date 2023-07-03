# **Network Device Access Control and Infrastructure Security**

## 1. **Access Control Lists (ACLs)**

![image-20230703132642961](images/image-20230703132642961.png)

![image-20230703132856284](images/image-20230703132856284.png)

![image-20230703133009928](images/image-20230703133009928.png)

### **Numbered Standard ACLs**

![image-20230703133236738](images/image-20230703133236738.png)

### **Numbered Extended ACLs**

![image-20230703133322071](images/image-20230703133322071.png)

### **Named ACLs**

Example 26-3 shows how named standard and extended ACLs are created and applied to an interface. The numbered ACLs in Examples 26-1 and 26-2 are included as a reference for easy comparison to named ACLs.

![image-20230703133433056](images/image-20230703133433056.png)

![image-20230703133445404](images/image-20230703133445404.png)

### **Port ACLs (PACLs) and VLAN ACLs (VACLs)**

Layer 2 Cisco switches support access lists that can be applied on Layer 2 ports as well as VLANs. Access lists applied on Layer 2 ports are called port access control lists (PACLs), and access lists applied to VLANs are called VLAN access control lists (VACLs).

#### PACLs

![image-20230703133747810](images/image-20230703133747810.png)

![image-20230703133802916](images/image-20230703133802916.png)



#### VACLs

![image-20230703133849290](images/image-20230703133849290.png)

![image-20230703133943130](images/image-20230703133943130.png)

![image-20230703134037317](images/image-20230703134037317.png)



## 2. **Terminal Lines and Password Protection**

![image-20230703134153782](images/image-20230703134153782.png)

![image-20230703134247613](images/image-20230703134247613.png)

![image-20230703134352686](images/image-20230703134352686.png)

#### **Password Encryption**

![image-20230703134550759](images/image-20230703134550759.png)

![image-20230703134625669](images/image-20230703134625669.png)

#### **Username and Password Authentication**

![image-20230703144333097](images/image-20230703144333097.png)

#### **Configuring Line Local Password Authentication**

![image-20230703144624397](images/image-20230703144624397.png)

![image-20230703144636309](images/image-20230703144636309.png)

#### **Configuring Line Local Username and Password Authentication**

![image-20230703144728933](images/image-20230703144728933.png)

![image-20230703144821255](images/image-20230703144821255.png)

#### **Privilege Levels and Role-Based Access Control (RBAC)**

![image-20230703144928365](images/image-20230703144928365.png)

![image-20230703145536650](images/image-20230703145536650.png)

![image-20230703145551187](images/image-20230703145551187.png)

#### **Controlling Access to vty Lines with ACLs**

![image-20230703145846683](images/image-20230703145846683.png)

![image-20230703145915932](images/image-20230703145915932.png)

![image-20230703145944691](images/image-20230703145944691.png)

![image-20230703150106697](images/image-20230703150106697.png)

![image-20230703150025768](images/image-20230703150025768.png)



#### **Enabling SSH vty Access**

![image-20230703150328990](images/image-20230703150328990.png)

![image-20230703150349538](images/image-20230703150349538.png)

![image-20230703150402421](images/image-20230703150402421.png)

![image-20230703150447497](images/image-20230703150447497.png)

![image-20230703150557249](images/image-20230703150557249.png)



## 3. **Authentication, Authorization, and Accounting (AAA)**

![image-20230703150622098](images/image-20230703150622098.png)

![image-20230703150645737](images/image-20230703150645737.png)

![image-20230703150736812](images/image-20230703150736812.png)

The following sections explain why TACACS+ is preferred for network access control while RADIUS is preferred for secure network access.

![image-20230703151851178](images/image-20230703151851178.png)

![image-20230703151921298](images/image-20230703151921298.png)

![image-20230703152127756](images/image-20230703152127756.png)

![image-20230703152237478](images/image-20230703152237478.png)

#### **Configuring AAA for Network Device Access Control**

![image-20230703152448516](images/image-20230703152448516.png)



## 4. **Zone-Based Firewall (ZBFW)**

![image-20230703152959767](images/image-20230703152959767.png)

<img src="images/image-20230703153059974.png" alt="image-20230703153059974" style="zoom:50%;" />

![image-20230703153258906](images/image-20230703153258906.png)

![image-20230703153314024](images/image-20230703153314024.png)

#### **ZBFW Configuration**



## 5. **Control Plane Policing (CoPP)**

![image-20230703154006248](images/image-20230703154006248.png)

#### **Configuring ACLs for CoPP**



#### **Configuring Class Maps for CoPP**



#### **Configuring the Policy Map for CoPP**



#### **Applying the CoPP Policy Map**



## 6. **Device Hardening**

![image-20230703155706151](images/image-20230703155706151.png)

![image-20230703155721090](images/image-20230703155721090.png)

![image-20230703155731526](images/image-20230703155731526.png)



