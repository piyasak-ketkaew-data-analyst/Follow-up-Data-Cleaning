# Follow-up-Data-Cleaning
Cleaning Data and Follow up by Automation
## 🚀 **ขั้นตอนการ Implementation**

### **Phase 1: Setup (1-2 วัน)**
1. ✅ เตรียม Excel File บน OneDrive/SharePoint
2. ✅ สร้าง Table ทั้ง 4 Sheets
3. ✅ ใส่ข้อมูลตัวอย่าง
4. ✅ Test Connection จาก Power Automate

### **Phase 2: Build Flow 1 - Data Validation (2-3 วัน)**
1. ✅ สร้าง Trigger + List rows
2. ✅ ทำ Validation Logic ทีละ Rule
3. ✅ Test แต่ละ Condition
4. ✅ เขียน Error Report
5. ✅ ทดสอบส่งอีเมล Error Summary

### **Phase 3: Build Flow 2 - Follow-up (3-4 วัน)**
1. ✅ ดึงข้อมูล Tickets ที่ต้อง Follow-up
2. ✅ ทำ Group by Email Logic
3. ✅ สร้าง HTML Template
4. ✅ ทดสอบส่งอีเมล (เริ่มจาก 1-2 Emails)
5. ✅ เพิ่ม Error Handling
6. ✅ บันทึก Log

### **Phase 4: Build Flow 3 - Report (2 วัน)**
1. ✅ ดึงข้อมูลจาก Log
2. ✅ คำนวณ Metrics
3. ✅ สร้าง Report Template
4. ✅ Schedule การส่ง

### **Phase 5: Testing & Go-Live (2-3 วัน)**
1. ✅ Test End-to-End ด้วยข้อมูลจริง
2. ✅ ปรับแต่งตาม Feedback
3. ✅ เปิดใช้งาน Production

---

## 💡 **Tips & Best Practices**

### **1. Error Handling**
```
Scope Action (Try-Catch Pattern):
- Scope "Try": [Main Logic]
- Scope "Catch":
  Configure run after: has failed, has timed out
  Action: Send error notification + Log error
