# Configuration

Deux fichiers sont disponibles selon votre équipement :

- `lovelace/dehumidifier_tile.yaml`
- `lovelace/climatiseur.yaml`

## Entités par défaut

### Déshumidificateur

- `humidifier.deshumidificateur`
- `select.deshumidificateur_fan_speed`
- `sensor.deshumidificateur_current_humidity`

### Climatiseur

- `climate.152832117217942_climate`

## Mapping recommandé

Si vos entités sont différentes, remplacez **toutes** les occurrences dans le YAML :

- déshumidificateur : `humidifier.<votre_entite>`
- vitesse ventilateur : `select.<votre_entite_fan_speed>`
- humidité actuelle : `sensor.<votre_entite_current_humidity>`
- climatiseur : `climate.<votre_entite>`

## Modes gérés

### Déshumidificateur

- `Clothes-Dry` → affichage `Intense`
- `Continuous` → affichage `Continuel`
- `Manual` → affichage `Manuel`

Les vitesses (`Low`, `Medium`, `High`) ne sont affichées que pour `Manual` et `Continuous`.

### Climatiseur

- `cool` (Froid)
- `fan_only` (Ventil)
- `dry` (Sec)
- `auto` (Auto)

## Robustesse recommandée

Si certaines entités sont parfois indisponibles (`unknown`/`unavailable`), conservez les fallbacks déjà présents dans les YAML pour éviter un affichage cassé.
