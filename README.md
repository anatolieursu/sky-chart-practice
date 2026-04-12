# Skychart Exam — Instrucțiuni

## Structura folderului

```
skychart-exam/
  index.html          ← aplicația
  exam-example.json   ← exemplu examen iarnă
  exam-vara.json      ← exemplu examen vară
  charts/
    orion-winter.jpg  ← imaginile tale de skychart
    summer-sky.jpg
    ...
```

## Formatul JSON

```json
{
  "title": "Numele examenului",
  "image": "charts/numele-imaginii.jpg",
  "tasks": {
    "directions": {
      "enabled": true,
      "items": ["N", "S", "E", "V"]
    },
    "zenit": true,
    "pnc": true,
    "lst": true,
    "month": false,
    "constellations": [
      "Orion",
      "Taurus",
      "Gemini"
    ],
    "messier": [
      "M42",
      "M45",
      "M1"
    ]
  }
}
```

### Câmpurile `tasks`

| Câmp | Tip | Descriere |
|------|-----|-----------|
| `directions.enabled` | bool | activează sarcinile de orientare |
| `directions.items` | array | care direcții: N, S, E, V |
| `zenit` | bool | sarcină: marchează zenitul |
| `pnc` | bool | sarcină: marchează Polul Nord Ceresc |
| `lst` | bool | sarcină: scrie estimarea LST |
| `month` | bool | sarcină: scrie luna aproximativă |
| `constellations` | array | lista constelațiilor de desenat |
| `messier` | array | lista obiectelor Messier de marcat |

## Cum se folosește

1. Deschide `index.html` în browser (Chrome sau Firefox)
2. Trage fișierul `.json` pe fereastră
3. Dacă imaginea nu se încarcă automat, trage și fișierul imagine
4. Desenează cu uneltele din bara de sus
5. Bifează sarcinile cu `✓ bifează` sau tasta `Enter`
6. Apasă `↓ salvează hartă` — se salvează local în browser
7. Accesează hartile salvate din butonul `📁 harti salvate`

## Taste rapide

| Tastă | Unealtă |
|-------|---------|
| P | Creion |
| L | Linie |
| C | Cerc |
| T | Text |
| E | Radieră |
| Ctrl+Z | Undo |
| Enter | Bifează sarcina curentă |
