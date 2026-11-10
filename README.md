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

## Good to know

- **Fonts:** the card uses two free Google fonts, Graduate and Archivo Narrow. They load automatically when you're online. If you're offline, the page uses similar fonts unless those two are installed on your computer.
- **PNG downloads** need an internet connection the first time, because the page loads a small helper library. Printing and saving PDFs work offline.
- **Works offline:** you can also download `index.html` and open it by double-clicking. It works the same way without hosting.
- **Print layout:** when printing, the page asks whether to rotate the back to portrait. Choose *rotate* for double-sided printing, so the back lines up with the front.
