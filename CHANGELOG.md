# Changelog

All notable changes to the omidtootoonchi.ir website are documented in this file.
This project uses date-based versioning (`YYYY.MM.DD`).

## [2026.10.16.1]

### Fixed
- **Duplicate without user-selected canonical** (Google Search Console): added `<link rel="canonical">` to every page and removed the duplicate `index.html` entry from `sitemap.xml` (only the canonical `https://omidtootoonchi.ir/` root remains).
- **Page with redirect**: canonical URLs now consistently use the `https://` non-`www` apex, aligning the sitemap, canonical tags, and the HTTP→HTTPS redirect so Google indexes the canonical HTTPS URL.

## [2026.10.16]

### Added
- Google Knowledge Graph structured data (schema.org / JSON-LD) across all pages, following Google's structured data documentation:
  - `index.html`: `Person` (Omid Tootoonchi) and `WebSite`.
  - `works.html`: `CollectionPage` with `ItemList` (filmography) and `BreadcrumbList`.
  - `contact.html`: `ContactPage`, `Person`, and `BreadcrumbList`.
  - `film-safe-zone.html`, `film-crumpling.html`, `film-oedipus.html`, `film-neurasthenia.html`: `Movie` schema (credits, cast, genre, awards) plus `BreadcrumbList`.

### Notes
- Website content is unchanged; only structured data was added inside `<head>`.
