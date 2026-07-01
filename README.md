# Pokemon AI Automation

A low-code automation project that generates Pokémon-themed Instagram content using Make.com, Airtable, PokéAPI, and Google Gemini.

The workflow automatically selects a Pokémon from a database, retrieves its official information from PokéAPI, generates an Instagram-ready post with Gemini, and stores the generated content back into Airtable.

---

## Features

- Selects the next Pokémon from Airtable.
- Retrieves official Pokémon data from PokéAPI.
- Generates:
  - Pokémon facts
  - Competitive move recommendations
  - Background theme
  - Background search query
  - Instagram caption
  - Hashtags
- Stores generated content back into Airtable.
- Prevents duplicate generation by marking processed Pokémon.

---

## Workflow

```
Scheduler
      │
      ▼
Airtable (Search Records)
      │
      ▼
PokéAPI (HTTP Request)
      │
      ▼
Google Gemini
      │
      ▼
Airtable (Update Record)
```

---

## Technologies Used

- Make.com
- Airtable
- PokéAPI
- Google Gemini API

---

## Database Structure

| Field | Purpose |
|--------|----------|
| Pokemon | Pokémon name |
| Posted | Indicates whether content has been generated |
| Theme Override | Optional custom background theme |
| Background Folder | Background category |
| Caption | AI generated content |
| Date Posted | Publishing date |

---

## Current Version

### Version 1

- Airtable integration
- PokéAPI integration
- Google Gemini integration
- Automatic database updates

---

## Planned Features

- Download official Pokémon artwork automatically.
- Random background selection based on Pokémon type.
- Canva integration for carousel generation.
- Automatic Instagram publishing.
- Error handling and retry system.
- Generation logs and analytics.

---

## Example Workflow

1. Search Airtable for the next unposted Pokémon.
2. Retrieve official Pokémon information from PokéAPI.
3. Generate Instagram content with Gemini.
4. Save the generated content to Airtable.
5. Mark the Pokémon as processed.

---

## Project Status

🚧 Active Development

This project is being built incrementally, with each version adding a new automation component while keeping previous functionality stable.

---

## License

MIT License