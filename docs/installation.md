# Installation

## Prérequis

- Home Assistant à jour.
- HACS installé et fonctionnel.
- Dashboard Lovelace avec support YAML.

## Étapes détaillées

1. **Installer les dépendances via HACS**
   - `Mushroom Cards`
   - `Card Mod` (incluant `mod-card`)
2. **Vider le cache navigateur** (recommandé) puis **redémarrer Home Assistant**.
3. Ouvrir le dashboard Lovelace cible, puis **modifier le tableau de bord**.
4. Ajouter une carte en mode YAML et coller le contenu de `lovelace/dehumidifier_tile.yaml`.
5. Sauvegarder.
6. Adapter les entités (humidifier/select/sensor) selon votre installation.

## Vérifications rapides

- L'icône ventilateur tourne quand le déshumidificateur est `on`.
- Les puces de mode changent de couleur selon le mode actif.
- Les vitesses de ventilation apparaissent en mode `Manual` et `Continuous`.

## En cas de problème

Consultez directement le guide de dépannage : `docs/troubleshooting.md`.
