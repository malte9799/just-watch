<div align="center">

# ▶ just**watch**

**Search, browse and watch movies & series from one clean, fast page.**

No accounts. No backend. No build step. Just open it and press play.

[**Open the site →**](https://malte9799.github.io/just-watch/) &nbsp;·&nbsp; [Video demo](https://youtu.be/ZdbZgsT-24k)

</div>

---

## ✨ Features

| | |
|---|---|
| 🎬 **Cinematic home** | A rotating hero of today's trending titles, plus rows for popular and top-rated movies and series. |
| 🔎 **Instant search** | Results appear as you type. Press <kbd>/</kbd> anywhere to jump to the search bar. |
| 📺 **Episode guide** | Season picker and episode list with thumbnails, air dates and runtimes. Episodes you've watched get a ✓. |
| ⏭ **Next episode** | One click moves to the next episode, and on to the next season when the current one ends. |
| ⏯ **Continue watching** | Series resume at the last episode you played. |
| 🔖 **Watchlist** | Bookmark any poster to save it for later. |
| 🎞 **Trailers** | YouTube trailers play in an in-page dialog. |
| 🌗 **Theater mode** | Dims everything except the player. Toggle with <kbd>T</kbd> and exit with <kbd>Esc</kbd>. |
| 🛡 **Pop-up shield** | On sources known for pop-ups, a shield catches the first click and re-arms after 20 seconds. |
| 🔁 **Two sources** | Switch between **MultiEmbed** and **VSEmbed** without losing your place. Your choice is remembered. |
| 🔗 **Shareable links** | Every title and episode has its own URL, and browser back/forward work as you'd expect. |
| 📱 **Responsive** | Works on phones, tablets and desktops. |

## 🚀 Usage

1. Open the site.
2. Search for something, or pick a title from the home rows.
3. Press **Watch now**. For a series, choose a season and episode from the sidebar.

### Open by IMDb ID

Click the **#** button in the top bar, then paste an IMDb ID or link (for example `tt1553656`). For a series, add a season and an episode.

### URL parameters

| URL | Opens |
|---|---|
| `?id=tt0816692` | A movie |
| `?id=tt0903747&s=1&e=1` | A specific episode |
| `?q=dune` | Search results |
| `?view=library` | Your history and watchlist |

## 🧱 How it's built

- **One file:** [`index.html`](index.html) contains the HTML, CSS and vanilla JS. There are no frameworks and no build step.
- **Metadata:** [TMDB API](https://www.themoviedb.org/) provides titles, posters, seasons, episodes, cast and trailers. The API key is built in.
- **Playback:** third-party embed players, looked up by IMDb ID.
- **Storage:** `localStorage` holds history, the watchlist, watched episodes and your preferred source. Nothing leaves your browser.
- **Look:** Inter and Bricolage Grotesque fonts, with Bootstrap Icons.
- **Hosting:** GitHub Pages.

## 🛠 Run locally

```bash
git clone https://github.com/malte9799/just-watch.git
cd just-watch
python3 -m http.server 8000   # then open http://localhost:8000
```

You can also open `index.html` directly in a browser.

## ⌨️ Shortcuts

| Key | Action |
|---|---|
| <kbd>/</kbd> | Focus search |
| <kbd>T</kbd> | Toggle theater mode |
| <kbd>Esc</kbd> | Exit theater mode or close a dialog |
| <kbd>Enter</kbd> | Open the focused poster |

---

<div align="center">
<sub>Metadata & images by <a href="https://www.themoviedb.org/">TMDB</a>. This product uses the TMDB API but is not endorsed or certified by TMDB.<br>This project hosts no media; all streams come from third-party embed providers.</sub>
</div>
