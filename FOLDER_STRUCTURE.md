# 📁 THE VIEW GROUP - Folder Structure Guide

## 🏗️ **โครงสร้างโปรเจกต์ (Professional)**

```
THE_VIEW_Loyalty/
│
├── 📄 Frontend (HTML Files - ตัวโปรแกรม)
│   ├── index.html                      (Dashboard หลัก)
│   ├── loyalty_with_registration.html  (Admin Panel)
│   ├── customer-portal.html            (Customer Portal)
│   └── qr-badge-generator.html         (Badge Generator)
│
├── 📁 api/ (Backend - Phase 2)
│   ├── middleware/
│   │   ├── auth.js                    (Authentication)
│   │   └── pdpa.js                    (PDPA validation)
│   ├── routes/
│   │   ├── customers.js               (Customer API)
│   │   ├── points.js                  (Points API)
│   │   ├── promo.js                   (Promotion API)
│   │   └── auth.js                    (Login API)
│   ├── models/
│   │   ├── customer.js
│   │   ├── transaction.js
│   │   └── promo.js
│   ├── config/
│   │   └── database.js
│   └── server.js                      (Main server file)
│
├── 📁 lib/ (Utility Functions)
│   ├── calculations.js                (Age, tier, points calc)
│   ├── validators.js                  (Data validation)
│   ├── storage.js                     (localStorage wrapper)
│   └── qrcode.js                      (QR code helper)
│
├── 📁 public/ (Static Assets)
│   ├── images/
│   │   ├── logo.png
│   │   ├── badge-template.png
│   │   └── icons/
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   ├── utils.js
│   │   └── storage.js
│   └── fonts/
│
├── 📁 docs/ (Documentation)
│   ├── README.md
│   ├── INSTALLATION_GUIDE.md
│   ├── GITHUB_INSTALLATION.md
│   ├── QUICK_START_GUIDE.md
│   ├── QUICK_INSTALL.md
│   ├── THE_VIEW_SETUP_GUIDE.md
│   ├── PDPA_COMPLIANCE_GUIDE.md
│   ├── FOLDER_STRUCTURE.md
│   └── API_DOCUMENTATION.md
│
├── 📁 data/ (Local Data - .gitignore)
│   ├── customers.json
│   ├── transactions.json
│   └── backup/
│
├── 📁 tests/ (Testing - Phase 3)
│   ├── unit/
│   ├── integration/
│   └── e2e/
│
├── 📄 Config Files
│   ├── package.json                   (Project metadata + dependencies)
│   ├── vercel.json                    (Vercel deployment config)
│   ├── .gitignore                     (Files to exclude from Git)
│   ├── .env.example                   (Environment variables template)
│   └── .github/
│       └── workflows/
│           └── deploy.yml             (Auto-deploy CI/CD)
│
└── 📄 Root Files
    ├── LICENSE                        (MIT License)
    ├── CHANGELOG.md                   (Version history)
    └── CONTRIBUTING.md                (Contribution guide)
```

---

## 📖 **ประกาศนียบัตร - ทำความเข้าใจแต่ละ Folder**

### **📄 Frontend (ระดับล่าง)**
```
Files: index.html, loyalty_with_registration.html, 
       customer-portal.html, qr-badge-generator.html

ใช้สำหรับ:
✓ UI/UX (สิ่งที่ลูกค้าเห็น)
✓ ปัจจุบันใช้ localStorage
✓ Phase 1 (เสร็จแล้ว)

หน้าที่:
├─ Admin → ลงทะเบียน + บวกคะแนน
├─ Customer → เช็คคะแนน
└─ Badge → พิมพ์บัตร
```

### **📁 api/ (Backend - Phase 2)**
```
Server-side code (Node.js/Express)

Structure:
├─ middleware/ → Authentication, PDPA validation
├─ routes/ → API endpoints
├─ models/ → Database schema
├─ config/ → Database connection
└─ server.js → Main server

ตัวอย่าง Routes:
GET  /api/customers/:id
POST /api/customers
PUT  /api/customers/:id/points
GET  /api/promo/:id
```

