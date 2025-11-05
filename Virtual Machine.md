1. Virtual Machine (VM) คืออะไร

   A) โปรแกรมสร้างกราฟิก 3D

   B) การจำลองระบบคอมพิวเตอร์ด้วยซอฟต์แวร์

   C) การเก็บข้อมูลบนคลาวด์

   D) โปรแกรมแปลงไฟล์

   คำตอบ: B

   อธิบาย: VM คือการจำลองระบบคอมพิวเตอร์แบบซอฟต์แวร์ — ให้สามารถรันระบบปฏิบัติการและแอปพลิเคชันเหมือนบนเครื่องจริง โดย Hypervisor จะสร้างสภาพแวดล้อมเสมือน (vCPU, vRAM, virtual disk, virtual NIC) เพื่อแยกการทำงานเป็นหน่วยอิสระจากฮาร์ดแวร์จริง

2. ระบบปฏิบัติการที่รันอยู่บนเครื่องจริงเรียกว่าอะไร

   A) Virtual OS

   B) Cloud OS

   C) Host OS

   D) Guest OS

   คำตอบ: C

   อธิบาย: ระบบปฏิบัติการบนเครื่องจริงเรียกว่า Host OS — เป็น OS ที่รันบนฮาร์ดแวร์จริงและอาจเป็นที่ติดตั้ง hypervisor (สำหรับ Type-2) หรือจัดการ VM และทรัพยากรของ host

3. ระบบปฏิบัติการที่รันอยู่ภายใน Virtual Machine เรียกว่าอะไร

   A) Hyper OS

   B) Host OS

   C) Guest OS

   D) Virtual Host

   คำตอบ: C

   อธิบาย: ระบบปฏิบัติการใน VM เรียกว่า Guest OS — guest OS มองเห็นฮาร์ดแวร์เสมือนที่ hypervisor ให้มาและรันแยกจาก host

4. โปรแกรมที่ใช้สร้างและจัดการ Virtual Machine คืออะไร

   A) Emulator

   B) Compiler

   C) Hypervisor

   D) Allocator

   คำตอบ: C

   อธิบาย: ซอฟต์แวร์ที่สร้างและจัดการ VM คือ Hypervisor (หรือ VMM — Virtual Machine Monitor) ซึ่งทำหน้าที่จัดสรรทรัพยากร จัดการ life-cycle ของ VM และทำ isolation ระหว่าง VM กับ host

5. Hypervisor แบบ Type 1 เรียกว่าอะไร

   A) Hosted Hypervisor

   B) Bare-Metal Hypervisor

   C) Software Layer Hypervisor

   D) Virtual Host Manager

   คำตอบ: B

   อธิบาย: Hypervisor แบบ Type-1 เรียกว่า Bare-Metal Hypervisor — ติดตั้งบนฮาร์ดแวร์โดยตรง (ไม่มี host OS ชั้นบน) เช่น VMware ESXi, Xen, Proxmox (KVM บางรูปแบบถูกใช้งานแบบนี้)

6. ตัวอย่างของ Type 1 Hypervisor คือข้อใด

   A) VirtualBox

   B) VMware Workstation

   C) VMware ESXi

   D) QEMU

   คำตอบ: C

   อธิบาย: VMware ESXi เป็นตัวอย่าง Type-1 (ติดตั้งบนฮาร์ดแวร์โดยตรง) — ต่างจาก VirtualBox/VMware Workstation ที่เป็น Type-2

7. Type 2 Hypervisor จะติดตั้งบนอะไร

   A) Hardware โดยตรง

   B) BIOS

   C) Host Operating System

   D) Firmware

   คำตอบ: C

   อธิบาย: Type-2 Hypervisor ติดตั้งบน Host Operating System (เช่น Windows/Linux) แล้วรัน VM เป็นกระบวนการ/แอปพลิเคชันของ host (ตัวอย่าง VirtualBox, VMware Workstation)

8. ตัวอย่างของ Type 2 Hypervisor คือข้อใด

   A) KVM

   B) Hyper-V Server Core

   C) VirtualBox

   D) VMware ESXi

   คำตอบ: C

   อธิบาย: VirtualBox เป็นตัวอย่าง Type-2 (ติดตั้งเป็นโปรแกรมบน host OS) ส่วน KVM เป็น module ใน Linux kernel (มักพิจารณาเป็นแบบที่ใกล้ Type-1) และ VMware ESXi เป็น Type-1

9. ข้อใดคือส่วนประกอบของ VM

   A) vCPU, vRAM, Virtual Disk, Virtual Network

   B) CPU, GPU, SSD, PSU

   C) Router, Firewall, Switch, DNS

   D) HTML, CSS, JavaScript, PHP

   คำตอบ: A

   อธิบาย: ส่วนประกอบหลักของ VM ได้แก่ vCPU, vRAM, virtual disk, virtual network interface — ส่วนประกอบเหล่านี้ยืดหยุ่นและถูกแม็ปไปยังทรัพยากรจริงภายใต้ hypervisor

10. ไฟล์ .vmdk เป็นไฟล์ชนิดใด

    A) ไฟล์ระบบเสียง

    B) ไฟล์วิดีโอจำลอง

    C) ไฟล์ดิสก์เสมือนของ VM

    D) ไฟล์บันทึกการทำงาน

    คำตอบ: C

    อธิบาย: .vmdk เป็นไฟล์ virtual disk ของ VMware — เก็บข้อมูลดิสก์เสมือน (เหมือนไฟล์ image ของดิสก์) ใช้เป็น storage backend ให้ guest OS

11. Virtualization คืออะไร

    A) การติดตั้ง OS ลงบน Hardware จริง

    B) การแบ่งพาร์ติชันของดิสก์

    C) การจำลองฮาร์ดแวร์หรือซอฟต์แวร์ให้ทำงานแยกอิสระ

    D) การเข้ารหัสข้อมูลในระบบ

    คำตอบ: C

    อธิบาย: Virtualization คือการ จำลองฮาร์ดแวร์หรือซอฟต์แวร์ เพื่อให้หลาย environment (VM/container) ทำงานแยกอิสระบนชั้นเดียวกันของฮาร์ดแวร์จริง — เกิด isolation, consolidation และความยืดหยุ่น

