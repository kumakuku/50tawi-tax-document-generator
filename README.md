# 🇹🇭 Thailand 50 Tawi Tax Document Generator Pro

[![Live Demo](https://img.shields.io/badge/Demo-Live-success)](https://kumakuku.github.io/50tawi-tax-document-generator/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Professional web-based tool for batch generating Thailand Withholding Tax Certificates (Section 50 Bis / 50 ทวิ) in PDF format from CSV files.

เครื่องมือสร้างหนังสือรับรองการหักภาษี ณ ที่จ่าย (50 ทวิ) แบบอัตโนมัติในรูปแบบ PDF จากไฟล์ CSV

---

## ✨ Features / ฟีเจอร์หลัก

### 🆕 Pro Version Features
- **📄 Real PDF Generation** - Generate actual PDF files using jsPDF library
- **🏢 Company Information Management** - Save and reuse company details with LocalStorage
- **💰 Multiple Income Types** - Support 8 different income categories
- **✍️ Digital Signature** - Add digital signatures using SignaturePad
- **🎨 Professional UI** - Modern gradient design with responsive layout
- **📊 Batch Processing** - Generate multiple PDFs with progress tracking
- **💾 Auto-save** - Automatic company info persistence
- **🔄 Data Preview** - Review data before generating documents

### 📋 Supported Income Types
1. เงินเดือน ค่าจ้าง / Salary & Wages
2. ค่าธรรมเนียม ค่านายหน้า / Fee, Commission
3. ค่าแห่งลิขสิทธิ์ / Royalty
4. ดอกเบี้ย เงินปันผล / Interest, Dividend
5. ค่าเช่าทรัพย์สิน / Rental Income
6. รางวัล ส่วนลด / Prize, Discount
7. รับเหมาก่อสร้าง / Construction Contract
8. รายได้อื่นๆ / Other Income

---

## 🚀 Quick Start / เริ่มต้นใช้งาน

### Option 1: Use Online (Recommended)
Visit the live demo: **[https://kumakuku.github.io/50tawi-tax-document-generator/](https://kumakuku.github.io/50tawi-tax-document-generator/)**

### Option 2: Download and Run Locally
1. Download `index.html` from this repository
2. Open the file in your web browser (Chrome, Firefox, Edge, Safari)
3. No installation or server required!

---

## 📖 How to Use / วิธีใช้งาน

### Step 1: Enter Company Information / กรอกข้อมูลบริษัท
- Company Name (ชื่อบริษัท)
- Tax ID (เลขประจำตัวผู้เสียภาษี) - 13 digits
- Address (ที่อยู่)
- Phone (optional)
- Email (optional)
- Click **Save Company Info** to store for future use

### Step 2: Select Income Type / เลือกประเภทเงินได้
Choose the appropriate income category from the dropdown menu

### Step 3: Add Digital Signature / เพิ่มลายเซ็นดิจิทัล
- Draw your signature on the canvas
- Click **Save** to store the signature
- Use **Clear** to redraw

### Step 4: Upload CSV File / อัปโหลดไฟล์ CSV
- Drag and drop your CSV file, or click to browse
- The file will be validated and previewed automatically

### Step 5: Generate PDFs / สร้างไฟล์ PDF
- **Test First PDF**: Generate a sample PDF for the first employee
- **Generate All PDFs**: Batch generate PDFs for all employees
- PDFs will be downloaded automatically to your Downloads folder

---

## 📊 CSV File Format / รูปแบบไฟล์ CSV

### Required Columns (ข้อมูลที่ต้องมี):

```csv
employee_name,tax_id,personal_id,address,payment_date,income_type,amount_paid,tax_withheld,social_security,provident_fund
Somchai Jaidee,1234567890123,1-2345-67890-12-3,"123 Main St, Bangkok",2024-01-15,Salary,50000,5000,750,2500
Pranee Suksa,9876543210987,3-4567-89012-34-5,"456 Second Rd, Chiang Mai",2024-01-15,Salary,45000,4500,750,2250
```

### Column Descriptions:
- `employee_name` - Full name in Thai or English
- `tax_id` - 13-digit tax identification number
- `personal_id` - Thai national ID (13 digits with dashes)
- `address` - Full address
- `payment_date` - Payment date (YYYY-MM-DD format)
- `income_type` - Type of income (e.g., "Salary", "Fee", "Commission")
- `amount_paid` - Total income amount (number)
- `tax_withheld` - Tax amount withheld (number)
- `social_security` - Social security contribution (number)
- `provident_fund` - Provident fund contribution (number)

### 📥 Sample File
Download the sample CSV file: [sample_data.csv](./sample_data.csv)

---

## 🛠️ Technical Details / รายละเอียดทางเทคนิค

### Technologies Used
- **HTML5** - Document structure
- **CSS3** - Modern styling with gradients and animations
- **JavaScript (ES6+)** - Core functionality
- **jsPDF** - PDF generation library
- **html2canvas** - HTML to canvas conversion
- **SignaturePad** - Digital signature capture

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

### Features
- 📱 **Responsive Design** - Works on desktop, tablet, and mobile
- 💾 **LocalStorage** - Save company info and signatures
- 🎨 **Modern UI** - Gradient backgrounds, smooth animations
- 🔒 **Privacy First** - All processing done in browser, no data sent to server
- 🚀 **Fast** - Pure client-side, no server delays

---

## 📁 Repository Structure / โครงสร้างไฟล์

```
50tawi-tax-document-generator/
├── index.html              # Pro version (main file)
├── index_basic.html        # Basic version (original)
├── sample_data.csv         # Sample CSV with 5 employees
└── README.md              # This file
```

---

## 🔐 Privacy & Security / ความเป็นส่วนตัวและความปลอดภัย

- ✅ **100% Client-Side** - All data processing happens in your browser
- ✅ **No Server Upload** - CSV files never leave your computer
- ✅ **No Tracking** - No analytics or third-party scripts
- ✅ **LocalStorage Only** - Company info saved locally on your device
- ✅ **Secure** - Can be used offline after first load

---

## 💡 Tips & Best Practices / เคล็ดลับการใช้งาน

1. **Save Company Info**: Use the "Save Company Info" button to avoid re-entering data
2. **Test First**: Use "Test First PDF" to verify your data before generating all PDFs
3. **UTF-8 Encoding**: Ensure your CSV file is saved with UTF-8 encoding for Thai characters
4. **Signature Once**: Save your signature once and reuse it for all documents
5. **Backup CSV**: Keep a backup of your CSV file for record-keeping

---

## 🆚 Version Comparison / เปรียบเทียบเวอร์ชัน

| Feature | Basic Version | Pro Version |
|---------|--------------|-------------|
| HTML Preview | ✅ | ✅ |
| CSV Upload | ✅ | ✅ |
| Batch Processing | ✅ | ✅ |
| **PDF Generation** | ❌ | ✅ |
| **Company Info Save** | ❌ | ✅ |
| **Income Type Selection** | ❌ | ✅ |
| **Digital Signature** | ❌ | ✅ |
| **Progress Bar** | ❌ | ✅ |
| **Modern UI** | ❌ | ✅ |

---

## 🤝 Contributing / การมีส่วนร่วม

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

---

## 📄 License / ใบอนุญาต

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments / กิตติกรรมประกาศ

- **jsPDF** - PDF generation
- **html2canvas** - HTML to canvas conversion
- **SignaturePad** - Digital signature capture
- Thailand Revenue Department - Tax form specifications

---

## 📞 Support / ติดต่อสอบถาม

For questions or support, please open an issue in this repository.

---

## 🔗 Links / ลิงก์ที่เกี่ยวข้อง

- 🌐 [Live Demo](https://kumakuku.github.io/50tawi-tax-document-generator/)
- 📚 [GitHub Repository](https://github.com/kumakuku/50tawi-tax-document-generator)
- 📖 [Thailand Revenue Department](https://www.rd.go.th/)

---

**Made with ❤️ for Thailand's tax professionals**

*Last updated: January 2026*
