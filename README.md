# 💧 Fontaines autour de moi

Petite web app pour trouver les fontaines d'eau potable les plus proches.

👉 https://benoitleveque.github.io/fontaines-autour-de-moi/

- Géolocalisation, carte et liste triée par distance (avec temps de marche)
- Rayon de 500 m à 5 km, recherche dans la zone affichée
- Itinéraire à pied via Google Maps
- Indique les fontaines saisonnières, l'accessibilité, etc.

## Données

[OpenStreetMap](https://www.openstreetmap.org/copyright) (ODbL), interrogé en direct via l'API Overpass :
`amenity=drinking_water`, `amenity=water_point`, et `man_made=water_tap` / `amenity=fountain` / `natural=spring` avec `drinking_water=yes`.

## Technique

Un seul fichier `index.html` (Leaflet + tuiles OSM), sans build ni dépendance. Hébergé sur GitHub Pages (HTTPS requis pour la géolocalisation).
