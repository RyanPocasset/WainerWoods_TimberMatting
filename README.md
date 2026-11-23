# Wainer Woods S1 Mat Crossing

Timber mat layout for the temporary crossing where the brook passes under the raised stone laneway in Stand 1 at Wainer Woods, Westport, MA. One self-contained page: a to-scale plan on 2025 leaf-off imagery and lidar relief, a breakdown in feet, ground profiles along and across the lane, and a crew sheet for mats and materials.

Prepared by the PPLT Land Division, 23 Nov 2026. For field layout; not a survey.

## What's in the repo

| File | Purpose |
|---|---|
| `index.html` | The whole site. Imagery, layout data and code are embedded, so it has no other files to load. |
| `.nojekyll` | Tells GitHub Pages to serve the file as-is. |
| `README.md` | This file. |

## Publish on GitHub Pages

1. Create a new repository, for example `wainer-woods-s1-mat-crossing`.
2. Upload `index.html`, `.nojekyll` and `README.md` to the root of the `main` branch.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The site comes up at `https://<your-username>.github.io/wainer-woods-s1-mat-crossing/` within a minute or two.

To embed it in a story map or another page, use that URL in an iframe or embed block.

A GitHub Pages site is public to anyone with the link, even when it's published from a private repository (the exception is GitHub Enterprise Cloud's access-controlled Pages). That includes the crossing coordinates, stand outlines and the NRCS references in the header and feet table.

## Using the page

- **Lidar relief / 2025 aerial** switch the base map.
- **Drag the mats** to move the layout, for example onto the NRCS planner's field flag; **Rotate** turns it. The stakeout coordinates for the west end, culvert and east end update as you go.
- **Measure** gives the distance in feet between two clicks.
- **Copy coordinates** copies the stakeout table.

## Layout summary

- 16 timber mats, 4 × 16 ft, 8-inch hardwood.
- 13 deck mats laid crosswise on the lane crown, stations 0+00 to 0+52 (28 ft west to 24 ft east of the culvert), 16 ft wide.
- 3 bridge mats laid lengthwise under deck mats 6–9, stations 0+20 to 0+36, centered over the culvert.
- About 2,400 lb a mat, about 38,400 lb in all.

## Data sources

- MassGIS spring 2025 leaf-off orthophotos (15 cm).
- USGS 3DEP 1 m lidar elevation (profiles, causeway measurements, brook flow path).
- MassGIS lidar slope and shaded relief.
- PPLT Wainer Woods planning layer (stands, parcels).
- NRCS FY26 conservation plan map for Wainer Woods 2 LLC, 6/25/2026 (655 line placement).
- Walden Forest Conservation forest management plan, Aug 2023, with the Northeast Engineers & Consultants survey.

## Editing

The page's data sits in the `const D = {...}` line inside the `<script>` block (map frame in metres relative to the culvert point at 41.546222, -71.070716). Text and tables are plain HTML above it.