### **📁 lib/ (Utility Functions)**
```
Helper functions ที่ใช้ซ้ำ

File:
├─ calculations.js
│  ├─ calculateAge(dob)
│  ├─ getTier(points)
│  ├─ getDaysUntilBirthday(dob)
│  └─ calculateRedemption(points, tier)
│
├─ validators.js
│  ├─ validateEmail()
│  ├─ validatePhone()
│  ├─ validateDOB()
│  └─ validatePDPA()
│
├─ storage.js
│  ├─ saveCustomer()
│  ├─ getCustomer()
│  ├─ deleteCustomer()
│  └─ getAllCustomers()
│
└─ qrcode.js
   ├─ generateQR()
   ├─ parseQR()
   └─ validateQR()
```

### **📁 public/ (Static Assets)**
```
ไฟล์ที่สาธารณะ (images, css, fonts)

Structure:
├─ images/ → Logo, icons, templates
├─ css/ → Stylesheets
├─ js/ → Client-side utilities
└─ fonts/ → Custom fonts

Use:
<img src="/public/images/logo.png">
<link rel="stylesheet" href="/public/css/styles.css">
```

### **📁 docs/ (Documentation)**
```
README, guides, API documentation

Files:
├─ README.md → Overview
├─ INSTALLATION_GUIDE.md → How to install
├─ QUICK_START_GUIDE.md → How to use
├─ PDPA_COMPLIANCE_GUIDE.md → PDPA info
└─ API_DOCUMENTATION.md → API reference (Phase 2)
```

### **📁 data/ (Local Data)**
```
⚠️ .gitignore (ไม่ push ไป GitHub)

Files:
├─ customers.json → Customer data
├─ transactions.json → Transaction history
└─ backup/ → Manual backups

🔒 CONFIDENTIAL (ไม่ public)
```

### **📁 tests/ (Testing - Phase 3)**
```
Unit tests, integration tests, E2E tests

Structure:
├─ unit/ → Individual function tests
├─ integration/ → API tests
└─ e2e/ → Full flow tests

Tools:
Jest, Mocha, Cypress
```

---

## 🎯 **Phase Breakdown**

### **Phase 1: Frontend** ✅ (ตอนนี้)
```
Folder:
├─ Root files (index.html, etc.)
├─ public/images/
└─ docs/

Status: COMPLETE
Vercel: ✓ Live
```

### **Phase 2: Backend + API** 📅 (1-2 เดือน)
```
Folder:
├─ api/
├─ lib/
├─ package.json
├─ vercel.json
└─ .env

Tasks:
□ Create Express server
□ Setup database (MongoDB)
□ Create API routes
□ Add authentication
□ Deploy to Vercel Functions
```

### **Phase 3: Advanced** 📅 (3-6 เดือน)
```
Folder:
├─ tests/
├─ .github/workflows/
└─ Multi-database support

Tasks:
□ Unit tests
□ Integration tests
□ CI/CD pipeline
□ Multi-branch support
```

---

## 📋 **สร้าง Folder Structure - Step by Step**

### **ใน GitHub Web Interface:**

#### **1. สร้าง Folders**

```
1. เข้า Code tab
2. Click "Add file" → "Create new file"
3. ป้อน: public/images/.gitkeep
4. Commit
   → GitHub auto-create folder "public" + "images"

Repeat สำหรับ:
├─ api/middleware/.gitkeep
├─ api/routes/.gitkeep
├─ api/models/.gitkeep
├─ api/config/.gitkeep
├─ lib/.gitkeep
├─ docs/.gitkeep
├─ data/.gitkeep
└─ tests/.gitkeep
```

#### **2. Upload Config Files**

```
1. Click "Add file" → "Upload files"
2. Upload:
   ├─ package.json
   ├─ vercel.json
   ├─ .gitignore
   ├─ FOLDER_STRUCTURE.md
   └─ .env.example

3. Commit all
```

#### **3. Upload Documentation**

