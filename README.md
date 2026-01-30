# 🇹🇭 Thailand 50 Tawi Tax Document Generator Pro

A professional web-based tool for batch generating Thailand tax withholding certificates (50 Tawi forms) in PDF format from CSV data files.

เครื่องมือสร้างหนังสือรับรองการหักภาษี ณ ที่จ่าย (50 Tawi) แบบอัตโนมัติในรูปแบบ PDF จากไฟล์ CSV

---

## ✨ Features / ฟีเจอร์หลัก

### 📋 Core Functions
- **✅ Batch PDF Generation** - Generate multiple tax documents at once
- **🏢 Company Information Customization** - Save and reuse company details
- **📊 CSV Data Import** - Drag & drop or click to upload employee data
- **✍️ Digital Signature** - Built-in signature pad for authorized persons
- **🎨 Professional PDF Output** - Clean, bilingual (Thai/English) format
- **💾 Local Storage** - Save company info for future use

### 🎯 Advanced Features
- **6 Income Types Supported**:
  1. Salary (เงินเดือน)
  2. Bonus (โบนัส)
  3. Overtime (ค่าล่วงเวลา)
  4. Commission (ค่าคอมมิชชั่น)
  5. Allowance (เบี้ยเลี้ยง)
  6. Other Income (รายได้อื่นๆ)

- **Automatic Calculations**:
  - Total income
  - Total deductions (Social Security + Provident Fund)
  - Net income
  - Tax withheld

- **Data Preview** - Review uploaded data before generation
- **Progress Tracking** - Real-time progress bar and generation log
- **Responsive Design** - Works on desktop, tablet, and mobile

---

## 🚀 Quick Start / เริ่มใช้งาน

### 1. Download and Open
1. Download `50tawi_generator_pro.html`
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. No installation or server required!

### 2. Setup Company Information
Go to **📋 Company Info** tab and fill in:
- Company Name *
- Company Tax ID *
- Company Address *
- Phone (optional)
- Email (optional)
- Authorized Person *
- Position (optional)
- Tax Year *

Click **💾 Save Company Info**

### 3. Select Income Type
Choose the default income type for your batch (can be overridden in CSV)

### 4. Upload CSV Data
Go to **📤 Upload Data** tab:
- Drag & drop your CSV file or click to browse
- Review the data preview (first 10 records shown)
- Verify total record count

### 5. Add Digital Signature (Optional)
Go to **✍️ Digital Signature** tab:
- Sign in the signature pad using mouse or touch
- Click **💾 Save Signature**
- Preview will appear below

### 6. Generate PDFs
Go to **🎯 Generate Documents** tab:
- Check the readiness checklist
- Click **📄 Batch Generate PDF Documents**
- Wait for progress bar to complete
- PDFs will auto-download one by one

---

## 📄 CSV File Format / รูปแบบไฟล์ CSV

### Required Columns / คอลัมน์ที่ต้องมี

Your CSV file must include these columns:

```csv
employee_name,tax_id,personal_id,address,payment_date,income_type,amount_paid,tax_withheld,social_security,provident_fund
```

### Column Descriptions

| Column Name | Description | Example |
|------------|-------------|---------|
| `employee_name` | Employee full name | Somchai Kittikul |
| `tax_id` | Tax identification number (13 digits) | 1234567890123 |
| `personal_id` | Personal ID number | 1-2345-67890-12-3 |
| `address` | Employee address | 123 Sukhumvit Road Bangkok 10110 |
| `payment_date` | Payment date | 2026-01-31 |
| `income_type` | Income type description | 1. Salary |
| `amount_paid` | Gross amount paid (THB) | 50000.00 |
| `tax_withheld` | Tax withheld amount (THB) | 3500.00 |
| `social_security` | Social security deduction (THB) | 750.00 |
| `provident_fund` | Provident fund deduction (THB) | 2500.00 |

### Sample CSV

Download `50tawi_sample.csv` for a working example with 3 employees.

---

## 🖼️ Screenshots / ภาพหน้าจอ

