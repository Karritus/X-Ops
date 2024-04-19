### cluster
  
![image](https://github.com/Karritus/X-Ops/assets/148041642/d646cfb8-69aa-4fb5-b1e2-57e955777190)

### corosync

### kvm (lernel-base virtual machine

### LXC (linux container)

![image](https://github.com/Karritus/X-Ops/assets/148041642/4360cb46-f19c-4fc8-aa14-563657f302c2)

  #### Linux containers 
  เป็นเทคโนโลยีที่ใช้ในการแยกแยะและรวมกลุ่มของกระบวนการและการทำงานของแอพพลิเคชันในสภาพแวดล้อมที่กำหนดเอง โดยใช้ระบบปฏิบัติการ Linux ซึ่งมีการใช้งานพื้นที่แบบแยกกันบนเครื่องเดียวกัน

* Feature
  * **Isolation** : Containers สามารถแยกแยะการทำงานของแอปพลิเคชันจากกันและจากระบบปฏิบัติการหลักของเครื่อง เพื่อให้แต่ละ container ทำงานได้อิสระจากกันและไม่ส่งผลกระทบต่อกัน
  * **Lightweight** : Containers มีขนาดเล็กและใช้ทรัพยากรน้อยกว่าการสร้างเครื่องเสมือน (virtual machines) ซึ่งทำให้สามารถรันมากพร้อมกันบนเครื่องเดียวได้
  * **Portability** : Containers สามารถถูกพกพาและเคลื่อนย้ายไปยังระบบปฏิบัติการอื่นๆ โดยไม่ต้องปรับแต่งใหม่
  * **Efficiency** : เนื่องจากมีการแบ่งปันส่วนของระบบปฏิบัติการ ทำให้ทรัพยากรของระบบน้อยลงและการประมวลผลมีประสิทธิภาพมากขึ้น
  * **Scalability** : สามารถปรับขนาดและขยายตัวได้โดยง่าย เพิ่มหรือลดจำนวน container ตามความต้องการ
#### การใช้งาน LXC
  1. **Create Container** : ผู้ใช้สามารถสร้าง container ใหม่โดยใช้คำสั่ง lxc-create
  2. **Starte and Manage Container** : คำสั่ง lxc-start และ lxc-stop ใช้ในการเริ่มต้นและหยุดการทำงานของ containers ตามลำดับ
  3. **Manage Resource** : ผู้ใช้สามารถกำหนดและจัดการทรัพยากรต่างๆ ของ containers ได้ เช่น หน่วยความจำ พื้นที่จัดเก็บข้อมูล และเครือข่าย

### Linux bridge

![image](https://github.com/Karritus/X-Ops/assets/148041642/aaf30aa2-f068-4875-a876-314e35958b78)

 #### Linux bridge 
 เป็นเทคโนโลยีที่ใช้ในการเชื่อมต่อและส่งข้อมูลระหว่างเครื่องคอมพิวเตอร์หลายๆ เครื่องในระบบเครือข่ายแบบเชิงแพลตฟอร์ม

* Feature
  * **Layer 2 Network Connectivity** : Linux bridge เป็นสวิตช์เครือข่าย Layer 2 ซึ่งทำหน้าที่ในระดับ MAC address ของอุปกรณ์เครือข่าย เช่น Ethernet frames
  * **Transparent and Flexible Connectivity** : Linux bridge สามารถเชื่อมต่อกับหลายอุปกรณ์และเชื่อมต่อกับอินเทอร์เฟซของเครือข่ายได้ และยังสามารถกำหนดคุณสมบัติของเส้นทางการส่งข้อมูลได้
  * **Operation at Both Machine and Network Virtualization Levels** : Linux bridge ทำงานในระดับเครื่อง และสามารถเชื่อมต่อกับอินเทอร์เฟซเครือข่ายเสมือน (virtual network interfaces) เช่น TAP (Virtual Ethernet Pair)
  * **Support for Integration with Other Networks** : Linux bridge สามารถทำงานร่วมกับเครือข่ายอื่นๆ ได้ เช่น VLAN , bonding interfaces และ tunneling protocols



### Openvswitch

![image](https://github.com/Karritus/X-Ops/assets/148041642/80ae690e-8685-45c7-ab00-1709fb59239b)

 #### Open vSwitch (OVS) 
 เป็นโครงสร้างการสร้างเครือข่ายซอฟต์แวร์แบบ open-source ซึ่งใช้ในการจัดการและควบคุมการเชื่อมต่อเครือข่ายบนระบบปฏิบัติการ Linux โดยทั่วไป OVS เป็นสวิตช์เครือข่ายแบบ layer-2 และ layer-3 ที่สามารถทำงานร่วมกับหลายๆ เทคโนโลยีเครือข่ายอื่นๆ ได้

* Feature
  * **Support for OpenFlow Control** : Open vSwitch สามารถทำงานร่วมกับโปรโตคอล OpenFlow เพื่อจัดการกับการส่งข้อมูลในเครือข่าย ซึ่งช่วยให้ผู้ดูแลเครือข่ายสามารถควบคุมและปรับเปลี่ยนพฤติกรรมการส่งข้อมูลได้อย่างยืดหยุ่น
  * **Virtual Network Creation** : Open vSwitch สามารถใช้ในการสร้างเครือข่ายเสมือน (virtual networks) ที่เชื่อมต่อกับเครือข่ายที่มีอยู่ โดยสามารถกำหนดคุณสมบัติของเครือข่ายได้
  * **New Management Paradigms with SDN** : Open vSwitch เป็นส่วนหนึ่งของการจัดการเครือข่ายแบบซอฟต์แวร์กับ SDN ซึ่งช่วยให้สามารถจัดการเครือข่ายได้อย่างยืดหยุ่น และปรับปรุงประสิทธิภาพตามความต้องการขององค์กร
  * **Flexibility and Customization** : Open vSwitch มีความยืดหยุ่นในการปรับแต่งและกำหนดค่าต่างๆ ที่ตรงตามความต้องการของผู้ใช้