```
Move ทั้งหมด ไปยัง /docs/:
├─ README.md
├─ INSTALLATION_GUIDE.md
├─ QUICK_START_GUIDE.md
├─ THE_VIEW_SETUP_GUIDE.md
├─ GITHUB_INSTALLATION.md
├─ PDPA_COMPLIANCE_GUIDE.md
└─ FOLDER_STRUCTURE.md
```

---

## 🔧 **Phase 2 Preparation - Template Code**

### **api/server.js** (Phase 2 - Template)
```javascript
// Phase 2: Backend Server
const express = require('express');
const cors = require('cors');
const app = express();

// Middleware
app.use(cors());
app.use(express.json());

// Routes
app.get('/api/customers/:id', (req, res) => {
  // Get customer by ID
  res.json({ id: req.params.id });
});

app.post('/api/customers', (req, res) => {
  // Create new customer
  res.json({ success: true });
});

app.put('/api/customers/:id/points', (req, res) => {
  // Update points
  res.json({ success: true });
});

// Error handling
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).json({ error: 'Internal Server Error' });
});

// Start server
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log(`Server running on port ${PORT}`));

module.exports = app;
```

### **lib/calculations.js** (Utility)
```javascript
// Calculation functions

function calculateAge(dob) {
  const today = new Date();
  const birthDate = new Date(dob);
  let age = today.getFullYear() - birthDate.getFullYear();
  const m = today.getMonth() - birthDate.getMonth();
  if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
    age--;
  }
  return age;
}

function getTier(points) {
  if (points >= 150000) return { name: 'Platinum', discount: '12-15%' };
  if (points >= 50000) return { name: 'Gold', discount: '7-10%' };
  return { name: 'Silver', discount: '3-5%' };
}

function getDaysUntilBirthday(dob) {
  const today = new Date();
  const birthDate = new Date(dob);
  const thisYearBirthday = new Date(today.getFullYear(), birthDate.getMonth(), birthDate.getDate());
  
  if (thisYearBirthday < today) {
    thisYearBirthday.setFullYear(today.getFullYear() + 1);
  }
  
  const daysLeft = Math.ceil((thisYearBirthday - today) / (1000 * 60 * 60 * 24));
  return daysLeft;
}

module.exports = {
  calculateAge,
  getTier,
  getDaysUntilBirthday
};
```

---

## 📊 **File Size Estimate**

```
Phase 1 (Frontend):
├─ HTML files: ~500 KB (all 4 files)
├─ Docs: ~200 KB
├─ Config: ~10 KB
└─ Total: ~710 KB ✓

Phase 2 (Backend - template):
├─ Server code: ~50 KB
├─ API routes: ~100 KB
└─ Estimated: ~150 KB

GitHub limit: 100 MB ✓ (Plenty of space)
Vercel limit: 100 MB ✓ (No problem)
```

---

## 🚀 **Next Steps**

### **ทันที (Now):**
```
1. Upload config files (package.json, vercel.json, .gitignore)
2. Create folder structure (.gitkeep files)
3. Move docs ไปยัง /docs/
4. Deploy ไป Vercel
```

### **1-2 เดือน (Phase 2):**
```
1. Create /api/ folder structure
2. Setup Node.js/Express
3. Create API routes
4. Setup database
5. Deploy backend
```

### **3-6 เดือน (Phase 3):**
```
1. Create /tests/ folder
2. Add CI/CD pipeline
3. Multi-branch support
4. Advanced features
```

---

## ✅ **Checklist - Folder Setup**

- [ ] Create /api/ folder structure
- [ ] Create /lib/ folder structure
- [ ] Create /public/ folder structure
- [ ] Create /docs/ folder
- [ ] Create /data/ folder
- [ ] Create /tests/ folder
- [ ] Upload package.json
- [ ] Upload vercel.json
- [ ] Upload .gitignore
- [ ] Upload FOLDER_STRUCTURE.md
- [ ] Move all docs to /docs/
- [ ] Deploy to Vercel
- [ ] ✓ Verify URL works

---

**Ready สำหรับ Phase 2 & Beyond!** 🚀💚

