# Hifz - Juz Amma memorisation site

A responsive static website for Juz 30 testing and recitation.

## Run locally
Open `index.html`, or use a local server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy with GitHub Pages
1. Create a public GitHub repository.
2. Upload `index.html`, `styles.css`, and `app.js` to the repository root.
3. Open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then save.

## Content and audio
The site fetches Uthmani text and verse audio at runtime from the AlQuran Cloud API. It contains no reciter portraits. Test mode excludes every surah's final verse from the random starting pool. Recitation mode supports Minshawi, Husary, and Alafasy.

## Production notes
Before a public launch, verify every displayed ayah against an approved Madinah Mushaf and add an offline/error policy. Do not silently substitute or edit Qur'anic text.

## Visual asset
The landing page background is stored at `assets/masjid-al-haram-sunset.png`. Keep the `assets` folder beside `index.html`. The CSS combines emerald overlays, warm gold highlights, ivory panels, and a responsive mobile crop.
