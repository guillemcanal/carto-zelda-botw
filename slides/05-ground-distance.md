## Calcul de la distance au sol

On s'élance d'une tour de `70m` de haut et on parcourt `214.3m` avant de toucher le sol.

Appliquer le **théorème de Pythagore** pour obtenir la distance parcourue au sol

```js
// Calculate the covered ground distance

const DISTANCE_TRAVELED = 214.3;
const TOWER_HEIGHT = 70;
const GROUND_DISTANCE = Math.sqrt(
    Math.pow(DISTANCE_TRAVELED, 2) - Math.pow(TOWER_HEIGHT, 2)
);

console.log("ground distance covered : %dm", Math.round(GROUND_DISTANCE));
```

### Distance parcourue : 203m