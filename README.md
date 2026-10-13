# RFDS Port Augusta Centre for Rural Health and Education

Photography-integrated architectural scrollytelling preview, based on the unchanged V4 ivory GLB.

**OPENING MID-2027**

**RFDS Port Augusta Centre for Rural Health and Education.**

The story opens on the real building (PACRE-198 cut-out), which dissolves into the ivory model. The floors separate and the floor in focus turns blue: the ground floor for **Health**, Level 02 for **Education** and **Training**. In **Together under one roof** the floors settle, the roof goes back on and the model turns into the real drone photograph, matched to the same camera. The last two chapters move to a satellite map: the model on its site at 38 Mackay Street, Port Augusta, then out to outback South Australia. The header uses the supplied RFDS SA & NT colour logo.

## Preview locally

No installation or build is required. Serve the `site` folder over HTTP:

```sh
python3 -m http.server 8080 --directory site
```

Open `http://localhost:8080`. File URLs may prevent the model from loading. The Three.js dependencies, model, images and logo are packaged locally.

The map chapters need an internet connection: CesiumJS 1.120 loads from the jsDelivr CDN and the satellite imagery from Mapbox, using the public token in `site/map.js` (restrict it to your domain in your Mapbox account). Both load only once a reader reaches the Training chapter; if either fails, the original photographs show instead. The model's position on the map (`SITE` at the top of `map.js`) is set from the street address and recent aerial imagery; check the heading against the real building.

`previews/` and `VALIDATION.md` describe the earlier version and have not been regenerated.

## Package contents

- `site/`: complete runnable website, model, web images, logo and browser-readable audit.
- `photography/`: all original supplied images, every-file visual audit, image inventory, masks and contact sheet.
- `previews/`: desktop and mobile browser captures, including the updated logo.
- `VALIDATION.md`: checks performed and remaining limitations.

## Image and model distinctions

Photography is supplied project imagery. Education and Training photo transitions show roof and courtyard details, not classrooms or training sessions. The V4 model is a schematic preview, with illustrative interiors and separation; it is not BIM or a surveyed architectural model.

Museo Sans 100/300/500/700/900 is selected when installed locally. Licensed webfont files were not supplied, so devices without Museo use Avenir Next/Arial fallback. The client's photographic grade, logo proportions and colours are retained.

Construction is complete; service opening is mid-2027. Content follows the supplied approved copy, including the $21m project, bulk-billed GP and nurse-led primary healthcare, School of the Air, workforce placements, local and outback audiences, and both $1m seed funders.

Client-supplied logos, photography and model assets are included for this project preview. Their inclusion does not grant permission for unrelated reuse. Three.js retains its upstream licence information.