12. Containerization ต่างจาก Virtualization อย่างไร

    A) Container มี OS แยกของตัวเองเสมอ

    B) Virtualization ใช้ Container แทน VM

    C) Container ใช้ OS เดียวกันแต่แยก Environment

    D) ไม่มีความแตกต่าง

    คำตอบ: C

    อธิบาย: Containerization แยก environment ของแอปโดย ใช้ kernel เดียวกันกับ host แต่แยก namespace/filesystem/process — ต่างจาก VM ที่มี guest OS แยกตัวเต็มรูปแบบ (container ใช้ kernel ของ host ทำให้เบากว่าและเริ่มเร็วกว่า)

13. ข้อใดคือเทคนิคที่ใช้คุณสมบัติของ CPU เพื่อช่วยจำลองระบบ

    A) Full Virtualization

    B) Hardware-Assisted Virtualization

    C) Paravirtualization

    D) Application Virtualization

    คำตอบ: B

    อธิบาย: Hardware-Assisted Virtualization ใช้คุณสมบัติ CPU (เช่น Intel VT-x, AMD-V) เพื่อให้ guest รันได้ใกล้เคียง native มากขึ้น ลด VM-exit และ overhead จากการ trap-and-emulate
    
14. Paravirtualization คืออะไร

    A) Guest OS ถูกปรับแต่งให้ทำงานกับ Hypervisor โดยตรง

    B) การจำลองทุกส่วนของฮาร์ดแวร์

    C) การรันแอปเดียวแบบ platform-independent

    D) การแยกระบบเครือข่าย

    คำตอบ: A

    อธิบาย: Paravirtualization คือการปรับแก้ Guest OS ให้ติดต่อกับ Hypervisor โดยตรง (ใช้ paravirtual drivers/APIs) เพื่อลด overhead ของการ emulate ตัวอย่างเช่น Xen paravirtualized guests หรือ VirtIO drivers

15. ตัวอย่างของ Process Virtual Machine คืออะไร

    A) VMware

    B) KVM

    C) Java Virtual Machine (JVM)

    D) Hyper-V

    คำตอบ: C

    อธิบาย: JVM (Java Virtual Machine) เป็น Process Virtual Machine — จำลอง runtime environment สำหรับแอปพลิเคชัน (รัน bytecode) เพื่อให้ platform-independent

16. ข้อใดเป็นข้อดีของ Virtual Machine

    A) ใช้ทรัพยากรสูงขึ้นเสมอ

    B) ไม่สามารถแยกระบบได้

    C) ทำ Snapshot และกู้คืนระบบได้

    D) รันได้เฉพาะ OS เดียว

    คำตอบ: C

    อธิบาย: ข้อดีสำคัญคือสามารถ snapshot และกู้คืนระบบได้ — นอกจากนี้ยังมี isolation, consolidation, และลดต้นทุนฮาร์ดแวร์ เป็นต้น

17. “Server Consolidation” หมายถึงอะไร

    A) รวมเซิร์ฟเวอร์หลายเครื่องให้เหลือเครื่องเดียวโดยใช้ VM

    B) การขยายพื้นที่เก็บข้อมูล

    C) การรวมระบบไฟล์

    D) การรวมรหัสผ่านเซิร์ฟเวอร์

    คำตอบ: A

    อธิบาย: Server Consolidation หมายถึงการรวม workloads หลายๆ อย่างไว้บน host เดียวโดยการใช้ VM เพื่อลดจำนวนเซิร์ฟเวอร์จริงและประหยัดค่าใช้จ่าย

18. Snapshot ของ VM คืออะไร

    A) รูปภาพหน้าจอ

    B) การบันทึกสถานะของ VM ณ เวลาหนึ่ง

    C) การย้าย VM

    D) การคัดลอกไฟล์ Log

    คำตอบ: B

    อธิบาย: Snapshot เป็นการ บันทึกสถานะของ VM ณ ช่วงเวลาหนึ่ง — รวม CPU state (บางระบบ), disk differencing, และ config เพื่อให้ย้อนกลับได้

19. VM Migration คืออะไร

    A) การย้ายข้อมูลระหว่างดิสก์

    B) การย้าย VM จาก Host หนึ่งไปอีก Host หนึ่ง

    C) การลบ VM

    D) การ Backup เฉพาะ vRAM

    คำตอบ: B

    อธิบาย: VM Migration คือการ ย้าย VM จาก Host หนึ่งไปอีก Host หนึ่ง — อาจเป็น cold (ขณะปิด) หรือ live migration (ขณะทำงาน)

20. การสร้าง VM ใหม่เรียกว่าอะไรในวงจรชีวิตของ VM

    A) Deployment

    B) Provisioning

    C) Management

    D) Decommissioning

    คำตอบ: B

    อธิบาย: การสร้าง VM ใหม่ใน lifecycle เรียกว่า Provisioning — การจองทรัพยากร ติดตั้ง image และตั้งค่า initial configuration

21. ขั้นตอน “Decommissioning” ในวงจรชีวิต VM หมายถึงอะไร

    A) การสร้าง VM

    B) การใช้งาน VM

    C) การเลิกใช้งานหรือยกเลิก VM

    D) การอัปเกรดระบบ

    คำตอบ: C

    อธิบาย: Decommissioning คือ การเลิกใช้งาน/ถอนการติดตั้ง VM (terminate) พร้อมลบข้อมูลที่ไม่ต้องการและจัดการ resources ให้คืนกลับ

22. การจัดสรร vCPU และ vRAM ถือเป็นส่วนหนึ่งของขั้นตอนใด

    A) Snapshot Management

    B) Resource Management

    C) Migration

    D) Backup

    คำตอบ: B

    อธิบาย: การจัดสรร vCPU และ vRAM เป็นส่วนหนึ่งของ Resource Management — การจัดสรร/resize/limit และ tuning ทรัพยากรของ VM

23. การรันหลายระบบปฏิบัติการบนเครื่องเดียวเกิดจากอะไร

    A) Cloud-only feature

    B) Dual Boot

    C) Virtualization

    D) BIOS Configuration

    คำตอบ: C

    อธิบาย: การรันหลาย OS บนเครื่องเดียวเกิดจาก Virtualization (หรือ dual-boot เป็นอีกแนวทางแต่ไม่ใช่การรันพร้อมกัน) — VM ช่วยให้รันหลาย OS พร้อมกัน

