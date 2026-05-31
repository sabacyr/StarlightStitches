# 🧶 Yarn Quest — My Knitting & Crochet HQ

A cutesy pixel-game-aesthetic website for tracking knitting and crochet projects, hosting PDF patterns, and managing your yarn stash. Built for GitHub Pages!

---

## 📁 Recommended Repo Structure

```
your-repo/
├── index.html          ← Main site (this file)
├── Knit/               ← Put all your knitting PDF patterns here
│   ├── Goyo-Balaclava.pdf
│   ├── Arctic-Holly-Sweater.pdf
│   └── ...
├── Crochet/            ← Put all your crochet PDF patterns here
│   ├── Hexagon-Cardigan.pdf
│   ├── Fox-Amigurumi.pdf
│   └── ...
└── README.md
```

---

## 🚀 GitHub Pages Setup

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch, **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/your-repo/` in a minute or two!

---

## 🪡 Linking to Your PDF Patterns

Once your PDFs are in the `Knit/` or `Crochet/` folders, you can link to them directly:

```
https://yourusername.github.io/your-repo/Knit/Goyo-Balaclava.pdf
https://yourusername.github.io/your-repo/Crochet/Hexagon-Cardigan.pdf
```

To add clickable links in the project cards, find the project in the `projects` array inside `index.html` and add a `patternUrl` field:

```js
{
  name: "Purple Rain Balaclava",
  craft: "knit",
  pattern: "Sijin Lee - Goyo Balaclava",
  patternUrl: "Knit/Goyo-Balaclava.pdf",   // ← add this
  yarn: "Mother Nature's Unicorn",
  status: "finished",
  rating: "5/5",
  notes: "Good pattern but I was bored kinda..."
}
```

---

## ✏️ Updating Your Projects

All your project data lives in the `projects` array near the bottom of `index.html`. Each entry looks like:

```js
{
  name: "Project Name",
  craft: "knit",         // "knit" or "crochet"
  pattern: "Designer - Pattern Name",
  yarn: "Brand Yarn Name",
  status: "finished",    // "finished", "wip", "frogged", "trashed", "future"
  rating: "5/5",
  notes: "Your notes here!"
}
```

---

## 🧶 Updating Your Stash

The stash data is in the `stash` array. Each entry:

```js
{
  brand: "Cascade",
  name: "Eco Duo",
  colorway: "Chinchilla",
  yardage: "197/100",
  weight: "Worsted (4)",
  fiber: "Alpaca + M Wool",
  skeins: "0/6",
  store: "Misty Acres Farm"
}
```

---

## 🎨 Customization Tips

- **Change your crafter name**: Search for `CRAFTY GOBLIN` and replace it with your own!
- **Add your cats' names**: The footer has a cat emoji section — make it yours!
- **Colors**: All colors are CSS variables at the top of the `<style>` block — easy to tweak.
- **Site title**: Change `YARN QUEST` in the `<title>` tag and `.site-title` heading.

---

*Made with love, yarn, and pixel art vibes* 🐱
