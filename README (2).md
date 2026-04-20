
```
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║    ██████╗  █████╗ ██╗   ██╗██████╗  █████╗ ███╗   ███╗██╗      █████╗ ██████╗     ║
║    ██╔══██╗██╔══██╗╚██╗ ██╔╝██╔══██╗██╔══██╗████╗ ████║██║     ██╔══██╗██╔══██╗    ║
║    ██████╔╝███████║ ╚████╔╝ ██████╔╝███████║██╔████╔██║██║     ███████║██████╔╝    ║
║    ██╔══██╗██╔══██║  ╚██╔╝  ██╔══██╗██╔══██║██║╚██╔╝██║██║     ██╔══██║██╔══██╗    ║
║    ██████╔╝██║  ██║   ██║   ██║  ██║██║  ██║██║ ╚═╝ ██║███████╗██║  ██║██║  ██║    ║
║    ╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝    ║
║                                                                              ║
║              K A L E N D A R І   —   2 0 2 6   ·   O ' Z B E K I S T O N              ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

<div align="center">

[![License](https://img.shields.io/badge/License-MIT-orange.svg?style=flat-square)](LICENSE)
[![Security](https://img.shields.io/badge/Security-AES--256--GCM-green.svg?style=flat-square)](#xavfsizlik)
[![API](https://img.shields.io/badge/API-Calendarific-blue.svg?style=flat-square)](https://calendarific.com)
[![Version](https://img.shields.io/badge/Version-2.0.0-red.svg?style=flat-square)](#)
[![HTML](https://img.shields.io/badge/Stack-Vanilla%20HTML%2FJS-yellow.svg?style=flat-square)](#)

**O'zbekiston va 14+ dunyo davlati uchun yillik bayramlar va kuzatuv kunlari kalendarі**  
*Bitta xavfsiz HTML fayl — server, framework, build tool kerak emas*

</div>

---

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                                             │
│   📁  bayramlar-xavfsiz.html          ← Yagona fayl, hammasi shu yerda     │
│                                                                             │
│   🔐  Parol bilan himoyalangan        ← AES-256-GCM + PBKDF2-SHA256        │
│   🌍  15+ davlat                      ← O'zbekiston, Rossiya, AQSh...       │
│   📅  2024 – 2030                     ← Ko'p yillik qo'llab-quvvatlash      │
│   ⚡  Zero dependencies               ← CDN ham yo'q, offline ishlaydi      │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

## 📋 Mundarija

- [Xususiyatlar](#-xususiyatlar)
- [Skrinshot](#-ko'rinish)
- [Tez Boshlash](#-tez-boshlash)
- [Xavfsizlik Arxitekturasi](#-xavfsizlik-arxitekturasi)
- [Parolni O'zgartirish](#-parolni-ozgartirish)
- [Qo'llab-quvvatlanadigan Davlatlar](#-qollabquvvatlanadigan-davlatlar)
- [API](#-api)
- [Fayl Tuzilmasi](#-fayl-tuzilmasi)
- [Muallif](#-muallif)

---

## ✨ Xususiyatlar

```
  ╭──────────────────────────────────────────────────────────────────────╮
  │                                                                      │
  │   🗓️   YILLIK KO'RINISH          12 oylik to'liq ko'rinish          │
  │   🔴   DAVLAT BAYRAMLARI         Rasmiy ta'til kunlari               │
  │   🔵   KUZATUV KUNLARI           Norasmiy muhim sanalar              │
  │   🌟   BUGUN BELGILASH           Joriy kun avtomatik ajralib turadi   │
  │   ⏩   KEYINGI BAYRAMLAR         Yaqin bayramlarga tezkor navigatsiya │
  │   📊   STATISTIKA                Bayram, dam olish, ish kunlari soni  │
  │   🔍   POPUP BATAFSIL            Har bir kun ustida batafsil ma'lumot │
  │   🔐   PAROL HIMOYA              AES-256-GCM shifrlash                │
  │   🛡️   BRUTE-FORCE HIMOYA        5 urinish → 30 daqiqa blok           │
  │   🔑   PAROL YANGILASH           Interfeysdan turib yangilash         │
  │   📱   RESPONSIVE                Mobil, planshet, desktop             │
  │                                                                      │
  ╰──────────────────────────────────────────────────────────────────────╯