24. ข้อใดเป็นข้อจำกัดของ Virtual Machine

    A) ไม่สามารถ Backup ได้

    B) มี Overhead ด้านประสิทธิภาพเล็กน้อย

    C) ไม่รองรับหลาย OS

    D) ไม่สามารถใช้งานบน Cloud

    คำตอบ: B

    อธิบาย: ข้อจำกัดคือมี overhead ด้านประสิทธิภาพเล็กน้อย (จากการ abstraction) และความซับซ้อนในการจัดการทรัพยากร แม้ hardware-assisted virtualization จะลด overhead ลงมาก

25. ข้อใดเป็นตัวอย่างการใช้งานจริงของ VM

    A) การวาดภาพ 3 มิติ

    B) การเล่นเกมออนไลน์

    C) การสร้างสภาพแวดล้อม Dev/Test

    D) การแก้ไขไฟล์ PDF

    คำตอบ: C

    อธิบาย: หนึ่ง use-case ที่ชัดเจนคือ การสร้างสภาพแวดล้อม Dev/Test — ให้แยกกัน ทดสอบ rollback และ snapshot ได้ง่าย

26. บริการ Cloud ใดที่ใช้ VM เป็นพื้นฐานการทำงานหลัก

    A) AWS EC2

    B) Google Drive

    C) GitHub Pages

    D) Dropbox

    คำตอบ: A

    อธิบาย: AWS EC2 (Elastic Compute Cloud) ใช้ VM/instance เป็นหน่วยประมวลผลพื้นฐาน — ให้เลือก instance types, images (AMI) และจัดการ lifecycle ของ VM

27. Hypervisor ทำหน้าที่ใดหลัก ๆ

    A) จัดการฐานข้อมูล

    B) จัดสรรทรัพยากรให้ VM

    C) แปลงโค้ดเป็นไฟล์ปฏิบัติการ

    D) สร้างเครือข่ายใน LAN

    คำตอบ: B

    อธิบาย: Hypervisor ทำหน้าที่ จัดสรรทรัพยากรให้ VM (CPU scheduling, memory allocation, I/O management) และทำ isolation ระหว่าง VM

28. Virtual Network Interface ใช้ทำอะไร

    A) สร้างกราฟิกเสมือน

    B) เชื่อมต่อ VM เข้ากับเครือข่าย

    C) จำลองเสียงภายในระบบ

    D) จัดการหน่วยความจำ

    คำตอบ: B

    อธิบาย: Virtual Network Interface (vNIC) ใช้เชื่อมต่อ VM เข้ากับเครือข่าย ภายใน host/ไปยังภายนอก ให้การสื่อสาร layer-2/3 ตามการตั้งค่า vSwitch/vRouter

29. การคิดค่าบริการ VM บน Cloud มักใช้โมเดลใด

    A) Monthly Contract

    B) Lifetime License

    C) Pay-as-you-go

    D) Free Tier Only

    คำตอบ: C

    อธิบาย: โมเดลการคิดค่าบริการบน cloud มักเป็น Pay-as-you-go — จ่ายตามการใช้งานจริง (per-second/hour) ยืดหยุ่น

30. ข้อใดคือประโยชน์ด้านความปลอดภัยของการใช้ VM

    A) ทำให้ระบบเร็วขึ้น

    B) ใช้เป็น Security Sandbox สำหรับทดสอบมัลแวร์

    C) ลบมัลแวร์โดยอัตโนมัติ

    D) แปลงข้อมูลเป็นรหัสผ่าน

    คำตอบ: B

    อธิบาย: หนึ่งในประโยชน์ด้านความปลอดภัยคือการใช้ VM เป็น Security Sandbox — รันแอปที่ไม่แน่นอนหรือทดสอบมัลแวร์ใน VM แยกจากระบบจริงเพื่อลดความเสี่ยง

31. ฟีเจอร์ของ CPU เช่น Intel VT-x และ AMD-V ช่วยให้ Hypervisor ทำอะไรได้ดีขึ้น

    A) จำลองเสียงได้ดีขึ้น

    B) ลด Overhead ในการจำลองฮาร์ดแวร์

    C) เพิ่มความละเอียดของกราฟิกใน VM

    D) เพิ่มความจุของ vRAM

    คำตอบ: B

    อธิบาย: Intel VT-x / AMD-V ลด overhead ของการจำลองฮาร์ดแวร์ ทำให้ hypervisor ไม่ต้อง trap & emulate ทุก privileged instruction และช่วยให้ performance ใกล้ native มากขึ้น โดย features เสริมเช่น EPT/NPT ช่วย map virtual→physical addresses ได้มีประสิทธิภาพ

32. Hypervisor ใช้เทคนิค “Ring De-privileging” เพื่ออะไร

    A) ลดสิทธิ์การเข้าถึงของ Guest OS เพื่อจำลอง privilege level ของ CPU

    B) เพิ่มสิทธิ์ของ Guest OS

    C) จัดการ Network Traffic

    D) ปรับขนาด Storage อัตโนมัติ

    คำตอบ: A

    อธิบาย: Ring De-privileging คือการลดสิทธิ์ของ Guest kernel (ดันลงจาก ring0) เพื่อ hypervisor จะเป็นผู้มีสิทธิ์สูงสุดและสามารถ intercept privileged ops — การใช้ hardware virtualization ช่วยลด VM-exit ที่เกิดจากวิธีดั้งเดิม

33. ในการจำลอง I/O ของ VM เช่น Disk และ Network, Hypervisor มักใช้เทคโนโลยีอะไรเพื่อเพิ่มประสิทธิภาพ

    A) Emulation ผ่าน BIOS

    B) Direct I/O หรือ VirtIO driver

    C) Full software emulation

    D) API Translation

    คำตอบ: B

    อธิบาย: เพื่อเพิ่มประสิทธิภาพ I/O hypervisor มักใช้ Direct I/O (PCI passthrough, SR-IOV) หรือ paravirtual drivers (เช่น VirtIO) แทน full emulation — ลด context switches และ latency, เพิ่ม throughput

