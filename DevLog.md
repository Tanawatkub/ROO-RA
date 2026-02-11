# RU-LAR
## Secure Real-time Learning and Interaction System

---

## Project Overview

RU-LAR เป็นระบบ Secure Real-time Learning and Interaction System ที่พัฒนาขึ้นเพื่อส่งเสริมการมีส่วนร่วมของนักศึกษาในห้องเรียน โดยรองรับการโต้ตอบแบบ Real-time และการมีส่วนร่วมแบบไม่เปิดเผยตัวตน (Anonymous Participation)

ระบบถูกออกแบบภายใต้แนวคิด Security by Design และใช้กระบวนการ Threat Modeling ในการวิเคราะห์ความเสี่ยงตั้งแต่ระดับสถาปัตยกรรม

---

## Problem Statement

ในห้องเรียนทั่วไป นักศึกษาจำนวนมาก:

- ไม่กล้าแสดงความคิดเห็น  
- ไม่กล้าถามคำถามในที่สาธารณะ  
- ขาดช่องทางการมีส่วนร่วมแบบ Real-time  
- กลายเป็น Silent Student แม้ยังไม่เข้าใจเนื้อหา  

ส่งผลให้อาจารย์ไม่สามารถประเมินระดับความเข้าใจของผู้เรียนได้อย่างแม่นยำระหว่างการสอน

RU-LAR จึงถูกพัฒนาขึ้นเพื่อแก้ไขปัญหาดังกล่าว ด้วยแพลตฟอร์มที่ปลอดภัยและสนับสนุนการมีส่วนร่วมอย่างเป็นระบบ

---

## Project Objectives

1. เปิดโอกาสให้นักศึกษาส่งคำถามและตอบโพลแบบ Anonymous  
2. แสดงผลการมีส่วนร่วมแบบ Real-time  
3. สนับสนุนการตรวจจับ Silent Student  
4. ส่งเสริม Data-driven Teaching  
5. ออกแบบระบบโดยคำนึงถึง Security ตั้งแต่ต้นทาง  

---

## System Roles

### Student
- เข้าร่วม Session ผ่าน QR Code หรือ Room Code  
- ส่งคำถามแบบไม่เปิดเผยตัวตน  
- ตอบ Poll และ Voting  
- ดูผลลัพธ์แบบ Real-time  

### Teacher
- Login และสร้าง Session ห้องเรียน  
- สร้างและควบคุม Poll  
- ดู Engagement Analytics  
- ทำ Content Moderation  

### Admin
- จัดการผู้ใช้งานและกำหนด Role  
- ตรวจสอบ System Log  
- กำหนดนโยบายด้าน Security  

---

## Core Features

- Secure Authentication  
- Session-based Classroom Interaction  
- Anonymous Q&A  
- Live Polling และ Voting  
- Real-time Communication (WebSocket)  
- Content Moderation  
- Engagement Analytics Dashboard  

---

## System Architecture

RU-LAR ใช้แนวคิด Session-based Architecture โดยกำหนด Trust Boundary อย่างชัดเจนระหว่าง:

- Client Layer  
- Application Services  
- External Services  
- Database Layer  

องค์ประกอบหลักของระบบประกอบด้วย:

- Authentication Service  
- Session Management Service  
- Message Submission Service  
- Moderation Service  
- Real-time Communication Service  
- Database Service  

---

## Threat Modeling Approach

โครงงานใช้ Microsoft Threat Modeling Tool (TMT) ในการวิเคราะห์ความเสี่ยง โดยแบ่งการวิเคราะห์เป็น 3 Layer:

### Layer 0 – Context Layer
- ระบุ External Entity  
- วิเคราะห์ Data Flow  
- กำหนด Trust Boundary  

### Layer 1 – Process Layer
- วิเคราะห์ Process หลักของระบบ  

### Layer 2 – Subprocess Layer
- แตกกระบวนการทำงานเป็นขั้นตอนย่อย  
- วิเคราะห์ Threat ในระดับลึก  

แนวทางนี้ช่วยให้สามารถกำหนด Mitigation Strategy ได้อย่างเป็นระบบ

---

## Technology Stack

### Software Management
- GitHub  
- Discord  
- Notion  

### Design Tools
- Figma  

### Front End
- React  
- Tailwind CSS  

### Back End
- Node.js  
- Socket.IO  

### Database
- PostgreSQL  

### Infrastructure
- Docker  

---

## Current Progress

- วิเคราะห์ Requirement เรียบร้อย  
- กำหนด Role และ Feature ครบถ้วน  
- ออกแบบ System Architecture  
- ดำเนินการ Threat Modeling ครบ 3 Layer  
- จัดทำเอกสารความคืบหน้าโครงงาน  

---

## Next Steps

- วิเคราะห์ Threat ตาม STRIDE Model  
- จัดทำ Data Flow Diagram (DFD)  
- กำหนด Mitigation Strategy  
- พัฒนา Prototype  
- ทดสอบระบบใน Scenario ห้องเรียนจริง  

---

## Project Status

อยู่ระหว่างการพัฒนา Prototype  
เพื่อศึกษาแนวคิดด้าน Real-time System และ Security Engineering ในบริบทการศึกษา

---
