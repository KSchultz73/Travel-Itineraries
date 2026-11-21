# Travel Itineraries — rules for AI agents

This repository is **public**. It holds only the code of a single-page app (`index.html`).

## Never put personal data in this repository

All personal data lives in the owner's Dropbox, in `Apps/Travel Itineraries/`
(`travel-data.json`, plus the `wardrobe/`, `outfits/` and `attachments/` photo folders).
The app reads and writes it through the Dropbox API.

**Do not commit, push, upload or open a pull request containing any of:**

- photos of any kind, especially clothing / closet photos (`.jpg`, `.jpeg`, `.png`, `.heic`, …)
- `travel-data.json` or any copy or export of it
- names of garments, trip details, confirmation numbers, passport or traveller details,
  or any lists derived from the owner's closet or trips
- seed files, fixtures or "starter" data built from the above

If the user attaches photos or data in chat and asks you to add them to the closet,
**do not write them into the repository.** Tell the user to add them through the app itself
(the 📷 button on a garment, or the closet's own photo import), which stores them in Dropbox.
If the app lacks a way to do what the user wants, build that feature in code — never
by shipping their files with the page.

The app must never load trips or photos from beside the page; Dropbox is the only source.
