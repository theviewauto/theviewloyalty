# 📥 THE VIEW GROUP - Installation Guide

## 4️⃣ **วิธีติดตั้ง (เลือกตามสถานการณ์)**

---

## **วิธี 1️⃣: Local Installation (ง่ายสุด) 🏠**

### สถานการณ์ที่เหมาะ:
```
✓ อู่เดียว
✓ ต้องการใช้ offline
✓ ไม่ต้องแชร์ข้อมูล
✓ Setup อย่างรวดเร็ว
```

### ขั้นตอนการติดตั้ง:

#### **1. ดาวน์โหลดไฟล์**
```
1. Download ไฟล์ทั้งหมด (8 ไฟล์)
2. สร้าง Folder: "THE_VIEW_Loyalty"
3. วางไฟล์ทั้งหมด เข้าโฟลเดอร์นี้
```

#### **2. ทำการ Setup**
```
Windows:
  → คลิก index.html ด้วย Chrome/Edge
  → Browser เปิดโดยอัตโนมัติ

Mac:
  → Double-click index.html
  → เลือก "Safari" หรือ "Chrome"

Mobile:
  → โอนไฟล์ไปที่ phone ผ่าน USB
  → ใช้ app "HTML Viewer" (ฟรี)
```

#### **3. ใช้งาน**
```
1. เปิด: index.html
2. เห็น 3 ปุ่ม
3. Admin/Customer/Badge ทั้งหมดใช้ได้
4. ข้อมูลเก็บในเบราว์เซอร์ (localStorage)
```

### ✅ **Pros:**
- ติดตั้ง 30 วินาที
- ใช้ offline ได้
- ไม่ต้องเซิร์ฟเวอร์
- ฟรี (ไม่มีค่าใช้)

### ❌ **Cons:**
- ข้อมูลเก็บที่ browser เดียว (ต้อง export CSV)
- ไม่ sync ต่อคน
- Multi-device ต้องใช้ LAN/Vercel

---

## **วิธี 2️⃣: LAN Network Installation (Share ใน Network) 🌐**

### สถานการณ์ที่เหมาะ:
```
✓ อู่ + เคาน์เตอร์ + Boss
✓ ต้องใช้ร่วมกัน (เชื่อมเน็ต)
✓ ข้อมูลอยู่ที่ server เดียว
✓ ประหยัดค่าเซิร์ฟเวอร์
```

### ขั้นตอน:

#### **1. ติดตั้ง Local (like วิธี 1)**
```
Computer A (Server/Boss):
  → Folder: C:\THE_VIEW_Loyalty\
  → เก็บไฟล์ทั้งหมด
  → เปิด index.html
```

#### **2. Set Up Web Server**
```
ใช้ Python (ฟรี - มักมี Mac/Linux)

Windows:
  1. ดาวน์โหลด Python: python.org
  2. Install with "Add Python to PATH"
  3. Open CMD → ไปที่ folder
     cd C:\THE_VIEW_Loyalty
  4. Run:
     python -m http.server 8000
  5. Browser: http://localhost:8000

Mac/Linux:
  1. Open Terminal
  2. cd ~/THE_VIEW_Loyalty
  3. python3 -m http.server 8000
  4. Browser: http://localhost:8000
```

#### **3. เชื่อม Network**
```
หา IP Address ของเครื่อง Server:

Windows (CMD):
  ipconfig
  → ดูที่ "IPv4 Address" เช่น 192.168.1.100

Mac (Terminal):
  ifconfig
  → ดูที่ inet
```

#### **4. Access จาก Device อื่น**
```
Mobile/Computer อื่น (ที่อยู่ Network เดียวกัน):
  Browser: http://192.168.1.100:8000
  → เห็น index.html
  → ทุกคนใช้ได้ (ข้อมูลร่วมกัน)
```

### ✅ **Pros:**
- Share ข้อมูล realtime
- ใช้ได้หลาย device
- ไม่ต้องเซิร์ฟเวอร์ (ใช้เครื่องเดิม)
- ค่าใช้: 0 บาท

### ❌ **Cons:**
- ต้องมีเน็ตในออฟฟิส
- Server device ต้องปิดไว้ตลอด
- Multi-branch ต้อง Vercel/Backend
- ความเร็วขึ้นอยู่กับ WiFi

---

## **วิธี 3️⃣: Vercel Deployment (Online - ดีที่สุด) 🚀**

### สถานการณ์ที่เหมาะ:
```
✓ Multi-branch (THE VIEW GROUP)
✓ ลูกค้าเข้าจากที่ไหนก็ได้
✓ URL สาธารณะ
✓ Scalable (1000+ ลูกค้า)
```