34. ถ้า Host มี CPU 8 Core แล้วกำหนด vCPU ให้ VM รวมกันเกิน 8 Core จะเกิดอะไรขึ้น

    A) เครื่องพังทันที

    B) เรียกว่า vCPU overcommit — Hypervisor จะสลับการประมวลผล (scheduling)

    C) VM จะไม่บูต

    D) ไม่สามารถสร้าง VM ได้

    คำตอบ: B

    อธิบาย: การกำหนด vCPU รวมกันเกินจำนวน core จริงเรียกว่า vCPU overcommit — hypervisor ต้องทำ scheduling (time-slicing) ให้ vCPUs ต่าง ๆ ใช้ pCPU ตามเวลาที่กำหนด ผลคือ CPU contention และ CPU-ready time ถ้ามากเกินจะกระทบ performance

35. ฟังก์ชัน “Ballooning” ใน Virtualization หมายถึงอะไร

    A) การขยายไฟล์ vDisk อัตโนมัติ

    B) การจัดการหน่วยความจำ (Memory Reclamation) เพื่อดึง RAM กลับจาก VM

    C) การขยายขนาด vCPU

    D) การเพิ่ม Snapshot

    คำตอบ: B

    อธิบาย:  ฟังก์ชัน Ballooning ใน Virtualization คือเทคนิคการจัดการหน่วยความจำที่ไฮเปอร์ไวเซอร์ (hypervisor) ใช้เพื่อเรียกคืนหน่วยความจำที่ไม่ได้ใช้งานจากเครื่องเสมือน (VM) ที่มีหน่วยความจำเหลืออยู่ เพื่อนำไปจัดสรรให้กับเครื่องเสมือนอื่นที่ต้องการหน่วยความจำเพิ่ม กระบวนการนี้จะทำให้เครื่องเสมือน (guest) ใช้หน่วยความจำได้น้อยลงในขณะที่เครื่องอื่น (host) สามารถจัดสรรหน่วยความจำที่ถูกยืมไปนั้นให้กับ VM ที่ต้องการได้

36. การทำ “Thin Provisioning” ของ Storage มีจุดประสงค์หลักคืออะไร

    A) สำรองพื้นที่เต็มตั้งแต่แรก

    B) สร้าง Disk โดยใช้พื้นที่จริงเท่าที่ใช้จริง

    C) ล็อกขนาด Disk คงที่

    D) ป้องกันการลบไฟล์

    คำตอบ: B

    อธิบาย: Thin provisioning ให้ logical disk ขนาดใหญ่ แต่จัดเก็บพื้นที่จริงเฉพาะเมื่อเขียนข้อมูล — ประหยัดพื้นที่แต่มีความเสี่ยงถ้าหลาย VM ขยายพร้อมกัน (storage overcommit)

37. การ Snapshot VM หลายชั้น (Nested Snapshot) อาจก่อให้เกิดปัญหาอะไร

    A) ลดความปลอดภัยของ VM

    B) ใช้พื้นที่ Disk มากและลดประสิทธิภาพ I/O

    C) เพิ่มความเร็วการบูต

    D) ลบ Snapshot เดิมโดยอัตโนมัติ

    คำตอบ: B

    อธิบาย: Nested Snapshot (สแนปช็อตแบบซ้อนกัน) คือการสร้างสแนปช็อตของ Virtual Machine (VM) ซ้ำ ๆ ต่อเนื่องกันไป ซึ่งแต่ละสแนปช็อตจะอ้างอิงถึงสถานะของสแนปช็อตก่อนหน้า ปัญหาหลักที่ตามมาจากการทำสแนปช็อตหลายชั้น คือผลกระทบต่อ พื้นที่จัดเก็บข้อมูล และประสิทธิภาพการทำงาน

           1. การใช้พื้นที่ Disk อย่างมหาศาล

              - หลักการทำงาน: สแนปช็อตไม่ได้คัดลอกไฟล์ดิสก์หลักทั้งหมด แต่จะสร้างไฟล์ Delta Disk หรือ Redo Log ใหม่

              - ปัญหา: ไฟล์ Delta Disk เหล่านี้จะบันทึกเฉพาะข้อมูลที่มีการเปลี่ยนแปลง (Writes) หลังจากที่สร้างสแนปช็อตนั้น ๆ เมื่อคุณทำสแนปช็อตหลายชั้นติดกัน จะมีไฟล์ Delta Disk สะสมเพิ่มขึ้นเรื่อย ๆ ส่งผลให้ ใช้พื้นที่จัดเก็บข้อมูลจริงบน Host (Hypervisor) มากขึ้นอย่างรวดเร็ว โดยเฉพาะเมื่อ VM มีการใช้งาน I/O สูง

           2. การลดประสิทธิภาพ I/O (Input/Output)

              - หลักการทำงาน: เมื่อ VM ถูกเรียกใช้งานในสถานะสแนปช็อต ระบบจะต้องอ่านข้อมูลผ่านไฟล์ Delta Disk หลายชั้นย้อนกลับไปจนถึงไฟล์ดิสก์หลัก (Base Disk)

              - ปัญหา: ทุกการอ่านข้อมูล (Read) จะต้องผ่านกระบวนการ Traversal หรือการค้นหาย้อนหลังผ่านไฟล์ Delta Disk ที่ซ้อนกันหลายชั้น ทำให้เกิดความซับซ้อนและเพิ่มเวลาหน่วง (Latency) ในการเข้าถึงข้อมูล ลดประสิทธิภาพ I/O ของ VM ลงอย่างเห็นได้ชัด

           ❌ ตัวเลือกอื่น ๆ ที่ไม่ถูกต้อง

               A) ลดความปลอดภัยของ VM: การทำสแนปช็อตเป็นฟีเจอร์การจัดการ ไม่ได้ส่งผลโดยตรงต่อความปลอดภัย (Security) ของระบบ VM

               C) เพิ่มความเร็วการบูต: ตรงกันข้าม การมีสแนปช็อตหลายชั้นมักจะ ลดความเร็วในการทำงาน โดยรวม รวมถึงการบูตด้วย เนื่องจากระบบต้องประมวลผลความเปลี่ยนแปลงของไฟล์จำนวนมาก

               D) ลบ Snapshot เดิมโดยอัตโนมัติ: ระบบส่วนใหญ่ไม่ได้ลบสแนปช็อตเก่าโดยอัตโนมัติ ผู้ดูแลระบบต้องดำเนินการลบเอง (Commit/Consolidate) การลืมลบสแนปช็อตทิ้งไว้เป็นระยะเวลานาน คือสาเหตุหลักของปัญหาพื้นที่ดิสก์เต็มและประสิทธิภาพตกต่ำ

