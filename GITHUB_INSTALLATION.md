# 🐙 THE VIEW - GitHub & Vercel Installation Guide

## 📖 **ติดตั้งผ่าน GitHub (ละเอียด)**

---

## **เหตุผลใช้ GitHub?**

```
✅ Code Version Control (เก็บ history)
✅ Easy Deployment (ไป Vercel/Deploy ต่อได้)
✅ Backup (Cloud)
✅ Shareable (Link ให้ branch อื่นได้)
✅ Free (GitHub ฟรี)
✅ Professional (Management ดู)
```

---

## 🎯 **Step 1: สร้าง GitHub Account**

### **ขั้นตอน:**

#### 1. เข้า GitHub
```
1. ไปที่: github.com
2. ดูหน้า Home → มีปุ่ม "Sign up"
3. Click "Sign up"
```

#### 2. ลงทะเบียน
```
Form:
  ├─ Email: your.email@gmail.com
  ├─ Password: ตั้งรหัสผ่าน
  ├─ Username: theview_loyalty (ตัวอย่าง)
  └─ Marketing: ติ๊ก หรือ ไม่ติ๊กก็ได้

Click "Create account"
```

#### 3. ยืนยัน Email
```
1. GitHub ส่ง email ยืนยัน
2. เข้า Gmail → หา email จาก GitHub
3. Click link "Verify email address"
4. ✓ Account สร้างเสร็จ
```

#### 4. Setup Profile (ไม่บังคับ)
```
1. GitHub ให้เลือก:
   - Repository type
   - Interests
2. Skip ได้ → Click "Skip this"
3. ✓ เข้า Dashboard
```

---

## 🎯 **Step 2: สร้าง Repository (เก็บโค้ด)**

### **ขั้นตอน:**

#### 1. เข้า Dashboard
```
1. Login แล้ว → หน้า Home
2. มีปุ่ม "New" (สีเขียว)
3. Click "New"
```

#### 2. สร้าง Repository ใหม่
```
Form:
  ├─ Repository name: THE_VIEW_Loyalty
  ├─ Description: THE VIEW GROUP Loyalty Management System
  ├─ Public: ✓ Select (ให้ทุกคนเห็นได้)
  ├─ Add README: ✓ Checked
  ├─ .gitignore: None
  └─ License: None

Click "Create repository"
```

#### 3. ✓ Repository สร้างเสร็จ
```
ได้ URL: github.com/your-username/THE_VIEW_Loyalty

เช่น: github.com/theview-shop/THE_VIEW_Loyalty
```

---

## 🎯 **Step 3: Upload ไฟล์ไป GitHub**

### **วิธี 1: Upload ผ่าน Web Interface (ง่ายสุด)**

#### 1. เข้า Repository
```
1. ไปที่: github.com/your-username/THE_VIEW_Loyalty
2. เห็น folder ว่าง
3. มีปุ่ม "Add file"
4. Click "Upload files"
```

#### 2. เลือกไฟล์
```
1. Click "choose your files"
2. เลือกไฟล์ 8 ไฟล์:
   ├─ index.html
   ├─ loyalty_with_registration.html
   ├─ customer-portal.html
   ├─ qr-badge-generator.html
   ├─ README.md
   ├─ QUICK_START_GUIDE.md
   ├─ THE_VIEW_SETUP_GUIDE.md
   └─ PDPA_COMPLIANCE_GUIDE.md
3. Drag & drop ได้ด้วย
```

#### 3. Commit (บันทึก)
```
Commit message:
  "Initial commit - THE VIEW Loyalty System"

Commit directly to the main branch:
  ✓ Selected

Click "Commit changes"
```

#### 4. ✓ Upload เสร็จ
```
ไฟล์ทั้งหมดปรากฏใน Repository
```

---

### **วิธี 2: Upload ผ่าน Git Command (Pro)**

#### **สำหรับ Windows:**

