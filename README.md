# Monai
<p align="center">
  <img src="monai_toolkit_logo.webp" width="600"/>
</p>

## مقدمه 
پیشرفت‌های اخیر در یادگیری عمیق، تحول بزرگی در حوزه تصویربرداری پزشکی ایجاد کرده‌اند؛ از تشخیص خودکار بیماری‌ها تا تحلیل پیچیده داده‌های MRI و CT. با این حال، کار با داده‌های پزشکی به دلیل فرمت‌های خاص، نیازمندی‌های پردازشی بالا، و پیچیدگی مدل‌های مورد نیاز، چالش‌برانگیز است. فریم‌ورک MONAI، که بر پایه PyTorch ساخته شده، با هدف ساده‌سازی توسعه مدل‌های هوش مصنوعی در حوزه پزشکی طراحی شده است. این کتابخانه امکانات پیشرفته‌ای برای پردازش داده‌های تصویربرداری پزشکی، ساخت مدل‌های پیچیده (مانند UNet، DynUNet و SegResNet)، و آموزش در سطح صنعتی فراهم می‌کند.

## 📌 کاربردهای MONAI

فریم‌ورک MONAI ابزارهای تخصصی برای توسعه مدل‌های یادگیری عمیق در تصویربرداری پزشکی فراهم می‌کند. در ادامه، مهم‌ترین کاربردهای آن را با مثال و تصویر بررسی می‌کنیم:

---

### 🧠 1. سگمنتیشن تصاویر پزشکی (Medical Image Segmentation)

📌 مثال‌ها:
- استخراج تومور مغز از MRI (BraTS)
- سگمنت‌کردن ریه در CT اسکن

🖼️ نمونه سگمنتیشن:
<p align="center">
  <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/unet_brats_example.png" alt="Brain Tumor Segmentation" width="600"/>
</p>

---

### 🔍 2. طبقه‌بندی پزشکی (Medical Image Classification)

📌 مثال‌ها:
- تشخیص COVID-19 در CT قفسه سینه
- طبقه‌بندی سرطان از ماموگرافی

🖼️ نمونه طبقه‌بندی:
<p align="center">
  <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/classification_example.png" alt="COVID CT Classification" width="600"/>
</p>

---

### 📏 3. ثبت تصاویر پزشکی (Image Registration)

📌 مثال‌ها:
- ثبت CT و MRI یک بیمار
- انطباق زمان‌دار اسکن‌ها

🖼️ نمونه ثبت تصویر:
<p align="center">
  <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/registration_example.gif" alt="Image Registration" width="500"/>
</p>

---

### 🩻 4. بازسازی سه‌بعدی (3D Reconstruction)

📌 مثال‌ها:
- بازسازی ساختار مغز از تصاویر slice
- مدل‌سازی اندام‌ها

🖼️ بازسازی 3D:
<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/41/Lung_CT_Scan_3D_Reconstruction.gif" alt="3D CT Reconstruction" width="500"/>
</p>

---

### ⚙️ 5. Pipelineهای کامل یادگیری ماشین پزشکی

📌 امکانات:
- Transforms پیشرفته
- آموزش توزیع‌شده
- ابزار ارزیابی پزشکی

🖼️ ساختار pipeline:
<p align="center">
  <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/pipeline_example.png" alt="Pipeline Structure" width="600"/>
</p>