### ขั้นตอนติดตั้ง:

#### **1. Prepare Files**
```
GitHub Repo (ฟรี):
  1. เข้า: github.com
  2. Sign Up (ฟรี)
  3. Create New Repository: "THE_VIEW_Loyalty"
  4. Upload ไฟล์ทั้งหมด
```

#### **2. Deploy to Vercel**
```
Step 1: เข้า vercel.com
Step 2: Sign up with GitHub (ฟรี)
Step 3: "New Project"
Step 4: Import your GitHub repo
Step 5: Deploy → ✓ ได้ URL
```

#### **3. ได้ URL**
```
Vercel จะให้ URL เช่น:
https://the-view-loyalty.vercel.app

Admin Panel:
https://the-view-loyalty.vercel.app/loyalty_with_registration.html

Customer Portal:
https://the-view-loyalty.vercel.app/customer-portal.html

Badge Generator:
https://the-view-loyalty.vercel.app/qr-badge-generator.html
```

#### **4. Share QR/Link**
```
สร้าง QR badge ที่มี URL:
https://the-view-loyalty.vercel.app/customer-portal.html

ลูกค้า Scan → เข้า Portal ได้ทันที
```

### ✅ **Pros:**
- URL สาธารณะ (ทั้งประเทศใช้ได้)
- 24/7 online
- Scalable สำหรับ 1000+ ลูกค้า
- ฟรี (Vercel ฟรี 1000 functions/month)
- Realtime sync

### ❌ **Cons:**
- ต้องมี GitHub account (ฟรี)
- ต้อง Internet connection
- localStorage ไม่ sync ระหว่าง browser ✓ (Vercel สามารถเพิ่ม API)

---

## **วิธี 4️⃣: Google Drive Shortcut (เร็วสุด) 📁**

### สถานการณ์ที่เหมาะ:
```
✓ ใช้ offline เหมือน Local
✓ Backup อัตโนมัติ
✓ Access จาก Phone/Tablet
✓ ไม่ต้อง GitHub/Vercel
```

### ขั้นตอน:

#### **1. Upload ไปที่ Google Drive**
```
1. เข้า: drive.google.com
2. สร้าง Folder: "THE_VIEW_Loyalty"
3. Upload ไฟล์ทั้งหมด
```

#### **2. ใช้ Hosted on Google Drive**
```
ไม่ได้ (Google Drive ไม่ให้ run HTML ตรงๆ)

แต่สามารถใช้ด้วย:
  A. ดาวน์โหลด + ใช้ Local
  B. ใช้ Google Drive ถ้า convert เป็น Google Apps Script
```

### Alternative: **GitHub Pages (ฟรี like Vercel)**
```
1. GitHub Repo
2. Settings → Pages
3. Branch: main
4. ได้ URL: yourusername.github.io/THE_VIEW_Loyalty

ฟรี + Online + Custom domain ได้
```

---

## 🎯 **เลือกวิธีไหน?**

### **ผู้ใช้ที่ต้องการ...**

| ต้องการ | วิธี | ค่าใช้ |
|--------|------|-------|
| เร็ว + เรียบง่าย | 1️⃣ Local | ฟรี |
| ใช้ร่วมกัน (1 อู่) | 2️⃣ LAN | ฟรี |
| ทั้งประเทศ + Online | 3️⃣ Vercel | ฟรี |
| บ้าน + Backup | 4️⃣ Google Drive | ฟรี |

---

## 📋 **Step-by-Step: Local Installation (ง่ายสุด)**

### **Windows:**
```
1. Download ไฟล์ 8 ไฟล์
   └─ index.html
   └─ loyalty_with_registration.html
   └─ customer-portal.html
   └─ qr-badge-generator.html
   └─ README.md
   └─ QUICK_START_GUIDE.md
   └─ THE_VIEW_SETUP_GUIDE.md
   └─ PDPA_COMPLIANCE_GUIDE.md

2. สร้าง Folder: C:\THE_VIEW_Loyalty

3. วางไฟล์ลงใน Folder

4. Double-click: index.html

5. Chrome/Edge เปิดโดยอัตโนมัติ

6. ✓ Ready to use!
```

### **Mac:**
```
1-3. Same as Windows

4. Right-click: index.html
   → Open with → Chrome/Safari

5. ✓ Ready to use!
```

### **Mobile (iOS/Android):**
```
iPhone:
  1. Share ไฟล์ไปที่ iPhone
  2. ใช้ app "HTML Viewer" (ฟรี)
  3. Open index.html

Android:
  1. Copy ไฟล์ไปที่ /Documents/
  2. ใช้ app "Web Browser" หรือ "Chrome"
  3. Open index.html
```

