# FAQ

## Pourquoi ne pas utiliser `stack-in-card` ?

Approche volontairement minimaliste en dépendances : `mushroom` + `card-mod` uniquement.

## Pourquoi ne pas utiliser de carte conditionnelle (`conditional card`) ?

La logique d'affichage est pilotée par les attributs d'entité via templates et `card-mod`, ce qui garde la structure de carte compacte.

## Pourquoi les vitesses ventilateur ne s'affichent pas toujours ?

C'est normal : les puces de vitesse ne sont visibles qu'en mode `Manual` ou `Continuous` sur la carte déshumidificateur.

## Le projet supporte-t-il aussi les climatiseurs ?

Oui, via `lovelace/climatiseur.yaml` (mode froid, ventilation, sec, auto, et contrôle de température).

## Que faire si mes noms d'entités sont différents ?

Remplacez toutes les entités par défaut dans le fichier YAML utilisé (`lovelace/dehumidifier_tile.yaml` ou `lovelace/climatiseur.yaml`).
