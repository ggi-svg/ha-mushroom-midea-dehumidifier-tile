# Configuration

Le fichier principal à adapter est :

- `lovelace/dehumidifier_tile.yaml`

## Entités par défaut

- `humidifier.deshumidificateur`
- `select.deshumidificateur_fan_speed`
- `sensor.deshumidificateur_current_humidity`

## Mapping recommandé

Si vos entités sont différentes, remplacez **toutes** les occurrences dans le YAML :

- humidificateur : `humidifier.<votre_entite>`
- vitesse ventilateur : `select.<votre_entite_fan_speed>`
- humidité actuelle : `sensor.<votre_entite_current_humidity>`

## Modes gérés

La tuile gère les modes suivants :

- `Clothes-Dry` → affichage `Intense`
- `Continuous` → affichage `Continuel`
- `Manual` → affichage `Manuel`

Les vitesses (`Low`, `Medium`, `High`) ne sont affichées que pour `Manual` et `Continuous`.

## Robustesse recommandée

Si certaines entités sont parfois indisponibles (`unknown`/`unavailable`), conservez les fallbacks déjà présents dans le YAML pour éviter un affichage cassé.