```

---

## 🖼️ Ko'rinish

```
┌────────────────────────────────────────────────────────────────────────────┐
│  LOGIN SAHIFASI (Split-Panel Premium Design)                               │
│                                                                            │
│  ┌──────────────────────────┐  ┌───────────────────────────────────────┐  │
│  │  ████████████████████   │  │                                       │  │
│  │  ██  BREND PANELI   ██  │  │   Xavfsiz kirish                      │  │
│  │  ████████████████████   │  │   ─────────────                       │  │
│  │                         │  │   Xush kelibsiz                       │  │
│  │  📅  Bayramlar           │  │                                       │  │
│  │      Kalendarі           │  │   Parol                               │  │
│  │                         │  │   ┌─────────────────────────────┐     │  │
│  │  O'zbekiston va dunyo   │  │   │ ••••••••••••          👁    │     │  │
│  │  davlatlarining rasmiy  │  │   └─────────────────────────────┘     │  │
│  │  bayramlari...          │  │                                       │  │
│  │                         │  │   ┌─────────────────────────────┐     │  │
│  │  ─────────────────────  │  │   │         Kirish →            │     │  │
│  │  15+    365    2026     │  │   └─────────────────────────────┘     │  │
│  │  Davlat  Kun    Yil     │  │                                       │  │
│  │                         │  │   🟢  AES-256 · PBKDF2 · Himoya       │  │
│  └──────────────────────────┘  └───────────────────────────────────────┘  │
└────────────────────────────────────────────────────────────────────────────┘

┌────────────────────────────────────────────────────────────────────────────┐
│  ASOSIY INTERFEYS                                                          │
│                                                                            │
│  O'zbekiston 2026               [Yil ▾] [Davlat ▾]  🔑 Parol              │
│  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   │
│   9 Bayram  |  12 Kuzatuv  |  104 Dam olish  |  252 Ish kuni             │
│  ─────────────────────────────────────────────────────────────────────    │
│  ⏩  Yanvar 1  Yangi Yil  [3 kun]   Mart 8  Xotin-qizlar [15 kun]  ...   │
│  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   │
│                                                                            │
│  ┌──────────────┬──────────────┬──────────────┐   │  Barchasi  Bayram   │  │
│  │   YANVAR     │   FEVRAL     │    MART       │   │  ──────────────────│  │
│  │ Du Se Ch...  │ Du Se Ch...  │ Du Se Ch...   │   │  1 Yan  Yangi Yil  │  │
│  │  1  2  3 ... │  1  2  3 ...│  1  2  3 ...  │   │  8 Mar  Xotin-qizl │  │
│  │ [8][9][10]...│ [5][6][7]...│ [7][8] 9 ...  │   │  21 Mar Navro'z    │  │
│  └──────────────┴──────────────┴──────────────┘   │  ...               │  │
└────────────────────────────────────────────────────────────────────────────┘
```

---

## 🚀 Tez Boshlash

### 1-qadam — Faylni yuklab oling

```bash
# Yoki to'g'ridan-to'g'ri brauzerda oching
open bayramlar-xavfsiz.html
```

### 2-qadam — Brauzerni oching

```
bayramlar-xavfsiz.html  →  Ikki marta bosing  →  Brauzerda ochildi ✓
```

### 3-qadam — Parol kiriting

```
Standart parol:  Boburjon20061805
```

> ⚠️ **Muhim:** Standart parolni birinchi ishlatishdan so'ng o'zgartiring!

---

## 🔐 Xavfsizlik Arxitekturasi

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                    XAVFSIZLIK QATLAMLARI                                    │
│                                                                             │
│   FOYDALANUVCHI PAROLI                                                      │
│          │                                                                  │
│          ▼                                                                  │
│   ┌─────────────────────────────────────────────────────────────────────┐  │
│   │  PBKDF2-SHA256                                                      │  │
│   │  ├── Iteratsiyalar: 310,000                                         │  │
│   │  ├── Salt: 16 byte tasodifiy                                        │  │
│   │  └── Chiqish: 256-bit kalit                                         │  │
│   └─────────────────────────────────────────────────────────────────────┘  │
│          │                                                                  │
│          ▼                                                                  │
│   ┌─────────────────────────────────────────────────────────────────────┐  │
│   │  AES-256-GCM DESHIFRLASH                                            │  │
│   │  ├── IV: 12 byte tasodifiy                                          │  │
│   │  ├── Auth Tag: 128-bit                                              │  │
│   │  └── Noto'g'ri parol → AuthenticationError → hech narsa chiqmaydi  │  │
│   └─────────────────────────────────────────────────────────────────────┘  │
│          │                                                                  │
│          ▼                                                                  │
│   ┌─────────────────────────────────────────────────────────────────────┐  │
│   │  API KALIT (faqat xotirada)                                         │  │
│   │  ├── localStorage / sessionStorage ga YOZILMAYDI                   │  │
│   │  ├── DOM ga CHIQARILMAYDI                                           │  │
│   │  └── Sahifa yopilsa → yo'qoladi                                     │  │
│   └─────────────────────────────────────────────────────────────────────┘  │
│                                                                             │
│   BRUTE-FORCE HIMOYASI                                                      │
│   ┌─────────────────────────────────────────────────────────────────────┐  │
│   │  Urinish 1  →  2 soniya kutish                                      │  │
│   │  Urinish 2  →  4 soniya kutish                                      │  │
│   │  Urinish 3  →  8 soniya kutish                                      │  │
│   │  Urinish 4  →  16 soniya kutish                                     │  │
│   │  Urinish 5  →  30 DAQIQA TO'LIQ BLOK  🚫                           │  │
│   └─────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Nimalar himoyalangan?

| Tahdid | Himoya | Status |
|--------|--------|--------|
| API kalitni HTML-dan o'qish | AES-256-GCM shifrlash | ✅ Himoyalangan |
| Brute-force parol taxminlash | Eksponensial kechiktirish + blok | ✅ Himoyalangan |
| Network sniffing | Parol hech qachon yuborilmaydi | ✅ Himoyalangan |
| DOM inspection | API kalit JS xotirasida | ✅ Himoyalangan |
| localStorage xacking | Hech narsa saqlanmaydi | ✅ Himoyalangan |
| Noto'g'ri parol bilan ochish | GCM auth tag xatolik beradi | ✅ Himoyalangan |

---

## 🔑 Parolni O'zgartirish

```
1.  Saytga kiring (joriy parol bilan)
       │
       ▼
