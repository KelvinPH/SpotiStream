# SpotiStream · Professional Spotify Overlay for Content Creators

[![Works in](https://img.shields.io/badge/OBS-Browser%20Source-6aa84f)](#-obs-setup)
[![Hosting](https://img.shields.io/badge/Hosting-GitHub%20Pages-1da1f2)](#-self-hosting--forks)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

The **most customizable Spotify overlay** for streamers and content creators. Features a stunning vinyl record aesthetic with deep customization options, multiple layouts, visual effects, and professional themes. No server required, no secrets exposed.

---

## 🔗 Quick Access

- **🎛️ Configurator (Start Here):** `https://kelvinph.github.io/SpotiStream/config.html`  
- **📺 Overlay:** `https://kelvinph.github.io/SpotiStream/overlay.html`  

> Use the **Configurator** to design your overlay visually with live preview, then copy the generated URL directly into OBS.

---

## ✨ Features

### 🎨 **10 Unique Layouts**
- **Record (Vinyl)** - Authentic spinning vinyl with grooves and optional tonearm
- **Card (Cover)** - Clean album artwork with text overlay
- **Bar (Minimal)** - Ultra-compact text-only strip
- **Stacked (Center)** - Centered vertical layout perfect for corners
- **Compact (Mini)** - Small 80px artwork for minimal footprint
- **Wide (Cinematic)** - Three-column layout with duplicate artwork
- **Split (Dual)** - Vertical artwork and text stacking
- **Floating (Overlay)** - Fixed top-right corner overlay
- **Corner (Tiny)** - Minimal 60px bottom-right widget
- **Ticker (Scroll)** - Full-width bottom scrolling bar

### 🎭 **19+ Professional Themes**
- **Classic**: Spotify, OBS Dark, Minimal, Neon
- **Creative**: Gaming, Lo-Fi, Cyberpunk, Retro Wave, Elegant
- **Atmospheric**: Sunset, Ocean, Forest, Midnight, Aurora
- **Artistic**: Gradient, Monochrome, Party, Cozy, Focus

### 🌟 **Visual Effects**
- **Particle Effects** - Floating accent-colored particles
- **Color Breathing** - Gentle hue rotation and brightness pulsing
- **Waveform Visualizer** - Animated bars that pulse with music
- **Album Blur Background** - Blurred artwork with hover-to-focus
- **5 Accent Styles**: Solid, Glow, Gradient, Pulse, Rainbow

### 🎯 **Advanced Customization**
- **Smart Text Alignment** - Auto-follows media position or manual override
- **Progress Bar Scaling** - Adjustable width (50%-100%)
- **Typography Control** - 5 Google Fonts + shadow options
- **Color Modes** - Theme-based or full custom color picker
- **Precise Sizing** - Media size, corner radius, blur, padding controls
- **Transparency Options** - Full transparency mode or custom opacity

### 🎵 **Intelligent Features**
- **Auto-accent Extraction** - Colors from album artwork
- **Marquee Text Scrolling** - Long titles scroll automatically
- **Responsive Design** - Scales perfectly in OBS
- **Demo Mode** - Test styling without Spotify connection
- **Text Shadows** - Enhanced readability over any background

---

## 🚀 Quick Start Guide

### 1. **Spotify App Setup**
1. Visit [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications)
2. **Create App** → Name it anything → **Web API**
3. **Edit Settings** → **Redirect URIs** → Add exactly:  
   `https://kelvinph.github.io/SpotiStream/overlay.html`
4. **Save** → Copy your **Client ID**

### 2. **Design Your Overlay**
1. Open the [**Configurator**](https://kelvinph.github.io/SpotiStream/config.html)
2. Enable **Demo Mode** (toggle in header) to preview without login
3. Choose a **Quick Preset** or customize manually:
   - **Basic**: Layout, theme, positioning
   - **Visual**: Effects, animations, accent styles  
   - **Content**: Elements, text behavior
   - **Advanced**: Typography, colors, transparency
4. **Copy URL** when satisfied

### 3. **Add to OBS**
1. **Sources** → **+** → **Browser Source**
2. **URL**: Paste your copied URL
3. **Width**: 900, **Height**: 300 (adjust as needed)
4. **Custom CSS**: Leave blank
5. **✓ OK**

### 4. **First-Time Authentication**
1. **Right-click** Browser Source → **Interact**
2. **Connect to Spotify** → Paste **Client ID** → **Save**
3. **Connect to Spotify** → **Allow** in popup
4. Start playing music in Spotify

> **Important**: Always do the first login **inside OBS** using **Interact** to ensure tokens are stored correctly.

---

## 🎛️ Configurator Guide

### **Header Controls**
- **Demo Mode Toggle** - Preview with sample data
- **Copy URL** - Get your customized overlay URL
- **Open Preview** - Test in new window
- **Reset** - Start over with defaults

### **Tabs Overview**

#### **Basic Tab**
- **Quick Presets** - 14 pre-designed combinations
- **Layout & Style** - Choose layout, theme, accent style
- **Sizing & Positioning** - Media size, progress width, alignment
- **Behavior** - Spin, tonearm, compact spacing options

#### **Visual Tab**  
- **Visual Effects** - Particles, color breathing, waveform, album blur
- **Animations** - Track change effects, animation speed control

#### **Content Tab**
- **Elements** - Toggle status pill, progress bar, time, title, artist
- **Text & Motion** - Scrolling, auto-accent, marquee speed

#### **Advanced Tab**
- **Typography** - Font selection, shadow control
- **Colors & Custom** - Theme vs custom color mode
- **Background** - Transparency, panel opacity, background color
- **Quick Actions** - One-click transparent preset

---

## 🎨 Theme Gallery

### **Gaming Themes**
- **Gaming** - Bright green text on black, perfect for streams
- **Cyberpunk** - Neon cyan and hot pink, futuristic glow
- **Neon** - Electric blue accents with dark background

### **Atmospheric Themes**  
- **Lo-Fi** - Warm browns and oranges, cozy aesthetic
- **Sunset** - Orange and pink gradients, golden hour vibes
- **Ocean** - Blue tones with aqua accents, calming
- **Forest** - Green palette, natural and organic
- **Midnight** - Purple hues, mysterious night theme

### **Professional Themes**
- **Elegant** - Clean whites and blues, sophisticated
- **Minimal** - Pure white on dark, maximum readability
- **OBS Dark** - Matches OBS interface perfectly
- **Monochrome** - Black and white, timeless

---

## 🎭 Preset Collection

### **Creative Presets**
- **Record** - Classic Spotify vinyl with spinning animation
- **Gaming** - Compact layout with particle effects
- **Lo-Fi** - Wide cinematic with color breathing
- **Cyberpunk** - Floating overlay with all effects enabled
- **Elegant** - Split layout with album blur
- **Party** - Ticker layout with rainbow effects

### **Functional Presets**
- **Card** - Clean OBS Dark theme for professional streams
- **Bar** - Ultra-minimal for small overlay areas
- **Transparent** - See-through for gameplay overlays
- **Streamer** - Floating neon overlay for corner placement
- **Focus** - Compact minimal for distraction-free streaming
- **Ultra Minimal** - Bare-bones text only

---

## 🧩 OBS Integration

### **Recommended Settings**
- **Browser Source Properties**:
  - **Width**: 900px (scales automatically)
  - **Height**: 300px (adjust for layout)
  - **FPS**: 30 (sufficient for smooth animations)
  - **Custom CSS**: Leave blank
  - **✓ Shutdown source when not visible**: **OFF**
  - **✓ Refresh browser when scene becomes active**: **OFF**

### **Positioning Tips**
- **Bottom Third**: Classic position, doesn't obstruct content
- **Top Corner**: Use Corner or Floating layouts
- **Full Width**: Perfect for Ticker layout
- **Sidebar**: Compact or Split layouts work well

### **Performance Optimization**
- **Lower-end systems**: Reduce blur, disable particle effects
- **High refresh rate**: Enable all visual effects
- **Multiple scenes**: Keep source active to maintain authentication

---

## 🔧 Advanced Customization

### **URL Parameters**
All configurator settings can be controlled via URL parameters:

```
?layout=floating&theme=cyberpunk&particles=1&colorbreathing=1
&waveform=1&accentstyle=pulse&disc=140&progresswidth=80
&textalign=center&transparent=1&shadow=0
```

### **Key Parameters**
- `layout` - record, card, bar, stacked, compact, wide, split, floating, corner, ticker
- `theme` - Any theme name (spotify, gaming, cyberpunk, etc.)
- `particles` - 1 to enable particle effects
- `colorbreathing` - 1 to enable color breathing
- `waveform` - 1 to enable waveform visualizer
- `accentstyle` - solid, glow, gradient, pulse, rainbow
- `transparent` - 1 for full transparency
- `shadow` - 0 to disable text shadows

### **Custom Colors**
```
?colormode=custom&accent=%23ff0080&text=%23ffffff&muted=%23cccccc
```

---

## ❓ Troubleshooting

### **Authentication Issues**
**Problem**: "Redirect URI mismatch"  
**Solution**: Ensure Spotify app redirect URI is exactly:  
`https://kelvinph.github.io/SpotiStream/overlay.html`

**Problem**: OBS keeps asking to login  
**Solution**: Do first authentication **inside OBS** using **Interact**, not in regular browser

### **Display Issues**  
**Problem**: Shows "Nothing playing"  
**Solution**: Start music playback on the authenticated Spotify account (Free accounts work)

**Problem**: Overlay doesn't update  
**Solution**: Hard refresh (Ctrl+F5) or use incognito/private browsing

**Problem**: Visual effects not showing  
**Solution**: Check if effects are enabled in configurator Visual tab, ensure modern browser

### **Performance Issues**
**Problem**: Overlay causes frame drops  
**Solution**: Reduce blur amount, disable particle effects, use simpler layouts

**Problem**: Text hard to read  
**Solution**: Enable text shadows in Advanced tab, or use higher contrast themes

---

## 🔒 Privacy & Security

### **Data Handling**
- **No Server Required** - Everything runs in your browser
- **OAuth 2.1 PKCE** - Industry-standard secure authentication
- **Local Storage Only** - Tokens stored in your browser/OBS environment
- **No Data Collection** - This project never sees your information
- **Open Source** - Full code transparency

### **Permissions Used**
- `user-read-currently-playing` - Get current track info
- `user-read-playback-state` - Get play/pause status

### **What We Don't Access**
- Your music library or playlists
- Personal information or email
- Listening history or recommendations
- Account details beyond current playback

---

## 🛠️ Development & Contributing

### **Self-Hosting**
1. Fork this repository
2. Enable GitHub Pages in Settings
3. Update redirect URI to your GitHub Pages URL
4. Customize as needed

### **Local Development**
```bash
git clone https://github.com/yourusername/SpotiStream
cd SpotiStream
# Serve locally (any static server works)
python -m http.server 8000
# Open http://localhost:8000/config.html
```

### **Contributing**
- 🐛 **Bug Reports** - Use GitHub Issues
- ✨ **Feature Requests** - Describe your use case
- 🔧 **Pull Requests** - Follow existing code style
- 🎨 **New Themes** - Add to THEMES object with PR

---

## 📄 License

MIT License - Feel free to use, modify, and distribute.

---

## 🙏 Acknowledgments

- **Spotify Web API** - For the excellent developer platform
- **OBS Studio** - For Browser Source capability
- **Google Fonts** - For beautiful typography options
- **Community** - For feedback and feature suggestions

---

**Made with ❤️ for content creators worldwide**

*Transform your streams with the most customizable Spotify overlay available.*