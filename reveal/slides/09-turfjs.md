## Calcul des coordonnées de la carte

Utiliser la librairie d'analyse spaciale **TURFJS** (http://turfjs.org/) pour calculer les coordonnées Nord Sud Est Ouest

```js
const destination = require("@turf/destination");
const point = require("@turf/helpers").point;
const getCoord = require("@turf/invariant").getCoord;

const NORTH = 0, EAST = 90, SOUTH = 180, WEST = 270;
const PARIS_CENTROID = point([2.3570288419096928, 48.85016763056825]);
const HORIZONTAL_DISTANCE = 11.358 / 2;
const VERTICAL_DISTANCE = 9.465 / 2;

getCoord(destination(PARIS_CENTROID, VERTICAL_DISTANCE, NORTH)).join(", ");
getCoord(destination(PARIS_CENTROID, HORIZONTAL_DISTANCE, EAST)).join(", ");
getCoord(destination(PARIS_CENTROID, VERTICAL_DISTANCE, SOUTH)).join(", ");
getCoord(destination(PARIS_CENTROID, HORIZONTAL_DISTANCE, WEST)).join(", ");
```

- **north**: 2.3570288419096928, 48.892714669097316  
- **east**: 2.4346186135996386, 48.85014159947358  
- **south**: 2.3570288419096928, 48.807620592039214  
- **west**: 2.279439070219747, 48.85014159947358  
