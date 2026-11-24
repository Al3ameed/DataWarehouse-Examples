<div align="center">
# 🏠 Data Has a Home
### الداتا ليها بيت
 
**An interactive, animated explainer for Data Warehouse concepts: Drill Down, Data Mart, and Data Mining**
<br>
**شرح تفاعلي متحرّك لمفاهيم الـ Data Warehouse: الـ Drill Down والـ Data Mart والـ Data Mining**
 
![HTML](https://img.shields.io/badge/HTML-single%20file-9B7BFF?style=flat-square)
![D3.js](https://img.shields.io/badge/D3.js-v7-F062C0?style=flat-square)
![No build](https://img.shields.io/badge/build-none-3FE0D0?style=flat-square)
![RTL](https://img.shields.io/badge/UI-Arabic%20RTL-7D96FF?style=flat-square)
 
[English](#-english) · [العربية](#-العربية)
 
<img src="assets/preview.gif" width="300" alt="Drill down from the globe to a branch">
</div>
---
 
## 🇬🇧 English
 
Students often memorize the definitions of Drill Down, Data Mart, and Data Mining without really feeling the difference. This project turns each concept into something you can **see and click**: you zoom from the planet down to a single branch, watch tables fly into a department's Data Mart, and let an algorithm discover patterns on its own.
 
### ✨ Features
 
**🌍 Google-Earth-style Drill Down**
- Fly from a spinning globe → Egypt → region → governorate → branch, drawn on real governorate borders.
- The camera tilts as you go deeper, with a live altitude readout and upright map pins.
- A side panel shows totals at each level and checks that **the children always add up to the parent**.
- A live SQL query rewrites itself on every step, so you can see the `WHERE` and `GROUP BY` changes. Roll Up takes you back.
**📦 Data Mart builder**
- Pick a department (Sales, HR, Finance, Marketing) and watch only its tables fly out of the warehouse.
- Shows shared (conformed) dimensions, and the difference between dependent and independent data marts.
**⛏️ Data Mining lab**
- **Association rules** on 16 supermarket receipts, with support, confidence, lift, and an adjustable minimum confidence.
- **K-Means clustering** animated step by step, grouping 45 customers with no labels.
**🃏 Compare & quiz**
- Flip cards, side-by-side comparison tables, and a 6-question quiz.
**🧳 Data journey**
- An animated pipeline: sources → ETL → Data Warehouse → Data Marts → Drill Down / Mining / Reports.
**Plus:** a space theme with dark and light modes, a responsive layout, an Arabic RTL interface, and support for reduced-motion settings.
 
### 🧠 The four concepts in one line each
 
| Concept | What it is | Storage or usage? |
|---|---|---|
| 🏢 **Data Warehouse** | One central store for all company data, organized for analysis | Storage |
| 📦 **Data Mart** | A smaller slice of the warehouse for one department | Storage |
| 🌍 **Drill Down** | An OLAP operation that moves from a summary to its details | Usage: *you* ask |
| ⛏️ **Data Mining** | Algorithms that find hidden patterns and make predictions | Usage: *the data* answers |
 
### 📸 Screenshots
 
| | |
|---|---|
| ![Hero](assets/hero.png) | ![Drill Down](assets/drilldown.png) |
| ![Data Mart](assets/datamart.png) | ![Data Mining](assets/datamining.png) |
 
![Compare](assets/compare.png)
 
### 🚀 Run it
 
No installation and no build step.
 
1. Download or clone the repo.
2. Open `index.html` in any modern browser.
> An internet connection is needed the first time to load D3.js and the fonts. The map data is already embedded in the file.
 
**Publish it with GitHub Pages:** go to **Settings → Pages → Deploy from a branch**, choose `main` and `/ (root)`, then save. Your site will be live at `https://<username>.github.io/<repo-name>/`.
 
### 🛠 Tech stack
 
- **Plain HTML, CSS, and JavaScript** in a single file
- **[D3.js v7](https://d3js.org/)** for the orthographic globe projection and the smooth zoom flights
- **Map data:** [Natural Earth](https://www.naturalearthdata.com/) (governorates, Nile, lakes) and [world-atlas](https://github.com/topojson/world-atlas), simplified with [mapshaper](https://mapshaper.org/) and embedded inline
- **Fonts:** Alexandria & Rubik via Google Fonts
### 📁 Structure
 
```
.
├── index.html       # the whole site
├── README.md
└── assets/          # screenshots and preview GIF
```
 
### ⚠️ About the data
 
All sales figures, receipts, and customers are **synthetic**. They're generated with a seeded random function for teaching purposes and don't represent any real company.
 
### 🎥 Demo
 
- 🌐 Live site: *add your link here*
- ▶️ YouTube Short: *add your link here*
### 🙏 Credits
 
- Map data: [Natural Earth](https://www.naturalearthdata.com/) (public domain) and [world-atlas](https://github.com/topojson/world-atlas) (ISC)
- [D3.js](https://d3js.org/) (ISC)
- Fonts: [Alexandria](https://fonts.google.com/specimen/Alexandria) & [Rubik](https://fonts.google.com/specimen/Rubik) (SIL Open Font License)
---
 
<div dir="rtl" align="right">
## 🇪🇬 العربية
 
طلاب كتير بيحفظوا تعريفات الـ Drill Down والـ Data Mart والـ Data Mining من غير ما يحسّوا بالفرق بينهم. المشروع ده بيحوّل كل مفهوم لحاجة **تشوفها وتدوس عليها**: بتنزل من الكوكب لحد فرع واحد، وبتشوف الجداول وهي بتطير على الـ Data Mart بتاع كل قسم، وبتسيب الخوارزمية تكتشف الأنماط لوحدها.
 
### ✨ المميزات
 
**🌍 Drill Down بستايل Google Earth**
- بتطير من كرة أرضية بتلف ← مصر ← الإقليم ← المحافظة ← الفرع، على حدود المحافظات الحقيقية.
- الكاميرا بتميل كل ما تنزل أعمق، ومعاها عدّاد ارتفاع ودبابيس واقفة على الخريطة.
- لوحة جانبية بتعرض الأرقام في كل مستوى، وبتأكد إن **مجموع اللي تحت = الرقم اللي فوق**.
- استعلام SQL بيتكتب لوحده مع كل خطوة، فتشوف الـ `WHERE` والـ `GROUP BY` بيتغيّروا إزاي. والـ Roll Up بيرجّعك لفوق.
**📦 بناء Data Mart**
- اختار قسم (مبيعات، HR، مالية، تسويق) وشوف الجداول اللي محتاجها بس وهي بتطير من المستودع.
- بيوضّح الجداول المشتركة بين الأقسام، والفرق بين الـ Dependent والـ Independent Data Mart.
**⛏️ معمل الـ Data Mining**
- **Association Rules** على 16 فاتورة سوبر ماركت، بالـ Support والـ Confidence والـ Lift، ومعاها حد أدنى للثقة تقدر تغيّره.
- **K-Means Clustering** متحرّك خطوة بخطوة، بيقسّم 45 زبون من غير أي تصنيف مسبق.
**🃏 مقارنة واختبار**
- كروت بتتقلب، وجداول مقارنة، واختبار من 6 أسئلة.
**🧳 رحلة الداتا**
- مسار متحرّك: المصادر ← ETL ← Data Warehouse ← Data Marts ← Drill Down / Mining / تقارير.
**وكمان:** ثيم فضاء بوضع غامق وفاتح، وتصميم بيظبط على الموبايل، وواجهة عربي من اليمين للشمال، وبيحترم إعداد تقليل الحركة.
 
### 🧠 المفاهيم الأربعة في سطر
 
| المفهوم | هو إيه | تخزين ولا استخدام؟ |
|---|---|---|
| 🏢 **Data Warehouse** | مخزن مركزي لكل داتا الشركة، متنظّم للتحليل | تخزين |
| 📦 **Data Mart** | حتّة أصغر من المستودع لقسم واحد | تخزين |
| 🌍 **Drill Down** | عملية OLAP بتنزل من الملخّص للتفاصيل | استخدام: *إنت* اللي بتسأل |
| ⛏️ **Data Mining** | خوارزميات بتكتشف أنماط مستخبية وبتتوقّع | استخدام: *الداتا* هي اللي بتجاوب |
 
### 🚀 التشغيل
 
مش محتاج تسطّب أي حاجة.
 
1. نزّل الريبو أو اعمله clone.
2. افتح `index.html` في أي متصفح حديث.
> محتاج نت أول مرة بس، عشان يحمّل مكتبة D3.js والخطوط. داتا الخريطة موجودة جوّه الملف.
 
**عشان تنشره على GitHub Pages:** ادخل على **Settings ← Pages ← Deploy from a branch**، واختار `main` و`/ (root)`، ودوس Save. الموقع هيبقى على `https://<username>.github.io/<repo-name>/`.
 
### 🛠 التقنيات
 
- **HTML و CSS و JavaScript** عادي في ملف واحد
- **D3.js v7** لإسقاط الكرة الأرضية وحركة الزووم الناعمة
- **داتا الخريطة:** Natural Earth و world-atlas، متبسّطة بـ mapshaper ومحطوطة جوّه الملف
- **الخطوط:** Alexandria و Rubik من Google Fonts
### ⚠️ عن الداتا
 
كل أرقام المبيعات والفواتير والزباين **وهمية**، اتعملت بدالة عشوائية ثابتة عشان الشرح، ومالهاش علاقة بأي شركة حقيقية.
 
### 🎥 الديمو
 
- 🌐 الموقع: *حط اللينك هنا*
- ▶️ يوتيوب Short: *حط اللينك هنا*
</div>
 