38. การใช้ “vMotion” ของ VMware หรือ “Live Migration” ของ KVM หมายถึงอะไร

    A) ย้าย VM ระหว่าง Host โดยไม่หยุดทำงาน

    B) ย้าย Snapshot

    C) สร้าง VM ใหม่จาก Template

    D) อัปเดต Hypervisor

    คำตอบ: A

    อธิบาย: vMotion คือการโยกย้ายเครื่องเสมือนระหว่างเซิร์ฟเวอร์ในขณะที่เครื่องเสมือนกำลังทำงานแบบสด ๆ (ย้ายเครื่องเสมือนจากเซิร์ฟเวอร์หนึ่งไปยังอีกเซิร์ฟเวอร์หนึ่งได้แบบสดๆ ) เราไม่ต้องปิดเครื่องเสมือน ซึ่งหมายความว่าผู้ใช้ระบบปฏิบัติการจะไม่หยุดทำงานหรือถูกรบกวนในระหว่างการโยกย้ายเวิร์กโหลด

           Live Migration เป็นคำศัพท์ทั่วไปในอุตสาหกรรมการจำลองเสมือน (Virtualization) ในขณะที่ vMotion เป็นชื่อเทคโนโลยีภายใต้เครื่องหมายการค้าของ VMware ซึ่งทั้งสองมีจุดประสงค์เดียวกันคือ:

           1. การย้ายโดยไม่หยุดบริการ (Zero Downtime)

              - หลักการ: กระบวนการนี้จะโอนย้าย สถานะการทำงานทั้งหมด ของ VM ซึ่งรวมถึงหน่วยความจำ (Active Memory), สถานะ CPU (Execution State), และการเชื่อมต่อเครือข่าย ให้ไปยัง Host ใหม่

              - กระบวนการโดยย่อ:

                1. คัดลอกหน่วยความจำส่วนใหญ่ของ VM จาก Host ต้นทางไปยัง Host ปลายทาง

                2. ในช่วงสุดท้าย จะมีการหยุดทำงาน (Stun Time) เพียงชั่ววินาทีเดียว (มักจะน้อยกว่า 1 วินาที) เพื่อคัดลอกหน่วยความจำส่วนที่เปลี่ยนแปลงไปในช่วงเวลาที่ทำการโอนย้าย

                3. VM จะเปิดทำงานต่อบน Host ปลายทางอย่างรวดเร็ว โดยที่เซสชันของแอปพลิเคชันหรือผู้ใช้ยังคงอยู่

           2. จุดประสงค์ในการใช้งาน

              - การบำรุงรักษาฮาร์ดแวร์ (Planned Maintenance): สามารถย้าย VM ออกจากเซิร์ฟเวอร์ที่ต้องการอัปเดตเฟิร์มแวร์หรือซ่อมบำรุงได้โดยไม่ต้องปิด VM

              - การปรับสมดุลภาระงาน (Load Balancing): ใช้เพื่อย้าย VM ที่มีการใช้งานทรัพยากรสูงไปยังเซิร์ฟเวอร์ที่มีทรัพยากรว่างมากกว่า เพื่อให้เกิดการใช้ทรัพยากรอย่างมีประสิทธิภาพทั่วทั้งกลุ่มเซิร์ฟเวอร์ (Cluster)

              - การประหยัดพลังงาน: ย้าย VM ออกจากเซิร์ฟเวอร์ที่มีภาระงานต่ำ เพื่อให้สามารถปิดเซิร์ฟเวอร์นั้น ๆ ได้
    
