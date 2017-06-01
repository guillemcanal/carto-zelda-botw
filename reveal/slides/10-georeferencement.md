## Géoréférencement

Utilisation de l'utilitaire [gdal_translate](http://www.gdal.org/gdal_translate.html) fournie par la librairie  
[GDAL](http://www.gdal.org/) (Geospatial Data Abstraction Library).

```sh
echo "---> Géoréférencement de la carte"
gdal_translate \
    -of GTiff \
    -r bilinear \
    -a_srs EPSG:4326 \
    -gcp 12000 0 2.35703 48.8927 \
    -gcp 24000 10000 2.43459 48.8501 \
    -gcp 12000 20000 2.35703 48.8076 \
    -gcp 0 10000 2.27947 48.8501 \
    BigMap.png \
    BigMap.tif
```

Retoune un fichier **TIF** contenant des métadonnées spaciales
