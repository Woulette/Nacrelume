# Commencer ici

Ce document permet à un nouveau chat ou contributeur de reprendre Nacrelume sans connaître les conversations précédentes.

## État actuel

Le projet est en **préproduction**.

Validé :

- nom de travail : **Nacrelume** ;
- personnage de base et quatre couleurs de première évolution ;
- vue 2D isométrique / trois-quarts haute ;
- direction artistique **Quartier opalin** ;
- combats en temps réel ;
- monde ouvert par grandes zones et chunks invisibles ;
- Tiled comme outil recommandé pour les cartes ;
- méthode carte maîtresse → chunks → assets de production ;
- prototype régional 3 × 3 prouvant la cohérence macro et le raccord sans joint.

Non validé :

- moteur de jeu ;
- langage et framework ;
- architecture serveur et réseau ;
- taille des tuiles ;
- dimensions réelles d’un chunk ;
- système précis de déplacement, collisions et pathfinding ;
- formule de combat, statistiques et compétences ;
- première carte de production.

## Objectif immédiat

Choisir le socle technique minimal puis produire la **première vraie zone jouable**, en commençant par le Quartier opalin et ses quatre voisins directs.

La première zone doit permettre de tester :

- déplacement isométrique ;
- caméra et streaming de chunks ;
- collisions ;
- passage derrière bâtiments et arbres ;
- navigation d’un monstre ;
- poursuite et désengagement ;
- attaque en temps réel ;
- changement de chunk invisible.

## Ordre de lecture selon la tâche

| Tâche | Documents |
|---|---|
| Comprendre le projet | `PROJECT_MEMORY.md`, `GAME_DESIGN.md` |
| Générer ou dessiner | `ART_DIRECTION.md`, `CHARACTER.md`, `ASSET_CATALOG.md` |
| Créer une carte | `WORLD_AND_MAPS.md`, `TECHNICAL_DECISIONS.md` |
| Décider du moteur | `GAME_DESIGN.md`, `TECHNICAL_DECISIONS.md` |
| Reprendre avec une IA | `AI_HANDOFF.md`, `AGENTS.md` |

## Règle principale

Ne jamais confondre une belle image conceptuelle avec une carte jouable. La production exige des assets séparés, des calques, des collisions, des occlusions et des données de navigation.
