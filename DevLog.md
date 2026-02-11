RU-LAR

Secure Real-time Learning and Interaction System

Project Overview

RU-LAR เป็นระบบ Secure Real-time Learning and Interaction System ที่พัฒนาขึ้นเพื่อเพิ่มการมีส่วนร่วมของนักศึกษาในห้องเรียน โดยเน้นการสื่อสารแบบ Anonymous Participation และการแสดงผลข้อมูลแบบ Real-time ภายใต้การออกแบบที่คำนึงถึง Security by Design

ระบบมีเป้าหมายเพื่อช่วยให้อาจารย์สามารถมองเห็นระดับความเข้าใจและการมีส่วนร่วมของผู้เรียนได้ชัดเจนมากขึ้น รวมถึงช่วยตรวจจับนักศึกษาที่มีพฤติกรรมเงียบ (Silent Student) แต่ยังอาจไม่เข้าใจเนื้อหาที่เรียนอยู่

Problem Statement

ในสภาพแวดล้อมการเรียนการสอนแบบดั้งเดิม พบว่านักศึกษาจำนวนมาก

ไม่กล้าแสดงความคิดเห็น

ไม่กล้าถามคำถามในที่สาธารณะ

ขาดช่องทางการมีส่วนร่วมแบบ Real-time

ส่งผลให้อาจารย์ไม่สามารถประเมินระดับความเข้าใจของผู้เรียนได้อย่างแม่นยำระหว่างการสอน

RU-LAR จึงถูกพัฒนาขึ้นเพื่อแก้ไขปัญหานี้ โดยสร้างแพลตฟอร์มที่ปลอดภัย เปิดโอกาสให้ผู้เรียนมีส่วนร่วมโดยไม่เปิดเผยตัวตน และส่งข้อมูลตอบกลับให้อาจารย์แบบ Real-time

Project Objectives

เปิดโอกาสให้นักศึกษาสามารถส่งคำถามและตอบโพลได้แบบ Anonymous

แสดงผลการมีส่วนร่วมของผู้เรียนแบบ Real-time

สนับสนุนอาจารย์ในการตรวจจับ Silent Student

ช่วยให้อาจารย์สามารถปรับการสอนได้จากข้อมูลจริง (Data-driven Teaching)

ออกแบบระบบโดยคำนึงถึง Security ตั้งแต่ขั้นตอนการออกแบบ

System Roles

ระบบ RU-LAR รองรับผู้ใช้งานหลัก 3 บทบาท

Student

เข้าร่วม Session ห้องเรียนด้วย QR Code หรือ Room Code

ส่งคำถามแบบไม่เปิดเผยตัวตน

ตอบ Poll และ Voting

ดูผลโหวตและคำถามที่ได้รับการอนุมัติแบบ Real-time

Teacher

Login และจัดการ Session ห้องเรียน

สร้างและควบคุม Poll และ Q&A

ดูผลการตอบสนองและ Engagement Analytics

ทำ Content Moderation เช่น ซ่อนหรือ ลบ ข้อความที่ไม่เหมาะสม

Admin

จัดการผู้ใช้งานและกำหนด Role

ตรวจสอบ System Log

กำหนดและบังคับใช้นโยบายด้าน Security

Core Features

Secure Authentication ผ่าน External Identity Provider

Session-based Classroom Interaction

Anonymous Q&A

Live Polling และ Voting

Real-time Data Synchronization

Content Moderation และ Abuse Control

Engagement Analytics สำหรับการเรียนการสอน

System Architecture (High-Level)

RU-LAR ถูกออกแบบในรูปแบบ Session-based Architecture
โดยทุกกิจกรรมของผู้ใช้จะต้องอยู่ภายใต้ Session ที่ถูกต้อง

ระบบมีการกำหนด Trust Boundary อย่างชัดเจนระหว่าง

Client (Student / Teacher)

Application Services

External Services

Database