2.  Header-dagi  🔑 Parol  tugmasini bosing
       │
       ▼
3.  Formani to'ldiring:
    ┌─────────────────────────────────┐
    │  Joriy parol:   ••••••••••••   │
    │  Yangi parol:   ••••••••••••   │
    │  Tasdiqlash:    ••••••••••••   │
    └─────────────────────────────────┘
       │
       ▼
4.  "O'zgartirish" tugmasini bosing
       │
       ▼
5.  Konsolni oching  (F12 → Console)
       │
       ▼
6.  Yangi ENCRYPTED_PAYLOAD ni nusxalang:
    {
      "iv":   "...",
      "ct":   "...",
      "salt": "...",
      "iter": 310000
    }
       │
       ▼
7.  HTML fayldagi  ENCRYPTED_PAYLOAD  ni yangi bilan almashtiring
       │
       ▼
8.  Faylni saqlang  ✅
```

> 💡 **Eslatma:** Brauzer yopilganda o'zgarish yo'qoladi — faqat HTML fayl tahrirlanganda doimiy bo'ladi.

---

## 🌍 Qo'llab-quvvatlanadigan Davlatlar

```
  ┌─────┬──────────────────────────┐   ┌─────┬──────────────────────────┐
  │ UZ  │ 🇺🇿  O'zbekiston         │   │ DE  │ 🇩🇪  Germaniya            │
  │ RU  │ 🇷🇺  Rossiya             │   │ US  │ 🇺🇸  AQSh                 │
  │ KZ  │ 🇰🇿  Qozog'iston         │   │ GB  │ 🇬🇧  Britaniya            │
  │ KG  │ 🇰🇬  Qirg'iziston        │   │ FR  │ 🇫🇷  Fransiya             │
  │ TJ  │ 🇹🇯  Tojikiston          │   │ CN  │ 🇨🇳  Xitoy               │
  │ TR  │ 🇹🇷  Turkiya             │   │ AE  │ 🇦🇪  BAA                 │
  │ JP  │ 🇯🇵  Yaponiya            │   │ IN  │ 🇮🇳  Hindiston           │
  │ SA  │ 🇸🇦  Saudiya Arabistoni  │   │     │                          │
  └─────┴──────────────────────────┘   └─────┴──────────────────────────┘
