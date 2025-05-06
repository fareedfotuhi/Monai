# Monai
<p align="center">
  <img src="monai_toolkit_logo.webp" width="600"/>
</p>

## مقدمه 
پیشرفت‌های اخیر در یادگیری عمیق، تحول بزرگی در حوزه تصویربرداری پزشکی ایجاد کرده‌اند؛ از تشخیص خودکار بیماری‌ها تا تحلیل پیچیده داده‌های MRI و CT. با این حال، کار با داده‌های پزشکی به دلیل فرمت‌های خاص، نیازمندی‌های پردازشی بالا، و پیچیدگی مدل‌های مورد نیاز، چالش‌برانگیز است. فریم‌ورک MONAI، که بر پایه PyTorch ساخته شده، با هدف ساده‌سازی توسعه مدل‌های هوش مصنوعی در حوزه پزشکی طراحی شده است. این کتابخانه امکانات پیشرفته‌ای برای پردازش داده‌های تصویربرداری پزشکی، ساخت مدل‌های پیچیده (مانند UNet، DynUNet و SegResNet)، و آموزش در سطح صنعتی فراهم می‌کند.

## 📌 کاربردهای MONAI

فریم‌ورک MONAI (Medical Open Network for AI) با تمرکز بر تصویربرداری پزشکی، ابزارها و ماژول‌هایی فراهم می‌کند که توسعه مدل‌های یادگیری عمیق را در حوزه سلامت تسهیل می‌سازد. در این بخش، با مهم‌ترین کاربردهای MONAI در پروژه‌های واقعی آشنا می‌شوید، همراه با تصاویر و مثال‌های عملی از مخازن GitHub.

---

### 🧠 1. سگمنتیشن تصاویر پزشکی (Medical Image Segmentation)

📌 **توضیح:**  
سگمنتیشن فرآیندی است که در آن نواحی مشخصی از تصویر (مانند تومورها، اندام‌ها یا بافت‌ها) تفکیک و شناسایی می‌شوند. این فرآیند یکی از مهم‌ترین و رایج‌ترین کاربردهای یادگیری عمیق در پزشکی است. با استفاده از معماری‌هایی مانند `UNet`, `Swin UNETR`, و `DynUNet`، MONAI می‌تواند مدل‌هایی قدرتمند برای استخراج دقیق ساختارهای پزشکی از داده‌های حجیم مانند MRI یا CT ایجاد کند.

📚 **مثال‌ها:**
- 🧪 BraTS Challenge: سگمنت‌کردن تومور مغزی با Swin UNETR  
  🔗 [کد منبع در GitHub](https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/swin_unetr_brats21_segmentation_3d.ipynb)
