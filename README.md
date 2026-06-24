<img width="407" height="777" alt="GARDEN" src="https://github.com/user-attachments/assets/9d850129-4b79-4416-98d5-03a02e48fe3c" />
# 🌸 Miso Garden

> A cozy browser-based gardening game — plant, water, harvest, and bloom your way through four seasons.

![HTML](https://img.shields.io/badge/HTML-Single%20File-FF9EC4?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-Vanilla-FFB8C8?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JS-Vanilla-FFE878?style=flat-square&logo=javascript&logoColor=black)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-B8F0DC?style=flat-square)

---

## 🌿 What is Miso Garden?

Miso Garden is a lightweight, zero-dependency cozy game that runs entirely in your browser from a single HTML file. You play as **Miso**, an adorable bunny gardener who tends a 12-plot garden through Spring, Summer, Autumn, and Winter. Plant seeds, water them to speed up growth, harvest for coins and XP, befriend visiting animal characters, and decorate your garden with cozy items.

No server. No install. No sign-up. Just open the file and grow.

---

## ✨ Features

- **12-plot garden grid** — start with 4 unlocked plots; earn more as you level up
- **6 unique crops** — Rose, Sunflower, Tulip, Mushroom, Blueberry, and Snowdrop, each with different grow times and coin rewards
- **4 seasons** — the sky gradient, season banner, and crop availability shift every few minutes of play
- **Tool system** — Plant 🌱, Water 💧, Harvest 🧺, and Remove ✂️ tools with context-sensitive feedback
- **Watering bonus** — watering a plot reduces grow time by 30% and boosts harvest reward
- **XP & leveling** — earn XP from harvests, visiting friends, and buying décor; level up to unlock new plots and refill water
- **4 garden friends** — Coco the Bunny Baker, Ribby the Frog Chef, Maple the Bear Explorer, and Mochi the Cat Artist; visit them for bonus coins and water
- **Garden décor shop** — 6 purchasable decorations from a bench to a windmill
- **Visitor events** — random friends drop by with gifts; claim coins and water from them
- **Water refill timer** — water slowly regenerates over time (1 per 30 seconds up to 10)
- **Harvest popup + confetti** — satisfying animated feedback on every harvest
- **Full localStorage persistence** — your garden saves automatically between sessions
- **Accessible markup** — ARIA labels on plots, tools, navigation, and dialogs
- **Mobile-friendly** — responsive max-width layout with a fixed bottom nav bar
- **Zero dependencies** — no frameworks, no build step, no npm; ships as one `.html` file

---

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/miso-garden.git
cd miso-garden
```

Then just open `index.html` in any modern browser:

```bash
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Or drag the file directly into your browser tab. That's it — no server required.

---

## 🎮 How to Play

| Action | How |
|---|---|
| **Plant** | Select the 🌱 Plant tool, pick a seed from the shop, tap an empty plot |
| **Water** | Select the 💧 Water tool, tap a growing plot (costs 1 water, speeds growth by 30%) |
| **Harvest** | Select the 🧺 Harvest tool, tap a glowing green plot when it's ready |
| **Remove** | Select the ✂️ Remove tool, tap any planted plot to clear it |
| **Visit friends** | Tap the 🐾 Friends tab and tap a friend card for bonus coins + water |
| **Buy décor** | Tap the 🏡 Décor tab and spend coins on garden items |
| **Level up** | Earn XP to unlock more plots and keep growing |

### Tips

- Watering always pays off — the coin bonus and speed boost outweigh the water cost on any high-value crop.
- Check the Friends tab whenever you need a coin injection between harvests.
- Seasons change every ~3 minutes of playtime; watch for the toast notification.
- Claim visitor gifts immediately — they disappear if you dismiss the banner.

---

## 🌱 Crops Reference

| Crop | Cost | Reward | Grow Time | XP |
|---|---|---|---|---|
| 🌷 Tulip | 12 🪙 | 28 🪙 | 6s | 10 |
| 🌹 Rose | 15 🪙 | 35 🪙 | 8s | 12 |
| 🌻 Sunflower | 18 🪙 | 40 🪙 | 10s | 14 |
| 🍄 Mushroom | 20 🪙 | 50 🪙 | 12s | 18 |
| 🫐 Blueberry | 22 🪙 | 55 🪙 | 14s | 20 |
| ❄️ Snowdrop | 25 🪙 | 65 🪙 | 16s | 24 |

*Watered crops yield 1.3× coins on harvest.*

---

## 🗂️ Project Structure

```
miso-garden/
└── index.html    # The entire game — HTML, CSS, and JS in one file
```

Everything lives in a single self-contained file. No build pipeline, no dependencies, no configuration.

---

## 🛠️ Customization

All game data lives in clearly labeled constant blocks at the top of the `<script>` tag in `index.html`:

- **`SEEDS`** — add or edit crops (id, emoji, cost, grow time, reward, XP)
- **`FRIENDS`** — add new animal companions with custom inline SVG avatars
- **`DECORS`** — add decoration items with costs
- **`PLOT_COUNT`** — change the number of garden plots
- **`UNLOCK_COSTS`** — adjust which plots unlock at which level
- CSS custom properties in `:root` control the entire color palette

---

## 💾 Save Data

Game state is saved automatically to `localStorage` under the key `misoGarden_v2`. To start fresh, use the **🔄 New Garden** button on the Profile tab, or clear site data in your browser's DevTools.

---

## 🌐 Deployment

Because it's a single HTML file, you can host it anywhere static files are served:

- **GitHub Pages** — push to a repo, enable Pages, done
- **Netlify / Vercel** — drag the file into the deploy drop zone
- **Itch.io** — upload as an HTML game (set it to play in browser)
- **Any web server** — drop the file into any public directory

---

## 🤝 Contributing

Contributions are welcome! Some ideas for what could be fun to add:

- More crop types and seasonal exclusives
- Garden music / ambient sound toggle
- Animated weather effects per season
- A gift/trade mechanic between friends
- Achievements and milestone badges
- Mobile PWA support for offline play

To contribute, fork the repo, make your changes in `index.html`, and open a pull request.

---

## 📄 License

MIT — do whatever you like with it, just keep the credit line if you redistribute.

---

*Made with 🌸 and a lot of tiny SVG bunnies.*<img width="407" height="777" alt="GARDEN" src="https://github.com/user-attachments/assets/d0237849-19a9-41f7-bb9c-6355761218bc" />
