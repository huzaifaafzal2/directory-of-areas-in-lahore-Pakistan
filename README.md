
# 📍 Lahore Areas Directory

A simple, open-source JSON directory of **120 main areas** and **574 sub-areas** in Lahore, Pakistan.  
Perfect for use in apps, address selectors, and location-based projects.

---

## 🗂️ Dataset Structure

- **`areas.json`** contains:
```json
{
  "total_areas": 120,
  "areas": {
    "LHE_001": {
      "name": "Anarkali",
      "sub_areas": ["Anarkali Bazaar", "Anarkali Tomb"]
    },
    "LHE_002": {
      "name": "Badami Bagh",
      "sub_areas": ["Badami Bagh Wholesale Market", "Badami Bagh Railway Colony"]
    }
    // ... more areas
  }
}
```

- Each main area has:
  - Unique **ID** (`LHE_001`, `LHE_002`, etc.)
  - **Name**
  - Array of **sub_areas** (strings)

---

## 🧩 Example Use Case

Check **`use_case.html`** for a working example:  
✔️ Dropdown selector of main areas & sub-areas  
✔️ Displays the selected area  
✔️ Loads data from `areas.json`

---

## 🔄 How to Update/Add Areas

1. **Find the latest area ID** (e.g., if last ID is `"LHE_120"`, the next will be `"LHE_121"`).
2. Add a new entry like:
```json
"LHE_121": {
  "name": "New Area Name",
  "sub_areas": ["Sub Area 1", "Sub Area 2"]
}
```
3. **Update `total_areas`** to reflect the new count.

---

## ✨ Contribution Guide

- Fork the repo.
- Update `areas.json` carefully (follow the format).
- Make a pull request.
- Mention if you add new areas, fix names, or modify sub-areas.

All contributions welcome to keep the directory fresh and complete!

---

## 📜 License

MIT License — free to use, modify, and share.

---

## ✅ Notes
- Format is kept simple — no extra metadata (like coordinates or types) to keep it lightweight.
- Ideal for dropdowns, forms, address validation, etc.