### Company Information Setup
![Company Info](https://via.placeholder.com/800x400?text=Company+Information+Tab)

### CSV Upload & Preview
![Upload](https://via.placeholder.com/800x400?text=CSV+Upload+and+Preview)

### Digital Signature
![Signature](https://via.placeholder.com/800x400?text=Digital+Signature+Pad)

### PDF Generation
![Generate](https://via.placeholder.com/800x400?text=PDF+Generation+Progress)

---

## 🛠️ Technical Details / รายละเอียดทางเทคนิค

### Technologies Used
- **HTML5** - Structure and markup
- **CSS3** - Styling with gradients and animations
- **Vanilla JavaScript** - Core logic (no framework dependencies)
- **jsPDF** - PDF generation library
- **html2canvas** - HTML to canvas conversion (for future enhancements)
- **Signature Pad** - Digital signature capture

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

### Security & Privacy
- ✅ **100% Client-Side** - All data processing happens in your browser
- ✅ **No Server Upload** - Your data never leaves your computer
- ✅ **No External APIs** - Works completely offline (after first load)
- ✅ **Local Storage Only** - Company info saved in browser storage

### File Size Limits
- Maximum CSV file size: **10 MB**
- Recommended: Less than 5,000 records per batch for optimal performance

---

## 📖 Usage Guide / คู่มือการใช้งาน

### Best Practices

1. **Prepare Your Data**
   - Ensure all employee data is accurate
   - Use consistent date format (YYYY-MM-DD)
   - Verify tax calculations before generating

2. **Company Information**
   - Save company info once, reuse for future batches
   - Update tax year annually

3. **Signature**
   - Use a clear, legible signature
   - Re-sign if signature is unclear
   - Signature is optional but recommended

4. **Batch Size**
   - For large batches (1000+ records), consider splitting into smaller batches
   - Close other browser tabs to improve performance

### Troubleshooting

**Problem: CSV upload fails**
- Check file format is `.csv` (not `.xlsx` or `.xls`)
- Verify column names match exactly
- Ensure file size is under 10 MB

**Problem: PDFs not downloading**
- Check browser popup blocker settings
- Allow multiple downloads from the page
- Try reducing batch size

**Problem: Signature not saving**
- Ensure you draw something on the signature pad
- Click "Save Signature" button after drawing
- Try using a mouse instead of trackpad

**Problem: Data preview shows incorrect values**
- Check CSV encoding (should be UTF-8)
- Verify no extra commas in address fields
- Use quotes around fields containing commas

---

## 📝 Sample Data / ข้อมูลตัวอย่าง

The repository includes `50tawi_sample.csv` with 3 sample employees:

1. **Somchai Kittikul** - Salary 50,000 THB
2. **Napat Wongsakul** - Salary 65,000 THB
3. **Pimchanok Srisawat** - Salary 45,000 THB

Use this file to test the tool before using your actual employee data.

---

## 🔄 Version History / ประวัติเวอร์ชัน

### Version 1.0 Pro (Current)
- ✅ Full PDF generation with jsPDF
- ✅ Company information customization
- ✅ 6 income types support
- ✅ Digital signature pad
- ✅ Progress tracking
- ✅ Bilingual (Thai/English) output
- ✅ Responsive design

### Planned Features (Future)
- [ ] Email PDF directly to employees
- [ ] Export summary report (Excel)
- [ ] Multi-company support
- [ ] Template customization
- [ ] Batch email sending
- [ ] Integration with payroll systems

---

## 🤝 Contributing / การมีส่วนร่วม

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

---

## 📄 License / ลิขสิทธิ์

This project is open source and available under the MIT License.

---

## ⚠️ Disclaimer / ข้อจำกัดความรับผิดชอบ

This tool is provided as-is for convenience. Users are responsible for:
- Verifying accuracy of all tax calculations
- Ensuring compliance with Thai tax regulations
- Consulting with tax professionals when needed
- Maintaining data security and privacy

The developers assume no liability for any errors or omissions in the generated documents.

เครื่องมือนี้จัดทำขึ้นเพื่อความสะดวก ผู้ใช้มีหน้าที่รับผิดชอบในการตรวจสอบความถูกต้องของข้อมูลและการคำนวณภาษีทั้งหมด

---

## 📧 Support / การสนับสนุน

For questions, issues, or suggestions:
- Open an issue on GitHub
- Check existing issues for solutions
- Review this README thoroughly

---

## 🌟 Star this Project

If you find this tool helpful, please give it a ⭐ on GitHub!

---

**Made with ❤️ for Thai businesses and HR professionals**

**สร้างด้วยใจเพื่อธุรกิจไทยและผู้เชี่ยวชาญด้าน HR**
