# PT Quest — NPTE Study PWA

A static, offline-capable NPTE study companion with flashcards, practice exams, local progress, and rewards. This is an unofficial educational resource; questions are not official FSBPT exam questions and have not been independently clinically validated.

## Deploy on GitHub Pages

1. Create a GitHub repository (for example, `pt-quest`).
2. Upload **the contents of this folder to the repository root** (including `.github/workflows/pages.yml`). Commit to the `main` branch.
3. In GitHub, open **Settings → Pages → Build and deployment → Source**, and select **GitHub Actions**.
4. Open **Actions**, wait for the `Deploy PT Quest to GitHub Pages` workflow to finish, then visit `https://YOUR-USERNAME.github.io/pt-quest/` (replace both values as needed).
5. On Android Chrome, use **Install app**; on iOS Safari, use **Share → Add to Home Screen**. Open online once to cache files before using offline.

All app paths are relative, so project Pages URLs (with a repository subpath) work without editing the manifest or service worker. The site requires HTTPS for offline service-worker support (GitHub Pages provides this).

## Local test

Run `python -m http.server 8000` in this folder, then open `http://localhost:8000`.

## Notes

- Study and exam data are saved in your browser's local storage. They **do not sync** between devices. Use the app's export/backup functionality before clearing browser data or moving to another URL.
- For continuity, deploy to the same GitHub Pages URL each time. Changing URL/origin will not migrate progress.
- GitHub Pages sites are publicly accessible on the internet. Do not commit private personal information or copyrighted commercial question banks.
- This app is not affiliated with or endorsed by FSBPT.
