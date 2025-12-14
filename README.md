# NityaSeva Contents Repository

This repository contains **structured devotional content** used by the **NityaSeva Android / iOS app**.

All data here is **language-wise**, **category-wise**, and follows a **strict JSON schema** so the app can load content both online and offline.

---

## 📁 Repository Structure

```
.
├── english/
│   ├── aarti.json
│   ├── chalisa.json
│   ├── ashtakam.json
│   ├── katha.json
│   ├── ramcharitmanas.json
│   └── mantras.json
│
├── hindi/
│   ├── aarti.json
│   ├── chalisa.json
│   ├── ashtakam.json
│   ├── katha.json
│   ├── ramcharitmanas.json
│   └── mantras.json
│
├── marathi/
│   ├── aarti.json
│   ├── chalisa.json
│   ├── ashtakam.json
│   ├── katha.json
│   ├── ramcharitmanas.json
│   └── mantras.json
│
├── images/
│   ├── ganapati.png
│   ├── durga.png
│   └── shankar.png
│
├── example.json
└── README.md
```

---

## 🌍 Languages

Each top-level folder represents a language:

- `english` → English content
- `hindi` → हिंदी सामग्री
- `marathi` → मराठी सामग्री

All languages follow **the same JSON structure**.

---

## 📖 Categories

Each JSON file corresponds to a category used in the app:

| File | Category Code |
|---|---|
| `aarti.json` | `aarti` |
| `chalisa.json` | `chalisa` |
| `ashtakam.json` | `ashtakam` |
| `katha.json` | `katha` |
| `ramcharitmanas.json` | `ramcharitmanas` |
| `mantras.json` | `mantra` |

---

## 🧩 JSON Schema

```json
{
  "category": "aarti",
  "version": 2,
  "items": [
    {
      "id": "unique_item_id",
      "title": "Display Title",
      "language": "english",
      "image": "optional_image_url",
      "orderIndex": 1,
      "content": [
        {
          "shloka": "Main text shown to user",
          "meaning": "Optional meaning",
          "transliteration": "Optional transliteration",
          "imageUrl": "Optional per-block image"
        }
      ]
    }
  ]
}
```

---

## 🖼 Images

Images can be referenced using absolute GitHub URLs from the `images/` folder.

---

## 🔁 Versioning

Increase `version` only when structure changes.

---

## 🚀 Used By

NityaSeva Android & iOS apps. || AmolSoftwares ||

---

🙏 Om Namah Shivaya
