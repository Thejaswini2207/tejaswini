# Tejaswini — tejaswini.shop

Traditional sarees from Mysuru, Karnataka.

---

## Folder structure

```
tejaswini-repo/
├── index.html        ← All page content (text, sections, links)
├── css/
│   └── style.css     ← All colours, fonts, layout, spacing
├── images/
│   ├── img_pink_temple1.jpg   ← Hero photo
│   ├── img_pink_temple2.jpg   ← Gallery photo 1
│   ├── img_bridal.jpg         ← Gallery photo 2
│   ├── img_maroon.jpg         ← Gallery photo 3
│   ├── img_temple_back.jpg    ← Gallery photo 4
│   ├── img_navy.jpg           ← Gallery photo 5
│   ├── img_lake.jpg           ← Gallery photo 6 (Cauvery)
│   └── img_paisley.jpg        ← Story section photo
├── CNAME             ← Routes tejaswini.shop to this repo
└── README.md         ← This file
```

---

## How to edit

### Change text
Open `index.html` — every section has a comment like:
```
<!-- ══ HERO SECTION — edit text here ══ -->
```
Find the comment for the section you want, then change the text between the tags.

### Change a photo
1. Add your new photo to the `images/` folder
2. In `index.html`, find the `<img src="images/OLD_NAME.jpg">` line
3. Change it to `<img src="images/YOUR_NEW_PHOTO.jpg">`

### Change colours
Open `css/style.css` — the top section has all colour variables:
```css
:root {
  --gold-bright: #E8B84B;   ← main gold
  --maroon-deep: #3D0E0E;   ← dark maroon
  --ivory:       #FAF6EC;   ← page background
}
```
Change the hex code next to any variable to update that colour everywhere.

### Change phone number
Search `index.html` for `+91 81237 44571` and replace both occurrences
(one in the visible text, one in the `href="tel:..."` attribute).

---

## Deploying to GitHub Pages + tejaswini.shop

See the hosting guide shared with you for full step-by-step instructions.
Short version:
1. Push this folder to a GitHub repo
2. Enable Pages in repo Settings → Pages → branch: main
3. GitHub Pages will automatically use the `CNAME` file to serve tejaswini.shop
4. Point GoDaddy DNS A records to GitHub's IPs (185.199.108–111.153)
