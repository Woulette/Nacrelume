# Décisions techniques

## Décisions validées

| Sujet | Décision | Conséquence |
|---|---|---|
| Projection | 2D isométrique / trois-quarts haute | caméra, collisions et assets doivent partager la même géométrie |
| Combat | Temps réel | zones assez grandes, navigation dynamique et frontières invisibles |
| Monde | Grandes zones découpées en chunks | streaming, registre de raccords et persistance par zone |
| Éditeur de cartes | Tiled recommandé | export TMJ/JSON ou format choisi par le moteur |
| Décors hauts | Calques et occlusions séparés | maisons et arbres ne peuvent pas rester dans un fond aplati unique |
| Production visuelle | Assets réutilisables | les concepts générés servent de référence, pas de tileset final automatique |

## Décisions ouvertes

| Sujet | État | À comparer |
|---|---|---|
| Moteur | À décider | Godot, Phaser ou autre solution adaptée au déploiement visé |
| Plateforme | À décider | PC, navigateur, mobile ou combinaison |
| Taille de tuile | À décider | lisibilité, précision des collisions, coût mémoire |
| Dimensions de chunk | À décider | portée de vue, streaming, combat et nombre d’entités |
| Réseau | À décider | autorité serveur, prédiction, interpolation, persistance |
| Backend | À décider | comptes, monde, inventaires, combats et base de données |
| Contrôles | À décider | clavier/souris, clic pour se déplacer, manette, tactile |
| Pathfinding | À décider | grille isométrique, graphe de navigation ou navigation hybride |
| Format des sprites | À décider | dimensions, directions, frames et atlas |

## Règle de décision

Une option technique n’est considérée comme validée que lorsque :

1. les objectifs et plateformes sont explicités ;
2. au moins deux solutions sont comparées ;
3. un petit prototype réduit le risque principal ;
4. la décision est ajoutée à `DECISION_LOG.md` ;
5. ce tableau est mis à jour.

## Risques déjà identifiés

- produire des cartes entières comme images aplaties empêche l’occlusion propre ;
- générer chaque carte indépendamment crée des raccords incohérents ;
- choisir une taille de chunk avant la caméra et le combat peut entraîner une refonte ;
- viser immédiatement un MMO massif sans prototype réseau augmente fortement le risque ;
- versionner trop d’images lourdes sans stratégie d’assets peut faire grossir le dépôt.

