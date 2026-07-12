# Split Guide — Adjusting Region Borders

## When to use splits?

When two or more regions claim the same chunk(s) (e.g. Kandarin and Fremennik), overlapping areas occur. These chunks are shown on the map with **yellow dashed borders**. The split mechanism lets you divide these chunks between regions, giving each region a clean boundary.

## ⚠️ Important: How to make a chunk splittable

A chunk only becomes splittable (yellow dashed) when it is **added to BOTH regions** in `static/Map1.csv`. For example, if the border between Kandarin and Fremennik runs through `chunk_8_23`, that chunk must appear in **both** the Kandarin row AND a Fremennik row in the CSV.

## How to use splits

### 1. Open the split editor
- **Right-click** on a chunk with yellow dashed borders (overlapping chunk)
- The split editor dialog opens

### 2. Choose split direction
- **Vertical (left | right)** — Splits the chunk into a left and right portion
- **Horizontal (top / bottom)** — Splits the chunk into a top and bottom portion
- **Both (H + V)** — Splits the chunk into 4 quadrants (for complex boundaries)

### 3. Set the split position
- Use the **slider** (5%–95%) to position the split line
- With "Both" you get two sliders: one for vertical, one for horizontal

### 4. Assign regions to sides/quadrants
- For Vertical/Horizontal splits: two regions are shown with `⇄ Swap` to flip sides
- For "Both": assign a region to each quadrant (↖ TL, ↗ TR, ↙ BL, ↘ BR) via dropdowns
- In the quadrants you can also hold the right mouse button on the lines to move

### 5. Save or remove
- Click **✓ Save** to save the split
- Click **✕ Remove** to delete an existing split
- Click **Cancel** to discard changes

### 6. Move existing split lines
- **Right-click + drag** an existing split line to reposition it
- Your cursor changes to ↔ or ↕ depending on the split direction

## Tips
- Use the **✂ Splits** button (top-left) to see how many overlapping chunks exist
- Splits are saved in your browser (localStorage) and persist between sessions
- Resetting all chunks does NOT clear splits