---

## 🔧 **Troubleshooting**

### ❓ ฟรสิ่งเดิมปรากฏขึ้นได้ไหม?
**แก้:**
```
1. Ctrl+Shift+Delete → Clear All
2. Reload page
3. ลองเบราว์เซอร์ใหม่ (Chrome/Firefox)
```

### ❓ QR Code ไม่ทำงาน?
**แก้:**
```
1. ลองเปิด HTML ด้วย Chrome (ไม่ใช่ Safari)
2. ใช้ http:// ไม่ใช่ file://
3. Check browser console (F12)
```

### ❓ ข้อมูลหายไป?
**ป้องกัน:**
```
1. Export CSV ทุกสัปดาห์
2. Backup folder ทั้งหมด
3. ถ้า LAN → Backup server ด้วย
```

### ❓ ต้องแชร์ให้ branch อื่น?
**แก้:**
```
ใช้ Vercel (วิธี 3):
  → URL สาธารณะ
  → ลิงค์ให้ branch อื่น
  → ข้อมูล sync ได้ (Phase 2 with API)
```

---

## 📱 **URL สำหรับลูกค้า**

### **Local (ตัวเอง):**
```
file://C:/Users/YourName/THE_VIEW_Loyalty/customer-portal.html
```

### **LAN (ในเน็ต):**
```
http://192.168.1.100:8000/customer-portal.html
→ ส่ง SMS ลูกค้า
```

### **Vercel (Online):**
```
https://the-view-loyalty.vercel.app/customer-portal.html
→ Link ง่ายสุด
```

### **QR Code:**
```
สร้าง QR ชี้ไปยัง URL ที่เลือก
→ เก็บบัตร
→ ลูกค้า Scan = เข้า Portal
```

---

## ✅ **Checklist - ก่อน Go Live**

### **Local Installation:**
- [ ] ดาวน์โหลดไฟล์เสร็จ
- [ ] สร้าง folder "THE_VIEW_Loyalty"
- [ ] วางไฟล์เข้าโฟลเดอร์
- [ ] Double-click index.html
- [ ] Browser เปิด + เห็น 3 ปุ่ม
- [ ] ทดลอง Admin → Add customer
- [ ] ทดลอง Customer portal (OTP: 000000)
- [ ] ทดลอง Badge generator → print
- [ ] Export CSV ได้ไหม
- [ ] ✓ Ready!

### **LAN Installation:**
- [ ] Computer A setup Local เสร็จ
- [ ] Install Python (Windows)
- [ ] Run: python -m http.server 8000
- [ ] หา IP Address
- [ ] Test from Mobile: http://IP:8000
- [ ] ✓ ทำงานได้

### **Vercel Installation:**
- [ ] GitHub account สร้างเสร็จ
- [ ] Push ไฟล์ไป GitHub
- [ ] Vercel account สร้างเสร็จ
- [ ] Deploy สำเร็จ
- [ ] ได้ URL
- [ ] ทดลอง URL ได้ไหม
- [ ] ✓ Live!

---

## 🚀 **Recommended Setup**

### **สำหรับ THE VIEW GROUP (อู่เดียวตอนนี้):**
```
✅ วิธี 1: Local Installation
   - ปลอดภัย (เก็บบ้าน)
   - ใช้งานง่าย
   - Export CSV ทุกสัปดาห์

📅 อนาคต (Multi-branch):
   → Upgrade เป็น Vercel (Phase 2)
   → ลูกค้า branch อื่นเข้า portal ได้
   → Sync realtime ผ่าน API
```

---

## 📞 **ติดขัด?**

### **ทำไม?**
1. อ่าน: QUICK_START_GUIDE.md
2. ลอง: Troubleshooting section ข้างบน
3. Check: F12 Browser console
4. Export: CSV backup

### **ถ้ายังไม่ได้:**
1. ลัดเลาะใหม่ (ขั้นตอนง่ายๆ)
2. ลอง browser ใหม่ (Chrome recommended)
3. Clear cache + reload
4. ให้ screenshot + error message

---

## 🎉 **ติดตั้งเสร็จแล้ว!**

```
✓ THE VIEW GROUP Loyalty System
✓ Ready to Launch
✓ Go live!

คำแนะนำ:
  1. ทดลองทั้งหมด 30 นาที
  2. Export CSV (backup)
  3. Train staff ให้รู้
  4. Announce ลูกค้า
  5. Launch! 🚀
```

---

**Questions?** ติดขัดเรื่องไหน บอกมา ฉันช่วยเลย! 💚

