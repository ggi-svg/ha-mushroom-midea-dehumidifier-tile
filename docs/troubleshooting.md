# Dépannage

## Les vitesses ventilateur n'apparaissent pas

1. Vérifiez le mode actif dans Outils de développement (`state_attr(<humidifier>, 'mode')`).
2. Les vitesses sont visibles uniquement en `Manual` ou `Continuous`.
3. Vérifiez que l'entité `select.*_fan_speed` existe et expose `Low/Medium/High`.

## L'animation de l'icône ne fonctionne pas

1. Vérifiez que `card-mod` est bien installé et chargé comme ressource.
2. Confirmez que l'entité humidifier est à l'état `on`.
3. Videz le cache navigateur puis rechargez l'interface.

## Les textes affichent `unknown` ou `unavailable`

1. Vérifiez l'état des entités dans Outils de développement.
2. Confirmez les IDs d'entités dans le YAML.
3. Redémarrez Home Assistant après changement d'intégration.


## La carte climatiseur ne répond pas

1. Vérifiez que l'entité `climate.*` existe et accepte les modes (`cool`, `fan_only`, `dry`, `auto`).
2. Remplacez `climate.152832117217942_climate` par votre propre entité dans `lovelace/climatiseur.yaml`.
3. Vérifiez dans Outils de développement que les services `climate.set_hvac_mode` et `climate.set_temperature` sont bien disponibles pour l'appareil.
