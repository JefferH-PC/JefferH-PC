# Jeffer Henrique

Software engineering student and developer building local-first web applications, backend services, and native Windows utilities.

[jeffer.contato.work@gmail.com](mailto:jeffer.contato.work@gmail.com)

---

## Projects

### [Kyos](https://github.com/JefferH-PC/project_kyos) · [Live App](https://project-kyos.vercel.app)
Personal finance and Brazilian fixed-income (`CDI`) yield dashboard.  
`React 19` · `JavaScript` · `PWA` · `Jest`

- Compounds daily returns strictly on Brazilian business days using cached [BrasilAPI](https://brasilapi.com.br) national holiday calendars, with automatic startup catch-up for missed working days.
- Models Brazilian fixed-income taxation across the 30-day regressive IOF table (`96%` down to `0%`) and IR brackets (`22.5%` to `15%`) for gross vs. net redeemable yield projections.
- Routes daily investment income through debt-recovery slots before funding wishlist targets so principal remains untouched, paired with an isolated CDI rate simulation sandbox and `localStorage` JSON backups.

### [Media Backlog](https://github.com/JefferH-PC/Media_Backlog) · [Live App](https://media-backlog-flame.vercel.app)
Local-first backlog tracker for games, movies, series, and books.  
`Next.js 15` · `TypeScript` · `Tailwind CSS 4` · `IndexedDB` · `PWA`

- Queries Steam, TVMaze, Open Library, iTunes, and Wikipedia through a unified `/api/media-lookup` endpoint with `HEAD` image verification to populate release metadata and cover options.
- Compresses custom cover uploads client-side to `300×450` WebP via HTML5 Canvas (`0.75` quality) with deterministic SVG fallbacks.
- Persists catalog entries, active-focus slots, completion dates, ratings, and review notes in IndexedDB, supporting validated JSON import/export with merge or overwrite conflict resolution (`EN` / `PT-BR`).

### [YouTube Daily Recap](https://github.com/JefferH-PC/yt_recap_bot)
Automated daily email digest of new uploads from subscribed YouTube channels.  
`Python 3.12` · `YouTube Data API v3` · `GitHub Actions` · `SMTP / MIME`

- Batches channel playlist lookups (50 IDs per request) to stay well within YouTube Data API v3 daily quota limits.
- Filters out YouTube Shorts via `#shorts` hashtag matching and `/shorts/` URL checks while deduplicating repeated video IDs and titles.
- Fetches video thumbnails with multi-tier YouTube CDN fallbacks and attaches them as inline `Content-ID` MIME parts so images render reliably across email clients on a daily GitHub Actions schedule.

---

## Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | TypeScript, JavaScript (ES2024+), Python 3, C++20, HTML5, CSS3 |
| **Frontend** | React 19, Next.js (App Router), Tailwind CSS, IndexedDB, Service Workers (PWA) |
| **Backend & Systems** | Node.js, Fastify, Win32 API, DirectX 11, Dear ImGui, REST APIs, SMTP / MIME |
| **Tooling & Testing** | Git, GitHub Actions, CMake, MSVC, Jest, React Testing Library, Vercel |
