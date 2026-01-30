# 🇹🇭 50 Tawi Tax Document Generator
## 泰國報稅文件批次產生器

[![Live Demo](https://img.shields.io/badge/Demo-Live-success)](https://kumakuku.github.io/50tawi-tax-document-generator/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Web-based tool for batch generating Thailand Withholding Tax Certificates (Section 50 Bis / 50 ทวิ) from CSV files.

基於網頁的泰國扣繳稅款證明（50 ทวิ）批次產生工具，可從 CSV 檔案快速產生多份報稅文件。

---

## ✨ Features | 功能特點

✅ **Drag & Drop Upload** - 支援拖曳上傳 CSV 檔案  
✅ **Batch Generation** - 一鍵批次產生多份文件  
✅ **Data Preview** - 即時資料預覽（顯示前 10 筆）  
✅ **Complete Format** - 符合泰國稅務局格式要求  
✅ **User-Friendly Interface** - 現代化直覺介面設計  
✅ **No Server Required** - 純前端運作，資料不上傳  

---

## 🚀 Quick Start | 快速開始

### Online Demo | 線上使用

**直接訪問：** https://kumakuku.github.io/50tawi-tax-document-generator/

### Local Usage | 本地使用

1. Clone this repository | 複製此專案
```bash
git clone https://github.com/kumakuku/50tawi-tax-document-generator.git
cd 50tawi-tax-document-generator
```

2. Open `index.html` in your browser | 在瀏覽器中開啟 `index.html`
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

3. Upload your CSV file or use the sample data | 上傳您的 CSV 檔案或使用範例資料

---

## 📋 CSV File Format | CSV 檔案格式

Your CSV file must include the following columns (必須包含以下欄位):

| Column Name | Description | 說明 | Example |
|------------|-------------|------|---------|
| `employee_name` | Employee name | 員工姓名 | Somchai Kittikul |
| `tax_id` | Tax identification number | 稅務識別號碼 | 1234567890123 |
| `personal_id` | Personal ID number | 個人身分證號 | 1-2345-67890-12-3 |
| `address` | Address | 地址 | 123 Sukhumvit Rd Bangkok |
| `payment_date` | Payment date | 支付日期 | 2026-01-31 |
| `income_type` | Type of income | 收入類型 | 1. Salary |
| `amount_paid` | Amount paid (THB) | 支付金額 | 50000.00 |
| `tax_withheld` | Tax withheld (THB) | 扣繳稅額 | 3500.00 |
| `social_security` | Social security (THB) | 社會保險 | 750.00 |
| `provident_fund` | Provident fund (THB) | 公積金 | 2500.00 |

### Sample CSV | 範例檔案

See [`sample_data.csv`](sample_data.csv) for a complete example with 5 employees.

查看 [`sample_data.csv`](sample_data.csv) 檔案，內含 5 位員工的完整範例。

---

## 📖 How to Use | 使用說明

### Step 1: Prepare Your Data | 準備資料
- Export payroll data from your system as CSV  
  從薪資系統匯出 CSV 格式的資料
- Ensure all required columns are present  
  確保包含所有必要欄位
- Use UTF-8 encoding for Thai characters  
  使用 UTF-8 編碼以支援泰文字元

### Step 2: Upload CSV File | 上傳檔案
- Drag and drop your CSV file to the upload area  
  拖曳 CSV 檔案到上傳區域
- Or click "選擇檔案" button to browse  
  或點擊「選擇檔案」按鈕瀏覽

### Step 3: Review Preview | 檢查預覽
- Check the data preview table (shows first 10 records)  
  檢查資料預覽表格（顯示前 10 筆）
- Verify all fields are correctly mapped  
  確認所有欄位正確對應

### Step 4: Generate Documents | 產生文件
- Click "🚀 批次產生 50 Tawi 文件" button  
  點擊「🚀 批次產生 50 Tawi 文件」按鈕
- Wait for processing (usually takes a few seconds)  
  等待處理（通常數秒完成）
- Documents will be automatically downloaded  
  文件將自動下載

---

## 🎯 Income Types | 收入類型

Common income types for 50 Tawi certificates:

| Code | Description (TH) | Description (EN) |
|------|------------------|------------------|
| 1 | เงินเดือน ค่าจ้าง | Salary, wage, pension |
| 2 | ค่าธรรมเนียม ค่านายหน้า | Commission, fee, bonus |
| 3 | ค่าแห่งลิขสิทธิ์ | Royalty |
| 4 | ดอกเบี้ย | Interest |
| 5 | เงินปันผล | Dividend |

---

## 🛠️ Technical Details | 技術細節

### Technologies Used | 使用技術
- **Pure HTML/CSS/JavaScript** - No frameworks required  
  純 HTML/CSS/JavaScript，無需框架
- **Client-side Processing** - All data stays in your browser  
  客戶端處理，資料不上傳伺服器
- **Responsive Design** - Works on desktop and mobile  
  響應式設計，支援桌面與行動裝置

### Browser Compatibility | 瀏覽器相容性
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

---

## 📝 Output Format | 輸出格式

Generated documents include:
- Certificate number (sequential)
- Payer and payee information
- Income details and breakdown
- Tax withheld amount
- Deductions (social security, provident fund)
- Certification section for signature and seal

Currently outputs as formatted text file (.txt). For PDF generation, see [Future Enhancements](#-future-enhancements--).

---

## 🔒 Privacy & Security | 隱私與安全

- ✅ **100% Client-Side** - No data uploaded to servers  
  完全於瀏覽器端處理，無資料上傳
- ✅ **No Tracking** - No analytics or cookies  
  無追蹤、無分析、無 Cookie
- ✅ **Open Source** - Code is fully transparent  
  開源專案，程式碼完全透明

---

## 🚧 Future Enhancements | 未來改進

- [ ] PDF generation with official format
- [ ] Digital signature support
- [ ] Company information customization
- [ ] Multiple income type templates
- [ ] Bulk email sending
- [ ] Thai language interface option

---

## 🤝 Contributing | 貢獻

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

歡迎貢獻！您可以：
- 回報錯誤
- 建議新功能
- 提交 Pull Request

---

## 📄 License | 授權

MIT License - feel free to use this tool for your business needs.

MIT 授權 - 歡迎用於您的商業需求。

---

## ⚠️ Disclaimer | 免責聲明

This tool is provided as-is for convenience. Please verify all generated documents comply with current Thai Revenue Department regulations before submission. The authors assume no liability for errors or omissions.

本工具僅供便利使用，提交前請確認所有產生的文件符合泰國稅務局最新規定。作者不對任何錯誤或遺漏負責。

---

## 📞 Support | 支援

For questions or issues:
- Open an [Issue](https://github.com/kumakuku/50tawi-tax-document-generator/issues)
- Contact: maktsai2525@gmail.com

---

<div align="center">

**Made with ❤️ for Thai businesses**

**為泰國企業打造** 🇹🇭

[⬆ Back to Top](#-50-tawi-tax-document-generator)

</div>