องค์ประกอบหลักของระบบประกอบด้วย

Authentication Service

Session Management Service

Message Submission Service

Moderation Service

Overlay Display Service

Real-time Communication Service

Threat Modeling Approach

การวิเคราะห์ความเสี่ยงด้านความปลอดภัยของระบบ RU-LAR ดำเนินการโดยใช้ Microsoft Threat Modeling Tool (TMT)

การวิเคราะห์แบ่งออกเป็น 3 Layer ได้แก่

Context Layer (Layer 0): ระบุ External Entity, Data Flow และ Trust Boundary

Process Layer (Layer 1): วิเคราะห์ Process หลักของระบบ

Subprocess Layer (Layer 2): แตก Process เป็นขั้นตอนการทำงานจริงของระบบ

แนวทางนี้ช่วยให้สามารถระบุ Threat ได้ตั้งแต่ระยะเริ่มต้นของการออกแบบระบบ และนำไปสู่การวาง Mitigation ที่เหมาะสม

Technology Stack

โครงงาน RU-LAR ถูกพัฒนาโดยใช้เทคโนโลยีที่เหมาะสมกับระบบ Real-time Web Application โดยคำนึงถึงความสามารถในการขยายระบบ ความปลอดภัย และความสะดวกในการพัฒนา

Software Management

GitHub
ใช้สำหรับ Version Control และการจัดการ Source Code ของโครงงาน

Discord
ใช้เป็นช่องทางหลักในการสื่อสาร ประชุม และประสานงานภายในทีม

Notion
ใช้สำหรับจัดการเอกสารโครงงาน แผนงาน และการติดตามความคืบหน้า

Design Tools

Figma
ใช้สำหรับออกแบบ User Interface (UI) และ User Experience (UX)
รวมถึงการสร้าง Mockup และ Prototype ของระบบก่อนการพัฒนา

Front End

React
ใช้สำหรับพัฒนา User Interface แบบ Component-based

Tailwind CSS
ใช้สำหรับจัดการ Styling ของหน้าเว็บ เพื่อความยืดหยุ่นและความรวดเร็วในการพัฒนา

Back End

Node.js
ใช้เป็น Runtime Environment สำหรับฝั่ง Server

Socket.IO
ใช้สำหรับการสื่อสารแบบ Real-time ระหว่าง Client และ Server
รองรับการส่งข้อมูล เช่น Q&A, Poll และ Voting แบบทันที

Database

PostgreSQL
ใช้เป็น Relational Database สำหรับจัดเก็บข้อมูลผู้ใช้
ข้อมูล Session ห้องเรียน และข้อมูลการมีส่วนร่วมของผู้เรียน

Infrastructure

Docker
ใช้สำหรับ Containerization เพื่อให้ระบบสามารถทำงานได้อย่างสม่ำเสมอ
ในทุกสภาพแวดล้อมการพัฒนาและการ Deploy

Current Progress

วิเคราะห์ปัญหาและความต้องการของผู้ใช้งานเรียบร้อยแล้ว

กำหนด System Role และ Core Features ครบถ้วน

ออกแบบ System Architecture ระดับภาพรวม

ดำเนินการ Threat Modeling ครบทั้ง 3 Layer

จัดทำเอกสารสำหรับรายงานความคืบหน้าโครงงาน

Next Steps

วิเคราะห์ Threat ตาม STRIDE Model

กำหนด Mitigation สำหรับ Threat ที่มีความเสี่ยงสูง

จัดทำ Data Flow Diagram (DFD) อย่างเป็นทางการ

พัฒนา Prototype ของระบบ

ทดสอบการใช้งานจาก Scenario ห้องเรียนจริง

Project Status

โครงงานนี้อยู่ในระหว่างการพัฒนาในรูปแบบ Prototype
เพื่อใช้ในการศึกษา ออกแบบ และประเมินแนวคิดเชิงระบบและความปลอดภัย
