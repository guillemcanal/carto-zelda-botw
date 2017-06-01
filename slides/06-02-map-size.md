## Convertion des pixels en mètres

```js
// [...] Calculate Map distances

const PIXELS_DISTANCE = 428;
const PIXELS_MAP_WIDTH = 24000;
const PIXELS_MAP_HEIGHT = 20000;

const METERS_PER_PIXEL = GROUND_DISTANCE / PIXELS_DISTANCE;
const MAP_WIDTH = METERS_PER_PIXEL * PIXELS_MAP_WIDTH;
const MAP_HEIGHT = METERS_PER_PIXEL * PIXELS_MAP_HEIGHT;
const AREA = (MAP_WIDTH  * MAP_HEIGHT)/1000000;

console.log("map width : %dm", Math.round(MAP_WIDTH));
console.log("map height : %dm", Math.round(MAP_HEIGHT));
console.log("area : %d km2", AREA.toFixed(2));
```

Largeur : **11358m**  
Hauteur : **9465m**  
Surface : **107,5 km2**