```

---

## 📡 API

Loyiha **[Calendarific API](https://calendarific.com)** dan foydalanadi.

```
Endpoint:
  GET https://calendarific.com/api/v2/holidays
      ?api_key={SHIFRLANGAN_KALIT}
      &country={UZ|RU|KZ|...}
      &year={2024..2030}
      &type=national,observance

Javob formati:
  {
    "response": {
      "holidays": [
        {
          "name": "Yangi Yil",
          "description": "...",
          "primary_type": "Public Holiday",
          "date": {
            "iso": "2026-01-01",
            "datetime": { "year": 2026, "month": 1, "day": 1 }
          }
        }
      ]
    }
  }
```

---

## 📁 Fayl Tuzilmasi

```
bayramlar-xavfsiz.html
│
├── <head>
│   ├── Google Fonts (Sora + Playfair Display)
│   └── <style>
│       ├── :root — CSS o'zgaruvchilar
│       ├── #lockScreen — Premium login sahifasi
│       ├── #changePwModal — Parol o'zgartirish modali
│       ├── header, .stats-bar, .upcoming-bar
│       ├── .main, .cal-area, .sidebar
│       └── .popup, footer
│
└── <body>
    ├── #lockScreen — Split-panel login ekrani
    │   ├── .lock-left — Brend paneli (dekorativ)
    │   └── .lock-right — Kirish formasi
    │
    ├── #changePwModal — Parol modali
    │
    ├── header — Logo, yil/davlat tanlash, 🔑 tugma
    ├── .stats-bar — 4 ta statistika kartasi
    ├── .upcoming-bar — Yaqin bayramlar chipi
    │
    ├── #loadingEl — Yuklash animatsiyasi
    │
    ├── .main
    │   ├── .cal-area — 12 oylik grid
    │   └── .sidebar — Bayramlar ro'yxati + filtr
    │
    ├── footer — Ma'lumot + soat
    ├── .popup — Hover tooltip
    │
    └── <script>
        ├── ENCRYPTED_PAYLOAD — Shifrlangan API kalit
        ├── BF — Brute-force himoya holati
        ├── decryptApiKey() — PBKDF2 + AES-GCM
        ├── encryptApiKey() — Qayta shifrlash
        ├── tryUnlock() — Parol tekshirish
        ├── doChangePw() — Parol yangilash
        ├── loadData() — API so'rov
        ├── renderCalendar() — Oylik grid
        ├── renderSidebar() — Ro'yxat
        └── renderStats() — Statistika
```

---

## 🛠️ Texnik Talablar

```
  Brauzer          │  Chrome 80+, Firefox 75+, Safari 14+, Edge 80+
  Internet         │  API so'rovlari uchun kerak (birinchi yuklashda)
  Server           │  Kerak emas — to'g'ridan-to'g'ri fayl sifatida ishlaydi
  Framework        │  Yo'q — Vanilla HTML/CSS/JS
  Build tool       │  Yo'q
  Node.js          │  Kerak emas
  Hajm             │  ~45 KB (bitta fayl)
```

---

## 📝 Litsenziya

```
MIT License

Copyright (c) 2026

Har qanday maqsadda bepul ishlatish, nusxalash, o'zgartirish va
tarqatish mumkin. Muallif mas'uliyati yo'q.
```

---

```
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║   Made with  ♥  in Toshkent                                                 ║
║                                                                              ║
║   🔐  Xavfsiz     🎨  Premium     📅  To'liq     ⚡  Tez                   ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

<div align="center">
<sub>Calendarific API · AES-256-GCM · PBKDF2-SHA256 · Vanilla JS · 2026</sub>
</div>