40. “NUMA Awareness” มีความสำคัญต่อ VM อย่างไร

    A) เกี่ยวกับการจัดการ Network Bandwidth

    B) เกี่ยวกับการแม็ปหน่วยความจำและ CPU ให้เหมาะกับโครงสร้าง NUMA ของ Host

    C) ใช้สำหรับทำ Snapshot

    D) ปรับขนาด Disk

    คำตอบ: B

    อธิบาย: NUMA awareness สำคัญเพราะ host อาจมี NUMA nodes — ถ้าจัด vCPU หรือ memory กระจายข้าม node จะเกิด remote memory access ที่ช้ากว่า local memory การตั้ง affinity/placement จะลด latency และใช้ performance ได้เต็มที่

           NUMA Awareness (การรับรู้ NUMA) เป็นคุณสมบัติที่สำคัญอย่างยิ่งสำหรับ Hypervisor (เช่น VMware ESXi, Hyper-V, KVM) ในการจัดการเครื่องเสมือน (VM) โดยเฉพาะ VM ที่มีขนาดใหญ่และต้องการประสิทธิภาพสูง

           1. เป้าหมาย: ลดการเข้าถึงหน่วยความจำระยะไกล

              ในระบบเซิร์ฟเวอร์สมัยใหม่ที่มีหลายซ็อกเก็ต CPU , แต่ละกลุ่มของ CPU และหน่วยความจำที่เชื่อมต่อกันอย่างใกล้ชิดจะเรียกว่า NUMA Node

              - Local Memory Access: CPU สามารถเข้าถึงหน่วยความจำที่อยู่บน Node ของตัวเองได้ เร็วกว่า

              - Remote Memory Access: การเข้าถึงหน่วยความจำที่อยู่บน Node อื่น (Remote Memory) ต้องเดินทางผ่านลิงก์เชื่อมต่อ (Interconnect Bus) ซึ่งทำให้เกิด ความหน่วง (Latency) สูงขึ้นและใช้แบนด์วิดท์ของระบบ

            NUMA Awareness ของ Hypervisor จึงมุ่งเน้นการจัดสรรทรัพยากรเพื่อให้ CPU เสมือน (vCPU) และ หน่วยความจำเสมือน (vMemory) ของ VM อยู่ใน Physical NUMA Node เดียวกัน บนเซิร์ฟเวอร์จริงให้มากที่สุด

            2. ผลกระทบต่อประสิทธิภาพ

               หาก Hypervisor ขาด NUMA Awareness หรือมีการจัดสรรทรัพยากรที่ไม่ดี (เช่น จัดสรร vCPU จาก Node 0 แต่ vMemory จาก Node 1):

               - VM จะต้องทำการเข้าถึง Remote Memory บ่อยครั้ง

               - ประสิทธิภาพการทำงานของ VM โดยเฉพาะเวิร์กโหลดที่ต้องใช้หน่วยความจำสูง (Memory-intensive workloads) จะ ลดลงอย่างมาก

             การแม็ป (Mapping) ทรัพยากรอย่างถูกต้องตามโครงสร้าง NUMA ของ Host จึงเป็นกุญแจสำคัญในการรับประกันว่า VM จะได้รับประสิทธิภาพการเข้าถึงหน่วยความจำที่เร็วที่สุด (Local Access) ใกล้เคียงกับการรันบนฮาร์ดแวร์จริง
    
           NUMA Awareness (การรับรู้ NUMA) คือความสามารถของระบบปฏิบัติการ (OS), Hypervisor, หรือแอปพลิเคชันในการรับรู้และจัดการ โครงสร้างฮาร์ดแวร์แบบ Non-Uniform Memory Access (NUMA) เพื่อเพิ่มประสิทธิภาพการทำงานสูงสุด
           1. โครงสร้าง NUMA คืออะไร ?

              - Non-Uniform Memory Access (NUMA) คือสถาปัตยกรรมหน่วยความจำที่ใช้ในระบบเซิร์ฟเวอร์ขนาดใหญ่ที่มี ซ็อกเก็ต CPU หลายตัว (Multi-socket Systems)

              - แต่ละซ็อกเก็ต CPU (หรือกลุ่มคอร์) จะถูกจัดเป็น NUMA Node ซึ่งมี หน่วยความจำเฉพาะของตัวเอง (Local Memory) และ I/O ของตัวเอง .

              - ความไม่สม่ำเสมอ: CPU สามารถเข้าถึงหน่วยความจำที่อยู่บน Node ของตัวเองได้ เร็วกว่า การเข้าถึงหน่วยความจำที่อยู่บน Node อื่น (Remote Memory) ผ่านลิงก์เชื่อมต่อระหว่าง Node (Interconnect Bus)
    
           2. NUMA Awareness ทำงานอย่างไร ?

              NUMA Awareness เป็นการปรับปรุงซอฟต์แวร์ (OS Scheduler, Hypervisor หรือแอปพลิเคชัน) เพื่อใช้ประโยชน์จากความแตกต่างของความเร็วในการเข้าถึงหน่วยความจำนี้:

    <img width="894" height="414" alt="NUMA01" src="https://github.com/user-attachments/assets/b29e3deb-c562-423a-bbbd-1dae1df20061" />

42. ในระบบ Cloud (เช่น AWS EC2) การเลือก Instance Type เช่น t2.micro หรือ m5.large หมายถึงอะไร

    A) เลือก OS ที่ติดตั้ง

    B) เลือกขนาดของทรัพยากร VM (vCPU, RAM, Network)

    C) เลือกประเภท Storage เท่านั้น

    D) เลือกระดับ Security

    คำตอบ: B

    อธิบาย: ใน cloud การเลือก instance type (t2, m5, c5 ฯลฯ) กำหนดขนาดทรัพยากรของ VM — vCPU, memory, network, IO performance และลักษณะพิเศษเช่น burstable credits

43. Virtual Switch (vSwitch) มีหน้าที่อะไรใน Virtual Network

    A) จำลองพอร์ตเชื่อมต่อ Network ระหว่าง VM

    B) จัดการ CPU Scheduling

    C) จัดการไฟล์ Snapshot

    D) บันทึก Log ของ Guest OS

    คำตอบ: A

    อธิบาย: vSwitch ทำหน้าที่เป็นสวิตช์ภายใน virtual network — เชื่อม VM กันหรือเชื่อม VM กับ external network, รองรับ VLAN, port-group, security policies, traffic shaping และ mirror

44. “Bridged Networking” ต่างจาก “NAT Networking” อย่างไรใน VM

    A) Bridged ใช้ IP เดียวกับ Host

    B) NAT ให้ VM ออกอินเทอร์เน็ตผ่าน IP ของ Host

    C) Bridged ต้องใช้ VPN

    D) NAT ทำให้ VM มองไม่เห็น Host

    คำตอบ: B

    อธิบาย: ใน NAT mode VM ออกอินเทอร์เน็ตผ่าน IP ของ host (หรือ NAT gateway) ทำให้ VM ไม่ถูกเข้าถึงจากภายนอกโดยตรง (ต้องทำ port forwarding) ขณะที่ Bridged ให้ VM อยู่บน LAN เดียวกันและได้ IP ของ network จริง

45. ฟีเจอร์ “Nested Virtualization” หมายถึงอะไร

    A) การรัน VM ภายใน VM อีกชั้นหนึ่ง

    B) การรวมหลาย Snapshot เข้าด้วยกัน

    C) การแชร์ Storage ข้าม VM

    D) การจำลอง BIOS ภายใน VM

    คำตอบ: A

    อธิบาย: Nested virtualization คือการรัน hypervisor ภายใน guest (VM ที่รัน VM อีกชั้น) — ใช้ใน lab/test หรือ virtualization development ต้องการการสนับสนุนจาก CPU/hypervisor

46. การใช้ “Template” ในระบบจัดการ VM มีประโยชน์อย่างไร

    A) เพิ่มประสิทธิภาพการจำลองเสียง

    B) ช่วยสร้าง VM ใหม่จากต้นแบบที่กำหนดไว้

    C) ใช้สำหรับการ Backup

    D) ปรับแต่ง Firewall

    คำตอบ: B

    อธิบาย: Template เป็นต้นแบบของ VM ที่บรรจุ OS + config + packages — ใช้ deploy VM ใหม่อย่างรวดเร็วและสม่ำเสมอ ลดความผิดพลาดจากการตั้งค่าด้วยมือ

47. ถ้า Snapshot ถูกลบโดยไม่ Merge กลับไปยัง Disk หลัก จะเกิดผลอย่างไร

    A) ไม่มีผลกระทบ

    B) VM จะเสียข้อมูลล่าสุด

    C) เพิ่มประสิทธิภาพการรัน

    D) ระบบจะสร้าง Snapshot ใหม่อัตโนมัติ

    คำตอบ: B

    อธิบาย: ถ้าลบ snapshot โดยไม่ merge ข้อมูลที่อยู่ใน snapshot อาจหลุดหรือสูญหาย (ขึ้นกับ implementation) — การลบ snapshot มักต้องมี consolidation (merge) เข้ากับ base disk เพื่อรักษาความต่อเนื่องของข้อมูล

