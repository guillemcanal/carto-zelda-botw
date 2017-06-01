## Calcul de la taille de la carte


![Report de la distance sur la carte](assets/measure.png)

```js
// [...] Calculate Map distances

const PIXELS_DISTANCE = 428;
const PIXELS_MAP_WIDTH = 24000;
const PIXELS_MAP_HEIGHT = 20000;
const METERS_PER_PIXEL = GROUND_DISTANCE / PIXELS_DISTANCE;
const MAP_WIDTH = METERS_PER_PIXEL * PIXELS_MAP_WIDTH;
const MAP_HEIGHT = METERS_PER_PIXEL * PIXELS_MAP_HEIGHT;

console.log("map width : %dm", Math.round(MAP_WIDTH));
console.log("map height : %dm", Math.round(MAP_HEIGHT));
```

Affiche `map width : 11358m` et `map height : 9465m`
