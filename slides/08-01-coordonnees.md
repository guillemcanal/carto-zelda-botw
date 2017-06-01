## Obtenir les coordonnées Nord/Sud/Est/Ouest de la carte

Positionner **centre de symétrie** de notre carte  
sur les coordonnées correspondantes au **barycentre** (centre de masse) de **Paris**.

- Récupération des contours de Paris avec [OverPass Turbo](http://overpass-turbo.eu/) d'[OpenStreepMap](http://openstreetmap.fr/)
- Calcul des coordonnées de la carte avec [TURF.js](http://turfjs.org/)
- Géoréférencement de la carte avec [gdal_translate](http://www.gdal.org/gdal_translate.html) de la librairie [GDAL](http://www.gdal.org/)
- Génération de tuiles pour afficher la carte avec [Leaflet](http://leafletjs.com/)