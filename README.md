# sentinel-2-grid

> ESA Sentinel Tile Grid as GeoJSON with extracted properties

## file download

```
wget -O grid.geojson https://unpkg.com/sentinel-2-grid/data/grid.json
```

## npm module

```
npm install sentinel-2-grid
```

```js
const grid = require('sentinel-2-grid')

console.log(grid.features.length)
// => 56686
```

## example feature

```json
{
  "type":"Feature",
  "geometry":{ ... },
  "properties":{
    "name":"01CCV",
    "id":"01CCV",
    "epsg":"32701",
    "mgrsRef":"-72.01265627 177.18928449 -72.077536527 -179.91249232 -72.972797991 179.93922476 -72.9043013 176.89507973",
    "utmWkt":"MULTIPOLYGON(((300000 2000020,300000 1890220,409800 1890220,409800 2000020,300000 2000020)))",
    "llWkt":"MULTIPOLYGON(((177.189340361676 -72.0124778858137,176.864623786205 -72.9914734627827,-179.775147078577 -73.064632943735,-179.627444421211 -72.081397340079,177.189340361676 -72.0124778858137)))"
  }
}
```

## build from src

```
npm run build
```
