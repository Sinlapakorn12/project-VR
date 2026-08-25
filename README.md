VR First Aid Training Game

> ระบบจำลองการฝึกปฐมพยาบาลเบื้องต้นในโลกเสมือนจริง (Virtual Reality) เพื่อฝึกทักษะการตัดสินใจ ลำดับขั้นตอนการปฐมพยาบาล และประเมินผลผู้ใช้งานแบบ Real-time

---

ภาพรวมโปรเจกต์ (Project Overview)

โปรเจกต์นี้พัฒนาขึ้นเพื่อเพิ่มประสิทธิภาพการเรียนรู้ด้านการปฐมพยาบาลฉุกเฉิน โดยนำเทคโนโลยี VR มาจำลองสถานการณ์ที่มีความสมจริง ลดความเสี่ยงในการฝึกจริง และเปิดโอกาสให้ผู้เรียนฝึกฝนซ้ำได้ไม่จำกัด

ฟีเจอร์หลัก (Key Features)

1. **6 First Aid Scenarios (สถานการณ์จำลอง 6 รูปแบบ):**
   - การดูแลรักษาแผลถลอก (Abrasion Wound Care)
   - การห้ามเลือดและทำแผลฉีกขาด (Laceration & Bleeding Management)
   - สถานการณ์ฉุกเฉินทางการแพทย์อื่นๆ รวม 6 เคส
2. **Physics & VR Interaction:**
   - หยิบ จับ และใช้งานอุปกรณ์ปฐมพยาบาล (ผ้าก๊อซ, น้ำเกลือล้างแผล, สำลี, ผ้าพันแผล)
   - ตรวจจับความถูกต้องของตำแหน่งและลำดับการทำหัตถการ
3. **Scoring & Evaluation System:**
   - คำนวณคะแนนตามความแม่นยำ ลำดับขั้นตอน และเวลาที่ใช้
   - ระบบสรุปผลและตัดเกรด/อันดับ (Rank S, A, B, C)
4. **Statistics & Attempts Tracking:**
   - บันทึกประวัติการฝึกฝน จำนวนครั้งที่ทดสอบ (Total Attempts) และคะแนนสูงสุด

---

 Tech Stack & Hardware

- **Game Engine:** Unity (C#)
- **VR Framework / SDK:** XR Interaction Toolkit / OpenXR
- **Target Platform:** Meta Quest 2 / Meta Quest 3 / PCVR
- **Architecture:** State Pattern (Scenario Logic), Event-Driven Architecture (Interaction System)

---

System Architecture & Workflow

```text
[ Main Menu ] 
     │
     ├──► [ Scenario Selection (6 Cases) ]
     │          │
     │          ▼
     │    [ VR Interactive Gameplay ]
     │    ├─ Tool Grabbing & Interaction
     │    ├─ Step-by-Step Validation
     │    └─ Timer & Action Tracker
     │          │
     │          ▼
     └──► [ Evaluation & Scoring Screen ]
          ├─ Accuracy Score
          ├─ Time Taken
          └─ Rank & Summary
