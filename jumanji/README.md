# Jumanji — jamoaviy dars o'yini

## Ishga tushirish
`index.html` faylini brauzerda oching (Chrome, Edge, Firefox). Internet yoki o'rnatish kerak emas.

## Qoidalar
1. Jamoalar sonini (2–6) va har bir jamoaning nomi va tokenini tanlang. Tokenlar takrorlanmasligi kerak.
2. Navbatdagi jamoa **🎲 Zarni tashlash** tugmasini bosadi. Zar 1 dan 6 gacha tasodifiy son tushiradi.
3. Savol chiqadi. O'qituvchi jamoaning javobini baholaydi:
   - **✅ To'g'ri** — token tushgan son qadar yuradi (masalan, 5 tushsa 5 katak).
   - **❌ Noto'g'ri** — token joyida qoladi.
4. Navbat keyingi jamoaga o'tadi.
5. Birinchi bo'lib oxirgi katak (🏁 FINISH) ga yetgan jamoa yutadi.

**👁 Javobni ko'rsatish** tugmasi javobni faqat o'qituvchiga ko'rsatadi (ekranda ko'rinadi).

## Savollarni o'zgartirish
`index.html` faylini matn muharririda oching. `<script>` ichidagi `QUESTIONS` ro'yxatini o'z mavzuingizdagi savollar bilan almashtiring:

```js
const QUESTIONS = [
  { q: "Savol matni?", a: "To'g'ri javob" },
  { q: "Boshqa savol?", a: "Javob" },
];
```

Hozirgi savollar namuna. Savollar tugasa, ro'yxat avtomatik qayta aralashtiriladi.

## Boshqa sozlamalar (`index.html`, `<script>` ichida)
- `CELLS` — taxtadagi katakchalar soni (hozir 36, ya'ni 6 x 6). Kattaroq son o'yinni uzoqroq qiladi. Qiymat `COLS` (6) ga karrali bo'lishi kerak.
- `STEP_DELAY` — token qadamlari orasidagi kechikish, millisekundda (hozir 350).