##### 1. Install Git
```
1. ไปที่: git-scm.com
2. Click "Download"
3. ติดตั้ง (Next → Next → Finish)
4. Restart Computer
```

##### 2. Clone Repository
```
1. เปิด Command Prompt (Cmd)
2. ไปที่ folder ที่ต้องการ:
   cd C:\Users\YourName\Desktop

3. Clone:
   git clone https://github.com/your-username/THE_VIEW_Loyalty.git
   
4. เข้า folder:
   cd THE_VIEW_Loyalty
```

##### 3. Copy ไฟล์
```
1. Copy ไฟล์ 8 ไฟล์ลงใน folder:
   C:\Users\YourName\Desktop\THE_VIEW_Loyalty\

2. ตรวจสอบว่าไฟล์ทั้งหมดอยู่
```

##### 4. Push ไปยัง GitHub
```
ใน Command Prompt:

1. git status
   (ดูไฟล์ที่ยังไม่ได้ commit)

2. git add .
   (เพิ่มไฟล์ทั้งหมด)

3. git commit -m "Initial commit - THE VIEW Loyalty System"
   (บันทึก comment)

4. git push -u origin main
   (อัพโหลดไปยัง GitHub)

5. ✓ Upload เสร็จ
   (ดู GitHub browser → ไฟล์ทั้งหมดปรากฏ)
```

---

#### **สำหรับ Mac/Linux:**

##### 1. Install Git
```
Mac (ใช้ Homebrew):
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  brew install git

Linux:
  sudo apt-get install git
```

##### 2-4. Clone, Copy, Push (เหมือน Windows)
```
คำสั่งเดียวกับ Windows
ใช้ Terminal แทน Cmd
```

---

## 🎯 **Step 4: Deploy ไป Vercel (Make Online)**

### **ขั้นตอน:**

#### 1. เข้า Vercel
```
1. ไปที่: vercel.com
2. Click "Sign up"
3. Click "Continue with GitHub"
4. GitHub redirect → ยืนยัน
5. ✓ Login Vercel ด้วย GitHub
```

#### 2. Authorize Vercel
```
GitHub ถาม: "Authorize Vercel?"
  ✓ Click "Authorize vercel"

Vercel ถาม: Install Vercel?
  ✓ Click "Install"
```

#### 3. Create New Project
```
ใน Vercel Dashboard:
  1. Click "New Project"
  2. GitHub → Import Git Repository
```

#### 4. เลือก Repository
```
1. Search: "THE_VIEW_Loyalty"
2. เห็น Repository ปรากฏ
3. Click "Select"
```

#### 5. Configure Project
```
ตั้งค่า:
  ├─ Project Name: the-view-loyalty (auto)
  ├─ Framework Preset: Other (default)
  ├─ Build Command: (ว่าง - ใช้ default)
  └─ Output Directory: (ว่าง)

ปรับแต่ง Environment Variables:
  (ไม่ต้อง - HTML ไม่มี API)

Click "Deploy"
```

#### 6. ✓ Deploy เสร็จ
```
Vercel deploy และสร้าง URL:
  https://the-view-loyalty.vercel.app

รอ 30-60 วินาที → "Congratulations"
```

---

## 🎯 **Step 5: ตรวจสอบ URL**

### **ขั้นตอน:**

#### 1. ดู Dashboard
```
ไปที่: vercel.com → Dashboard
เห็น "the-view-loyalty" project
Click "Visit"
```

#### 2. ✓ เห็น Landing Page
```
URL: https://the-view-loyalty.vercel.app
→ Dashboard THE VIEW ปรากฏ
→ ปุ่ม 3 ปุ่ม (Admin/Customer/Badge)
```

#### 3. Test ทั้ง 3 ส่วน
```
✓ Admin Panel
  https://the-view-loyalty.vercel.app/loyalty_with_registration.html

✓ Customer Portal
  https://the-view-loyalty.vercel.app/customer-portal.html

✓ Badge Generator
  https://the-view-loyalty.vercel.app/qr-badge-generator.html
```

