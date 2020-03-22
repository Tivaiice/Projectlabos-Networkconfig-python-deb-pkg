# Network Configuration Project

โครงงานนี้เป็นส่วนหนึ่งของวิชา Computer System Laboratory รหัสวิชา 03603322  
เป็นการประยุต์ใช้เครื่องมือในการตั้งค่าเพื่อเชื่อมต่อเครือข่าย( Networking Tools ) ซึ่งที่มาของ IP Address มาจาก DHCP Server หรือ Manual Setting  ผู้จัดทำได้นำบทเรียนที่เรียนในห้องมาประยุกต์ โดยสร้าง GUI python เพื่อรับข้อมูลจากผู้ใช้งาน
## Members

1. นางสาวกนิษฐา พุ่มผล          5930300011  
2. นายทิวา      วงศ์รัตน์กตัญญู    5930300283

## Getting Started

ผู้ใช้จะต้องทำการติดตั้ง ubuntu-18.04.4-desktop ใน Oracle VM VirtualBox ติดตั้งแพ็คเกจ python3 และ idle3

```
sudo apt-get update
sudo apt-get install python3
sudo apt-get install idle3
```

### Prerequisites

* Check version python (3.5+)

```
python3 --version
```
### Installing
คำแนะนำ: ควรสร้าง Directory ขึ้นมาใหม่ 

* Download Package Project 
```
git clone https://github.com/Tivaiice/Projectlabos-Networkconfig-python-deb-pkg.git
```
* ติดตั้ง Package Project

```
sudo dpkg -i nwconfig_1.0.2_all.deb
```
## Running the package project

```
sudo nwc-network-config.py
```
output: จะได้เป็น GUI Python ขึ้นมา
## How to use

ผู้ใช้สามารถ ตั้งค่า IP Address ได้ 2 รูปแบบ คือ  
  *  Stactic IP
  *  Dynamic IP

#### ตัวอย่างการตั้งค่า IP Address
*   Stactic IP
```
DHCP4: false
Addresses: [ 10.64.194.192/23 ]
Gateway4: 10.64.194.1
Nameserveres:
    Addresses: [ 158.108.0.2,158.108.0.3 ]
```
*   Dynamic IP
```
DHCP4: true
Addresses: 
Gateway4: 
Nameserveres:
    Addresses: 
```
และเมื่อผู้ใช้ทำการใส่ข้อมูลสำเร็จให้กดปุ่ม Save เพื่อทำการตั้งค่า IP Address ( DHCP Server )