- 👨‍⚕️ پروژه شخصی برای سگمنت‌کردن کبد یا ریه با UNet  
  🔗 [نمونه ریپوزیتوری](https://github.com/jinunyachhyon/Medical-Image-Segmentation-using-MONAI)

🖼️ **نمونه تصویر:**
<p align="center">
  <img src="https://docs.wandb.ai/images/tutorials/monai/viz-2.gif" alt="Brain Tumor Segmentation" width="600"/>
</p>

---

### 🔍 2. طبقه‌بندی پزشکی (Medical Image Classification)

📌 **توضیح:**  
طبقه‌بندی تصاویر پزشکی به فرآیند تشخیص وجود یا عدم وجود بیماری‌ها در تصاویر (مانند CT یا X-ray) اشاره دارد. از کاربردهای رایج آن می‌توان به تشخیص COVID-19، سرطان پستان یا بیماری‌های ریوی اشاره کرد. MONAI از مدل‌هایی مانند `DenseNet`, `ResNet`, و `EfficientNet` برای طبقه‌بندی تصاویر پشتیبانی می‌کند. ابزارهای ساده‌ی آموزش و ارزیابی باعث می‌شود مدل‌های تشخیص بیماری در زمان کوتاه توسعه یابند.

📚 **مثال‌ها:**
- 🤒 تشخیص COVID-19 از CT قفسه سینه  
  🔗 [نمونه پروژه](https://github.com/AkashArora2303/MONAI-COVID-CT-Classification)
- 🖼 آموزش مدل طبقه‌بندی با داده MedNIST  
  🔗 [آموزش در GitHub](https://github.com/Project-MONAI/tutorials/blob/master/2d_classification/mednist_tutorial.ipynb)

🖼️ **نمونه تصویر:**
<p align="center">
  <img src="download.png" alt="COVID CT Classification" width="600"/>
</p>

---

### 📏 3. ثبت تصاویر پزشکی (Image Registration)

📌 **توضیح:**  
ثبت تصاویر به معنای هم‌ترازی تصاویر پزشکی از زمان‌ها یا منابع مختلف است. این تکنیک برای مقایسه تصاویر قبل و بعد از درمان، ترکیب چند نوع modality (مثل CT و MRI)، یا حذف اثر حرکت بیمار کاربرد دارد. MONAI ابزارهایی برای ثبت تصاویر جفتی (supervised) و ثبت بدون نظارت (unsupervised) ارائه کرده که با استفاده از شبکه‌های کانولوشنی یا ترنسفورمر انجام می‌شود.

📚 **مثال‌ها:**
- 📦 ثبت تصاویر ریه در چند نوبت CT  
  🔗 [آموزش ثبت جفتی در GitHub](https://github.com/Project-MONAI/tutorials/blob/main/3d_registration/paired_lung_ct.ipynb)
- 🧠 ثبت بدون نظارت مغز با مجموعه داده OASIS  
  🔗 [کد آموزشی در GitHub](https://github.com/Project-MONAI/tutorials/blob/main/3d_registration/learn2reg_oasis_unpaired_brain_mr.ipynb)

🖼️ **نمونه تصویر:**
<p align="center">
  <img src="https://docs.monai.io/en/0.5.3/_images/3d_paired.png" alt="Image Registration" width="500"/>
</p>

---

### 🩻 4. بازسازی سه‌بعدی (3D Reconstruction)

📌 **توضیح:**  
در این کاربرد، هدف ایجاد نمای سه‌بعدی از اندام‌ها یا ساختارهای داخلی بدن بر اساس برش‌های دو‌بعدی (مانند CT/MRI slice) است. بازسازی سه‌بعدی در جراحی‌های پیچیده، مدلسازی دیجیتالی بیمار و شبیه‌سازی‌های درمانی اهمیت بالایی دارد. MONAI قابلیت‌هایی برای استفاده از VAE (Variational Autoencoder) و GAN برای این کاربرد فراهم کرده است.

📚 **مثال‌ها:**
- 📈 بازسازی تصاویر MedNIST با استفاده از VAE  
  🔗 [آموزش در GitHub](https://github.com/Project-MONAI/tutorials/blob/main/modules/varautoencoder_mednist.ipynb)

🖼️ **نمونه تصویر:**
<p align="center">
  <img src="1-s2.0-S2352711023001280-gr4_lrg.jpg" alt="3D CT Reconstruction" width="500"/>
</p>

---

### ⚙️ 5. ساختار Pipeline کامل یادگیری ماشین پزشکی

📌 **توضیح:**  
یکی از ویژگی‌های برجسته MONAI، پشتیبانی از ساخت pipelineهای کامل از ابتدا تا انتهای پروژه است. این قابلیت شامل مراحل مختلفی است:
- بارگذاری و پردازش داده‌های پزشکی (DICOM, NIfTI)
- افزایش داده (data augmentation) اختصاصی پزشکی
- آموزش مدل با چند GPU و پشتیبانی از Mixed Precision
- ارزیابی با متریک‌های پزشکی (Dice, Hausdorff Distance)
- استقرار مدل با MONAI Deploy در سیستم‌های کلینیکی یا لبه‌ای (edge devices)

📚 **مثال‌ها:**
- 🏥 ساخت اپلیکیشن قابل استقرار با MONAI Deploy SDK  
  🔗 [مشاهده در GitHub](https://github.com/Project-MONAI/monai-deploy-app-sdk)
- ⚡ پردازش بلادرنگ با MONAIStream  
  🔗 [لینک به ریپوزیتوری](https://github.com/Project-MONAI/MONAIStream)

🖼️ **ساختار pipeline:**
<p align="center">
  <img src="https://docs.monai.io/en/0.9.1/_images/end_to_end.png" alt="Pipeline Structure" width="600"/>
</p>

---
