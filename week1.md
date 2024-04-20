# X-Ops-2024
## Week 1
#### วิธีการเข้าสายLAN (terminate utp cable)
 -การเข้าสายLANมี2แบบ ได้เเก่  
 
1.การเข้าสายแบบตรง จะใช้สำหรับการเชื่อมต่อระหว่างอุปกรณ์ที่มีความต่างกัน

2.การเข้าสายแบบCross จะใช้สำหรับการเชื่อมต่อระหว่างอุปกรณ์ที่เหมือนกัน

![Logo](https://miro.medium.com/v2/resize:fit:4800/format:webp/1*hs8cEVxLXEgXdfM3h81BMw.png)


การเข้าสายLANจะเริ่มจากการมาปอกJacketออกประมาณ 1 นิ้วจากนั้นทำการคลายเกลียวและเรียงสายไฟสำหรับการเชื่อมต่อที่ต้องการ เมื่อเรียงและดัดสายไฟให้ตรงแล้วให้ดันสายไฟเข้าไปในหัวแลน(RJ45)ให้สุดจนเห็นทองเเดงจากนั้นใช้ด้ามคีมบีบหัวเเลนให้สุด

####  เทคนิค configure อุปกรณ์ 
VLAN :

กำหนด VLAN 801-804 สำหรับ Switch 1 (Services)

กำหนด VLAN 851-852 สำหรับ Switch 2 (Management)

VLAN Trunks ในการกำหนด VLAN แต่ละพอร์ตใน Switch

IP Subnet :

 - VLAN 801 = 10.80.1.1/24 
 - VLAN 802 = 10.80.2.1/24 
 - VLAN 803 = 10.80.3.1/24 
 - VLAN 804 = 10.80.4.1/24
 - VLAN 851 = 10.85.1.1/24
 - VLAN 852 = 10.85.2.1/24

(ใช้ DHCP ในการกำหนด IP)

NAT : Network Address Translation

#### Firewall fortigate 60e

![Logo](https://www.tbpgroup.com/wp-content/uploads/2018/05/fortigate-60e-500x400.png)

* [datasheet](https://www.firewalls.com/pub/media/wysiwyg/datasheets/Fortinet/FG-FW-60E.pdf)
* [FortiOS](https://docs.fortinet.com/product/fortigate/hardware)

#### Switch fortiswitch 424d
  
![Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTRK8DUjqK0NHeot6dOj2PprkFROuugANzQ2SENCfRYWOMQENSyrMqPOEm7T1Kk2nGONQ&usqp=CAU)

* [Specification](https://www.avfirewalls.com.au/FortiSwitch-424D.asp)

#### Server dell r330

![Logo](https://media.xbyte.com/cdn-cgi/image/width=500,height=320,format=auto,fit=scale-down/servers/Dell-PowerEdge-R330-Server_01.png)

* [datasheet](https://i.dell.com/sites/csdocuments/Shared-Content_data-Sheets_Documents/en/aa/Dell_PowerEdge_R330_SpecSheet_final.pdf)