---

## 🎯 **Step 6: Create QR Code Badge**

### **ขั้นตอน:**

#### 1. เข้า Badge Generator
```
https://the-view-loyalty.vercel.app/qr-badge-generator.html
```

#### 2. ป้อนข้อมูล
```
- ชื่อ: ชื่อลูกค้า
- ID: 1001
- Tier: Gold
- Discount: 7-10%
```

#### 3. สร้าง QR
```
Click "🎨 สร้างตัวอย่าง"
→ เห็น 3 บัตร + QR Code
```

#### 4. QR ชี้ไปยัง
```
QR URL:
https://the-view-loyalty.vercel.app/customer-portal.html?phone=0812345678

ลูกค้า Scan → เข้า Portal ตรง ✓
```

#### 5. พิมพ์บัตร
```
Click "🖨️ พิมพ์บัตร"
Ctrl+P → Print → PDF / Printer
```

---

## 📱 **Step 7: Share Link ให้ลูกค้า**

### **4 วิธี:**

#### 1️⃣ **QR Badge (ดีที่สุด)**
```
ขั้นตอน:
  1. สร้าง QR ที่มี URL
  2. พิมพ์บัตร
  3. ลูกค้าเก็บบัตร
  4. ลูกค้า Scan QR
  5. ✓ เข้า Portal
```

#### 2️⃣ **SMS Link**
```
Text SMS:
  "สวัสดี! เช็คคะแนนที่นี่: 
   https://the-view-loyalty.vercel.app/customer-portal.html"
```

#### 3️⃣ **WhatsApp**
```
WhatsApp:
  "THE VIEW Loyalty Portal 🌟
   https://the-view-loyalty.vercel.app/customer-portal.html
   
   Scan QR บนบัตร หรือ Click link ได้"
```

#### 4️⃣ **Facebook / IG**
```
Post:
  "สมาชิก THE VIEW Loyalty! 
   Check คะแนนของคุณ:
   https://the-view-loyalty.vercel.app
   
   Scan QR บนบัตร"
```

---

## 🔄 **Update Code (หลัง Deploy)**

### **ถ้าต้องแก้ไข:**

#### 1. Edit ใน GitHub
```
1. ไปที่ GitHub Repository
2. หาไฟล์ที่ต้องแก้
3. Click pencil icon (Edit)
4. แก้ไขโค้ด
5. Commit changes
```

#### 2. Auto Deploy
```
Vercel auto detect:
  → GitHub เห็นการแก้ไข
  → Auto deploy ใหม่
  → Website update ใน 1-2 นาที
```

#### 3. ตรวจสอบ
```
1. ไปที่ URL
2. Ctrl+Shift+R (Hard refresh)
3. เห็นการเปลี่ยนแปลง
```

---

## 🐙 **Git Command Summary**

### **Commands ที่ใช้บ่อย:**

```bash
# Clone Repository
git clone https://github.com/username/THE_VIEW_Loyalty.git

# ดู Status
git status

# เพิ่มไฟล์
git add .              # Add ทั้งหมด
git add filename.html  # Add เฉพาะไฟล์

# Commit (บันทึก)
git commit -m "Message"

# Push ไปยัง GitHub
git push origin main

# Pull จาก GitHub
git pull origin main

# Undo commit ล่าสุด
git reset --soft HEAD~1

# Check log
git log --oneline
```

---

## 🎯 **GitHub URL Structure**

```
Repository:
  https://github.com/your-username/THE_VIEW_Loyalty

Website (Vercel):
  https://the-view-loyalty.vercel.app

Admin Panel:
  https://the-view-loyalty.vercel.app/loyalty_with_registration.html

Customer Portal:
  https://the-view-loyalty.vercel.app/customer-portal.html

Badge Generator:
  https://the-view-loyalty.vercel.app/qr-badge-generator.html

QR Code Link (ตัวอย่าง):
  https://the-view-loyalty.vercel.app/customer-portal.html?phone=0812345678
```

