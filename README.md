# SpotiStream – Spotify Now Playing Overlay for Streamers

**Hosted overlay:**  
https://kelvinph.github.io/SpotiStream/overlay.html

---

## 🚀 How to Use

1) Create a Spotify app: https://developer.spotify.com/dashboard/applications  
2) In your Spotify app → **Settings** → **Redirect URIs** → **Add**: https://kelvinph.github.io/SpotiStream/overlay.html > Save.  
3) Copy your **Client ID**.  
4) In **OBS** → **Sources** → **+** → **Browser** → URL: https://kelvinph.github.io/SpotiStream/overlay.html > (Size e.g. 600×160; you can resize later.)  
5) Right-click the Browser Source → **Interact** → **Connect to Spotify** → paste your **Client ID** → approve.  

**Notes**
- Each user must use their **own Client ID** (no secret needed).
- Works with free Spotify.  
- If overlay shows “Nothing playing”, make sure music is actually playing on your account.

---

## 🎨 Styling & Themes

SpotiStream supports **themes** and **custom switches** via URL parameters—no code edits.

Append options to your overlay URL, for example: https://kelvinph.github.io/SpotiStream/overlay.html?theme=spotify


### Preset Themes
- **Minimal**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=minimal&bar=4&radius=12`
- **Classic Spotify**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=spotify`
- **Old Radio (vintage/sepia)**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=oldradio&square=1&spin=0&font=inter`
- **Blue**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=blue`
- **Red**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=red`
- **Yellow**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=yellow`
- **OBS Dark**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=obsdark`
- **Neon**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=neon`
- **Mint Glass**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=mintglass`
- **Sunset**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=sunset`
- **Ice**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=ice`
- **Vapor**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=vapor`
- **Mono**  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=mono`

### Layout Toggles
- `&compact=1` → tighter spacing  
- `&square=1` → square album art  
- `&vinyl=1` → vinyl record texture on art  
- `&spin=0` → stop spinning cover

**Examples**
- Compact + square art (OBS Dark):  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=obsdark&compact=1&square=1`
- Vapor + no shadow + taller bar:  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=vapor&shadow=0&bar=10`

### Visual Knobs (mix & match)
- `&accent=%23ff66cc` → accent color  
- `&panel=rgba(0,0,0,0.35)` → panel background  
- `&text=%23ffffff` → text color  
- `&muted=%23aaaaaa` → secondary text color  
- `&radius=20` → corner radius (px)  
- `&blur=8` → background blur (px)  
- `&shadow=0` → disable shadow  
- `&art=96` → album art size (px)  
- `&bar=4` → progress bar height (px)

### Fonts (Google Fonts)
Pick one with `&font=`: `inter`, `rubik`, `montserrat`, `poppins`, `firasans`  
- Example:  
  `https://kelvinph.github.io/SpotiStream/overlay.html?theme=oldradio&square=1&spin=0&font=inter`

---

## ❓ Troubleshooting

- **After login it loops/blank:** Make sure the **Redirect URI** in your Spotify app **exactly** equals  
  `https://kelvinph.github.io/SpotiStream/overlay.html`
- **Doesn’t update in OBS:** Right-click Browser Source → **Interact** and login **inside OBS** once.  
  In Browser Source properties, uncheck “Refresh browser when scene becomes active” and “Shutdown source when not visible” if you want to keep the session alive.
- **Nothing playing:** Ensure Spotify is actively playing on any device under your account.

---

## 🔒 Privacy / Tokens

This is a client-only overlay using OAuth **PKCE**. No server, no client secret. Tokens are stored locally in your browser/OBS instance.