48. การใช้ “Cloud-init” ใน VM มีจุดประสงค์อะไร

    A) ใช้บูตเครื่องเร็วขึ้น

    B) ใช้ตั้งค่าระบบอัตโนมัติในครั้งแรกของการบูต (เช่น user, SSH key, network)

    C) ใช้เก็บ Log

    D) ใช้จัดการ Snapshot

    คำตอบ: B

    อธิบาย: cloud-init ใช้สำหรับ ตั้งค่าระบบอัตโนมัติที่ first boot (เช่น สร้าง user, ใส่ SSH keys, config network, run scripts) — ทำ provisioning แบบ automated เมื่อ deploy images บน cloud

49. “VM Sprawl” คืออะไร

    A) การรัน VM หลายเครื่องโดยไม่จัดการ ทำให้เกิดความซ้ำซ้อนและใช้ทรัพยากรเกิน

    B) การขยาย Storage อัตโนมัติ

    C) การย้าย VM หลายเครื่องพร้อมกัน

    D) การเพิ่มจำนวน CPU ใน Host

    คำตอบ: A

    อธิบาย: VM Sprawl คือการสร้าง VM จำนวนมากโดยขาด governance — ทำให้ resource waste, security risk (unpatched), และเพิ่มค่าใช้จ่าย การควบคุมด้วย tagging, lifecycle policy, automation ช่วยแก้ปัญหา

50. การรักษาความปลอดภัยของ VM ทำได้ดีที่สุดโดยแนวทางใด

    A) ปิด Firewall

    B) ใช้ Network Isolation และ Snapshot Security Testing

    C) แชร์ Disk ระหว่างหลาย VM

    D) รันทุก VM ด้วยสิทธิ์ Root

    คำตอบ: B

    อธิบาย: การรักษาความปลอดภัย VM ที่ดีรวม network isolation (VLANs, security groups), patching, access control management plane, encryption, และการทดสอบผ่าน snapshots (sandbox testing) — ปิด firewall หรือรัน root ไม่ใช่แนวทางที่ปลอดภัย

51. ข้อใดคือปัญหาที่เกิดขึ้นเมื่อ Overcommit RAM มากเกินไป

    A) ระบบหยุดทำงานทันที

    B) VM จะใช้ Swap มาก ทำให้ช้า

    C) CPU ใช้ไม่เต็ม

    D) Network ถูกจำกัด

    คำตอบ: B

    อธิบาย: เมื่อ overcommit RAM มากไป VM/host จะเริ่มใช้ swap (hypervisor swap หรือ guest swap) ทำให้ performance ลดลงอย่างมาก (I/O bound) — อาจนำไปสู่ OOM และกระทบความเสถียร

52. Hypervisor ที่มาพร้อม Linux Kernel โดยตรงคืออะไร

    A) VMware ESXi

    B) KVM (Kernel-based Virtual Machine)

    C) XenServer

    D) QEMU

    คำตอบ: B

    อธิบาย: KVM (Kernel-based Virtual Machine) เป็น hypervisor ที่เป็นส่วนหนึ่งของ Linux kernel — ใช้ QEMU ใน userland สำหรับ device emulation และ libvirt เป็น toolstack ที่นิยมใช้ร่วม

53. การใช้ “SR-IOV” ใน VM มีประโยชน์อะไร

    A) แยก Storage ให้ VM

    B) ให้ VM เข้าถึงอุปกรณ์ Network โดยตรง เพิ่มประสิทธิภาพ I/O

    C) ปรับขนาด vRAM

    D) ใช้ Snapshot

    คำตอบ: B

    อธิบาย: SR-IOV แยก physical NIC เป็น virtual functions ให้ VM เข้าถึง network device โดยตรง (ผ่าน VF) เพิ่ม throughput และลด latency เทียบกับ hypervisor-mediated I/O แต่ trade-off คือความยืดหยุ่น (live migration ยากขึ้น)

54. ข้อใดต่อไปนี้ไม่ใช่ส่วนหนึ่งของ “VM Lifecycle”

    A) Provisioning

    B) Deployment

    C) Termination

    D) Compilation

    คำตอบ: D

    อธิบาย: VM lifecycle ประกอบด้วย provisioning, deployment, management, termination แต่ compilation ไม่ใช่ขั้นตอนของ lifecycle (เป็นการแปลงโค้ด)

55. ในการใช้งาน VirtualBox, “Guest Additions” มีหน้าที่อะไร

    A) เพิ่มฟีเจอร์ เช่น Shared Clipboard, Mouse Integration, Display Driver

    B) ทำ Snapshot อัตโนมัติ

    C) แปลงไฟล์ vmdk เป็น iso

    D) สร้าง Template

    คำตอบ: A

    อธิบาย: VirtualBox Guest Additions คือชุดของซอฟต์แวร์ (ไดรเวอร์และแอปพลิเคชันระบบ) ที่ออกแบบมาเพื่อติดตั้งภายใน Guest Operating System (Guest OS) หรือระบบปฏิบัติการที่ทำงานอยู่บน Virtual Machine (VM) เพื่อเพิ่มประสิทธิภาพและความสะดวกสบาย ในการใช้งาน VM อย่างมาก

    องค์ประกอบและหน้าที่ของ Guest Additions

    - Shared Clipboard คลิปบอร์ดที่ใช้ร่วมกัน คุณสมบัตินี้ทำให้คุณสามารถคัดลอกข้อความหรือไฟล์จาก Host OS (เครื่องคอมพิวเตอร์จริง) แล้วนำไปวางใน Guest OS ได้โดยตรง และในทางกลับกัน ทำให้การแลกเปลี่ยนข้อมูลระหว่างสองระบบเป็นไปอย่างราบรื่น

    - Mouse Integration การรวมเมาส์พอยเตอร์ เป็นการติดตั้งไดรเวอร์อุปกรณ์ชี้ตำแหน่งเสมือน ทำให้เมาส์พอยเตอร์สามารถเคลื่อนที่เข้าออกระหว่างหน้าต่าง VM (Guest OS) และหน้าจอ Host OS ได้อย่างอิสระ โดยไม่ต้องกดปุ่ม Host Key (ปกติคือ Right Ctrl) เพื่อ "จับ" หรือ "ปล่อย" เมาส์ ซึ่งเป็นหัวใจสำคัญของการใช้งาน VM ที่สะดวกสบาย
   
    - Display Driver ไดรเวอร์จอภาพเสมือน (Virtual Display Driver) จะถูกติดตั้งเข้าไปเพื่อแทนที่ไดรเวอร์พื้นฐาน (เช่น Standard VGA) ที่มากับ Guest OS ไดรเวอร์นี้จะสื่อสารโดยตรงกับ VirtualBox เพื่อ: 1. ปรับปรุงประสิทธิภาพการแสดงผลกราฟิก 2. อนุญาตให้ปรับความละเอียดหน้าจอ (Screen Resolution) ของ Guest OS ให้เข้ากับขนาดหน้าต่าง VM โดยอัตโนมัติ (Autoresize) และ 3. เปิดใช้งานคุณสมบัติ 2D/3D Video Acceleration (หากตั้งค่าไว้)
   
    - Shared Folders เปิดใช้งานการแชร์ไดเรกทอรีระหว่าง Host OS และ Guest OS
   
    - Time Synchronization ช่วยให้ Guest OS มีเวลาที่ตรงกับ Host OS อยู่เสมอ
    
