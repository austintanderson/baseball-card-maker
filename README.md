# Baseball Card Maker

Make custom youth baseball cards right in the browser. Change the names, stats, photos, logo and colors, then print the cards at real trading-card size (2.5 × 3.5 in) or download them as images.

Everything happens on your own computer. Photos you add are never uploaded anywhere. They stay in your browser, and in any design file you choose to save.

## Using it

1. Open the page.
2. Fill in the fields on the left. The card preview on the right updates as you type.
3. Click **Choose image…** to add a player photo, then drag the photo on the card to position it. Use the zoom slider to size it.
4. When the card looks right:
   - **Print / save PDF** prints the front and back as two card-size pages. In the print dialog, set margins to *None*. To get a PDF, pick *Save as PDF* as the printer.
   - **Front PNG** and **Back PNG** download high-resolution images (600 dpi at card size).
5. **Save design file** keeps a copy of the card, photos included, as a `.json` file. **Open design file** loads it back. Send the file to someone else and they can keep editing it.

**New player** clears the player's details and photo but keeps the colors, logo and team text, so the next card for the same team is quick to make. Your current card is also saved in your browser automatically.

## Hosting it on GitHub Pages

### Option 1: on the GitHub website (no software needed)

1. Sign in to GitHub and click **New repository**. Give it a name, such as `baseball-cards`, set it to **Public**, and click **Create repository**.
2. On the new repository's page, click **uploading an existing file**, or use **Add file → Upload files**.
3. Drag in `index.html`, `README.md` and `.nojekyll` from this folder, then click **Commit changes**.
   - `.nojekyll` starts with a dot, so your computer may hide it. If you can't see it, the site still works without it.
4. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the **main** branch and the **/ (root)** folder, and click **Save**.
5. After a minute or two, the site will be live at:
   `https://YOUR-USERNAME.github.io/baseball-cards/`
   The exact link also appears at the top of the Pages settings screen.

### Option 2: from the command line

```bash
cd baseball-card-maker
git init
git add .
git commit -m "Baseball card maker"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/baseball-cards.git
git push -u origin main
```

Then turn on Pages as in step 4 above.

## Sharing a team's starting design

You can give other people a link that opens with your team's colors, logo and text already filled in:

1. Set up a card the way you want everyone to start, then click **Save design file**.
2. Upload that `.json` file to the repository. You can put it in a folder, for example `designs/raptors.json`.
3. Share a link with `?design=` and the file's path at the end:
   `https://YOUR-USERNAME.github.io/baseball-cards/?design=designs/raptors.json`

Anyone who opens that link starts from your design. Their changes stay on their own computer.

**Note:** anything in a public repository can be seen by anyone. Leave player photos and personal details out of design files you upload. Use them for team colors, the logo and league text only.

## Good to know

- **Fonts:** the card uses two free Google fonts, Graduate and Archivo Narrow. They load automatically when you're online. If you're offline, the page uses similar fonts unless those two are installed on your computer.
- **PNG downloads** need an internet connection the first time, because the page loads a small helper library. Printing and saving PDFs work offline.
- **Works offline:** you can also download `index.html` and open it by double-clicking. It works the same way without hosting.
- **Print layout:** when printing, the page asks whether to rotate the back to portrait. Choose *rotate* for double-sided printing, so the back lines up with the front.
