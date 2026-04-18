# Publications Folder

This folder contains the data used by `publications.html`.

## Structure
- `index.json` is the manifest file used by the page to discover publication entries.
- `entries/` contains one JSON file per publication.

## Adding a new publication
1. Create a new JSON file in `publications/entries/` with a unique `id` and the same field structure as the other publication files.
2. Add a manifest entry in `publications/index.json` with `id`, `file`, `year`, and `category`.
3. The page will automatically load the new entry when published.

## Example entry file
```json
{
  "id": "publication-slug",
  "category": "Lead Author Journal Publications",
  "year": 2026,
  "type": "Journal Article",
  "title": "Your publication title",
  "authors": "Author list",
  "status": "Published",
  "venue": "Journal Name",
  "notes": "vol. X, no. Y, pp. Z",
  "url": "https://example.com",
  "doi": "10.xxxx/xxxx",
  "abstract": "Abstract unavailable. Add a short summary here.",
  "keywords": "your keywords for filter search"
}
```