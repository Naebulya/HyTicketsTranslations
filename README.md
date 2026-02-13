# HyTickets Translations

Community translation files for **HyTickets** — a Hytale server plugin that provides an in-game support ticket system.

- HyTickets (CurseForge): https://www.curseforge.com/hytale/mods/hytickets  
- Translations repo: https://github.com/winglessraven/HyTicketsTranslations

---

## Repository structure

- **One JSON file per language** (e.g. `EN.json`, `DE.json`, `FR.json`).
- Files contain a **flat key/value map** of translation keys to translated strings used by HyTickets (UI labels, messages, etc.).

---

## Translation file format

- JSON object with `"key": "value"` pairs  
- **Translate values only** — keys must stay exactly the same  
- Strings may include **placeholders** (keep them exactly as-is). Placeholders include:

| Placeholder |
|---|
| `{count}` |
| `{filter}` |
| `{page}` |
| `{pages}` |
| `{id}` |
| `{status}` |
| `{preview}` |
| `{assigned}` |
| `{name}` |
| `{world}` |
| `{coords}` |
| `{role}` |
| `{author}` |
| `{content}` |
| `{owner}` |
| `{updated}` |
| `{message}` |
| `{thread}` |
| `{minutes}` |
| `{version}` |
| `{location}` |


  - **Do not translate, remove, or rename placeholders** — keep them exactly as-is

Example:

```json
{
  "ticketsHeader": "Tickets",
  "openTicketsCount": "Open tickets: {count}"
}
```

## Add a new language

1. Copy `EN.json`
2. Rename it using a sensible language code (examples: `DE.json`, `ES.json`, `FR.json`)
3. Translate **values only**
4. Open a Pull Request

**Tips:**
- Keep button labels short (e.g., “View”, “Close”, “Reply”)
- Keep tone consistent across the file
- Preserve punctuation and formatting where it matters

## Contribution guidelines

- Prefer **natural, in-context phrasing** over literal translation
- Keep UI text concise
- Keep placeholders (e.g. `{count}`) unchanged

---

## License / usage

Translations in this repository are intended to be used by HyTickets.