---

## 🛠️ **Troubleshooting**

### ❓ GitHub Login ไม่ได้
```
❌ สาเหตุ: Email ไม่ verify

✅ แก้:
  1. Check Gmail → หา email จาก GitHub
  2. Click "Verify email address"
  3. Refresh GitHub
  4. ลอง login ใหม่
```

### ❓ Upload ไม่ได้
```
❌ สาเหตุ: Browser cache

✅ แก้:
  1. Ctrl+Shift+Delete → Clear all
  2. Refresh page
  3. ลอง upload ใหม่
```

### ❓ Vercel Deploy Fail
```
❌ สาเหตุ: Build error

✅ แก้:
  1. Click "Deployments" ใน Vercel
  2. ดู "Build logs"
  3. Check error message
  4. Fix ใน GitHub
  5. Auto re-deploy
```

### ❓ QR Code ไม่ทำงาน
```
❌ สาเหตุ: URL ผิด

✅ แก้:
  1. Check QR URL ว่าเขียนถูกไหม
  2. Test URL ใน browser
  3. Regenerate QR ใหม่
  4. ดู https:// ไม่ใช่ http://
```

### ❓ Customer Portal ไม่ Sync
```
❌ สาเหตุ: Admin ใช้ Local, Customer ใช้ Online

✅ แก้:
  1. Admin ทั้งคู่ ใช้ Vercel URL (ไม่ใช่ local)
  2. หรือ ใช้ Local ทั้งคู่ (LAN)
  3. รอ Phase 2 → API sync
```

---

## ✅ **Checklist - GitHub + Vercel Setup**

- [ ] GitHub account สร้างเสร็จ
- [ ] Email verify เสร็จ
- [ ] Repository สร้างเสร็จ
- [ ] ไฟล์ upload เสร็จ
- [ ] Vercel account สร้างเสร็จ
- [ ] Project import เสร็จ
- [ ] Deploy สำเร็จ
- [ ] URL ทำงานได้
- [ ] Test Admin/Customer/Badge ทั้งหมด
- [ ] QR Code generate ได้
- [ ] Share link ให้ลูกค้าแล้ว
- [ ] ✓ Live on GitHub + Vercel

---

## 🚀 **ข้ันตอนต่อไป**

### **Phase 2 (1-2 เดือน):**
```
□ Add Google Sheets API
□ Auto SMS Reminder
□ LINE Official Account
□ Mobile App
```

### **Phase 3 (3-6 เดือน):**
```
□ Backend Server
□ Multi-branch Sync
□ Advanced Analytics
□ AI Insights
```

---

## 📞 **ติดขัด?**

### **ปัญหา GitHub:**
- Email verification
- Repository creation
- Upload files

### **ปัญหา Vercel:**
- Deploy failed
- URL not working
- Auto refresh needed

### **ปัญหา QR:**
- URL incorrect
- Browser cache
- Regenerate QR

---

## 💡 **Pro Tips**

```
✅ ทำนี้:
  1. Backup GitHub ทุกสัปดาห์
  2. Commit message ชัดเจน
  3. Test URL ทั้งหมด
  4. Export CSV backup

❌ อย่าทำนี้:
  1. Delete repository โดยไม่ backup
  2. Commit sensitive data (password)
  3. ลืม verify email
  4. ลืม test ก่อน share
```

---

## 🎉 **สำเร็จแล้ว!**

```
✓ GitHub Repository สร้างเสร็จ
✓ Vercel Deploy สำเร็จ
✓ URL Online ทำงาน
✓ QR Code ได้
✓ Link ส่งให้ลูกค้า
✓ ✨ THE VIEW Loyalty Online!
```

---

**ติดตั้ง GitHub ได้ 100%? ลองแล้วบอกผล!** 🌟💚

