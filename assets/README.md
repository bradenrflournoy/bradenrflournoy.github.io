# Screenshot assets

Drop real screenshots here to replace the placeholder frames on the cards.
Expected filenames (referenced by the placeholders in `index.html`):

- `yardly.png`        — a Yardly app/simulator screen
- `bytefight.png`     — an example ByteFight match in the GUI
- `delivery-eerd.png` — the Enhanced ERD (export a page of cs4400_phase1_eerd_team3.pdf as PNG)

## How to swap a placeholder for a real image

In `index.html`, find the card's `.shot` block, e.g.:

    <div class="shot">
      <div class="shot-ph" role="img" aria-label="...">
        <span class="shot-ph-label">App screenshot coming soon</span>
        <span class="shot-ph-hint">assets/yardly.png</span>
      </div>
    </div>

and replace the inner `.shot-ph` div with a single image tag:

    <div class="shot">
      <img src="assets/yardly.png" alt="Yardly app screen">
    </div>

The `.shot` frame keeps a consistent 16:10 area and crops via object-fit,
so images of slightly different sizes will still line up.

Recommended: roughly 16:10, ~800px+ wide, PNG or JPG.