56. ข้อใดเป็นการปรับจูน (Tuning) เพื่อเพิ่มประสิทธิภาพของ VM

    A) ปิด Ballooning

    B) ใช้ VirtIO driver สำหรับ Disk/Network

    C) ปิด NUMA

    D) ใช้ Snapshot ต่อเนื่อง

    คำตอบ: B

    อธิบาย: การใช้ VirtIO drivers สำหรับ disk/network เป็นการปรับจูนสำคัญ — ลด overhead ของ emulated devices, เพิ่ม throughput และลด latency อีกวิธีคือ NUMA tuning, hugepages, CPU pinning, และ storage tuning

57. ในระบบ Cloud เช่น Azure, “Availability Set” เกี่ยวข้องกับอะไรของ VM

    A) การกระจาย VM หลายเครื่องข้าม Host เพื่อความทนทานสูง

    B) การรวม VM เข้าด้วยกัน

    C) การทำ Snapshot

    D) การบีบอัด Disk

    คำตอบ: A

    อธิบาย: Availability Set ใน Azure ช่วย กระจาย VM ข้าม physical hosts / fault domains และ update domains เพื่อเพิ่ม availability ของ application — ลดโอกาส downtime ถ้ามี host failure หรือ during maintenance

58. “VM Escape Attack” คืออะไร

    A) การที่ผู้ใช้ VM ออกจากระบบ

    B) การโจมตีที่หลุดจาก Guest VM ไปถึง Host OS

    C) การทำลาย Snapshot

    D) การโจมตี Network

    คำตอบ: B

    อธิบาย: VM Escape เป็นการโจมตีที่ attacker ใน guest สามารถหลุดออกไปควบคุม host หรือ hypervisor ได้ — ทำลาย isolation เป็นความเสี่ยงร้ายแรง ต้อง patch hypervisor และลดการรัน code ที่ไม่น่าเชื่อถือใน environment สำคัญ

59. ถ้า VM ทำงานช้าแม้ Host CPU ยังเหลือมาก มักเกิดจากสาเหตุใด

    A) Disk I/O bottleneck หรือ vStorage ถูกแชร์มากเกินไป

    B) CPU เสีย

    C) BIOS ตั้งผิด

    D) OS ติดไวรัส

    คำตอบ: A

    อธิบาย: ถ้า VM ช้าแม้ host CPU เหลือมาก สาเหตุส่วนใหญ่คือ disk I/O bottleneck หรือ contention ใน vStorage (เช่น noisy neighbor, slow storage array, snapshot chain) — ควรดู metrics IOPS, latency, queue depth

60. “Hypervisor Scheduling” คืออะไร

    A) การจัดการลำดับการประมวลผล vCPU ให้แบ่งใช้ทรัพยากร Host CPU

    B) การตั้งเวลา Snapshot

    C) การจัดการ Network Traffic

    D) การอัปเดต OS

    คำตอบ: A

    อธิบาย: Hypervisor scheduling เป็นการ จัดการ mapping/เวลาให้ vCPU ใช้ pCPU — algorithms ต่าง ๆ (round-robin, fair share, real-time) มีผลต่อ CPU ready time และ performance ของ VM

61. การสำรองข้อมูล VM แบบ “Cold Backup” หมายถึงอะไร

    A) Backup ระหว่างที่ VM กำลังทำงานอยู่

    B) Backup เมื่อ VM ปิดอยู่

    C) Backup ผ่านเครือข่ายเท่านั้น

    D) Backup เฉพาะ Snapshot

    คำตอบ: B

    อธิบาย: Cold backup คือการสำรองข้อมูล ขณะที่ VM ปิดอยู่ (offline) — ข้อดีคือ consistency ง่าย (no writes during backup) แต่มี downtime ต่างจาก hot backup ที่ต้องทำขณะที่ VM ยังทำงาน

62. ถ้าในระบบ Cloud มีการคิดค่าบริการแบบ “Reserved Instance” แตกต่างจาก “Pay-as-you-go” อย่างไร

    A) Reserved Instance จ่ายตามการใช้งานจริง

    B) Reserved Instance เหมาจ่ายล่วงหน้าเพื่อรับส่วนลด

    C) Pay-as-you-go เหมาจ่ายรายเดือน

    D) ทั้งสองแบบฟรี

    คำตอบ: B

    อธิบาย: Reserved Instance เป็นการจ่ายล่วงหน้า/จอง capacity เพื่อแลกกับส่วนลด (เหมาะกับ workload คงที่) ต่างจาก pay-as-you-go ที่จ่ายตามการใช้งานจริงและยืดหยุ่นกว่า

    <img width="972" height="606" alt="virtual machine01" src="https://github.com/user-attachments/assets/cad20cf4-d898-42c1-88d3-9495d9668b86" />
