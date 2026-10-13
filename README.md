# RFDS Port Augusta Centre for Rural Health and Education

Photography-integrated architectural scrollytelling preview, based on the unchanged PACRE ivory GLB MESH.

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
