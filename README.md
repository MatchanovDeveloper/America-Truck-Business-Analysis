# 🚛 America Truck Business Analysis — Power BI Dashboard

Power BI’da tayyorlangan interaktiv biznes tahlil dashboardi. Loyihada AQShdagi yuk tashish (trucking) biznesi bo‘yicha ma’lumotlar tahlil qilingan va DAX yordamida yillar kesimida solishtiruvchi ko‘rsatkichlar yaratilgan.

## 📌 Loyiha haqida

Ma’lumotlar tayyor Excel fayl shaklida olingan va Power BI’ga yuklab, star schema modeli asosida qayta ishlangan. Maqsad — biznes ko‘rsatkichlarini (daromad, foyda, yetkazib berish samaradorligi) real vaqt rejimida kuzatish va oldingi yil bilan solishtirish imkonini beruvchi dashboard yaratish edi.

## 🛠 Ishlatilgan vositalar

- **Power BI Desktop** — modellashtirish va vizualizatsiya
- **DAX** — measure’lar va vaqt intelligensiyasi (time intelligence)
- **Excel** — dastlabki ma’lumotlar manbai

## 🗂 Ma’lumotlar modeli

Star schema arxitekturasi:
- **Trip** — fakt jadval (har bir reys bo‘yicha ma’lumotlar: daromad, xarajat, masofa, sana va h.k.)
- **State** — o‘lchov (dimension) jadvali — shtatlar bo‘yicha geografik kesim

## 📐 Yaratilgan DAX measure’lar

- Umumiy daromad (Total Revenue) va foyda (Profit)
- Yetkazib berish darajasi (Delivery Rate)
- Faol haydovchilar va yuk mashinalari soni
- Oldingi yil bilan solishtirish — `SAMEPERIODLASTYEAR` / `DATEADD` funksiyalari asosida YoY (Year-over-Year) o‘sish/pasayish foizi
- Trend ko‘rsatkichlari uchun shartli ▲ / ▼ belgilar va rang formatlash (yashil — o‘sish, qizil — pasayish)

## 📊 Dashboard imkoniyatlari

- KPI kartalar — asosiy ko‘rsatkichlar va ularning yillik dinamikasi
- Gauge vizual — maqsad va bajarilish darajasini ko‘rsatish
- Line chart’lar — vaqt bo‘yicha trend tahlili
- Clustered bar chart va jadval — shtatlar kesimida taqqoslash
- Slicer’lar — sana, shtat va boshqa kesimlar bo‘yicha filtrlash
- Dark va Light rejim — ikkita alohida sahifa ko‘rinishida

## 🖼 Skrinshotlar

> `screenshots/` papkasiga dashboard sahifalaridan skrinshotlar qo‘shing (Power BI Desktop’da faylni oching → har bir sahifani PNG sifatida eksport qiling yoki Snipping Tool orqali screenshot oling).

## 🚀 Faylni ochish

1. [Power BI Desktop](https://www.microsoft.com/power-platform/products/power-bi/downloads) o‘rnatilgan bo‘lishi kerak
2. `.pbix` faylini yuklab oling
3. Power BI Desktop orqali oching

## 📫 Bog‘lanish

Savol yoki fikr-mulohazalar bo‘lsa, LinkedIn orqali murojaat qilishingiz mumkin.

---
### English Summary

Interactive Power BI dashboard analyzing U.S. trucking business performance, built from a prepared Excel dataset. Implemented a star schema (Trip fact table + State dimension table) and wrote DAX measures for revenue, profit, delivery rate, and fleet/driver counts, including year-over-year comparisons with trend indicators (▲/▼) and conditional formatting. The report includes KPI cards, gauge visuals, trend line charts, interactive slicers, and dark/light theme pages.
