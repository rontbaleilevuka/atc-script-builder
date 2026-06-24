# SIM Script Builder
### NZ Airways · Total Control · ATC Training

A standalone web app for building, saving, loading and printing ATC simulation scripts. No installation required — opens directly in any browser on computer or iPad.

---

## 🌐 Live App
**[Open SIM Script Builder](https://rontbaleilevuka.github.io/atc-script-builder)**

**[User Guide & Troubleshooting](https://rontbaleilevuka.github.io/atc-script-builder/ATC_Script_Builder_Guide.html)**

---

## Features
- Colour-coded ATC scripts matching the original Word document format
- IFR and VFR departure 3-call system with pushback, same-call and skip options
- Aircraft type dropdown (194 sim aircraft) and separate transponder field
- Full NZ, Australian and Pacific airport dropdowns including hospital helipads
- Frequency management — toggle on TWR / GND / DEL / APP / DEP / INFO / APRON
- Save scripts as `.json` and load them back instantly
- Export to PDF for Apple Pencil annotation in GoodNotes or Notability
- ATIS and QNH footer reference on every script
- Edit individual entries without starting from scratch
- Keyboard navigation for fast data entry
- Strip separator borders for easy reading during simulation
- Works fully offline once loaded

## Colour Code Reference
| Colour | Type |
|--------|------|
| 🔵 Medium blue | VFR Departure |
| 🔵 Light blue | IFR Departure |
| 🩷 Medium pink | VFR Arrival |
| 🩷 Light pink | IFR Arrival |
| 🟢 Green | VFR / IFR Transit / T&G |
| 🟣 Purple | Ground Vehicle / Tug |
| 🟡 Yellow | Co-Ord / X-NOTE / Data Block |

## Adding a New Aircraft to the Dropdown
1. Open `index.html` in **Notepad** (right-click → Open with → Notepad)
2. Press **Ctrl+F** and search for `SECTION 4 — AIRCRAFT LIST`
3. Find the alphabetical position for your new aircraft
4. Add a new line in the format: `'B350',`
5. Save the file (**Ctrl+S**) and hard-refresh the browser (**Ctrl+Shift+R**)

**Example — adding a B350:**
```javascript
// Before
'B212','B412',

// After
'B212','B350','B412',
```

> ⚠️ Always keep a backup copy of the file before editing.

## Files
| File | Purpose |
|------|---------|
| `index.html` | The complete app — open in any browser |
| `ATC_Script_Builder_Guide.html` | User guide and troubleshooting |
| `README.md` | This file |

## Updating the App
When a new version is provided:
1. Download the new `index.html`
2. Upload it to this GitHub repository (replace the existing file)
3. GitHub Pages updates automatically within a minute

---

*NZ Airways · Total Control · ATC Training · Version 2.3*
