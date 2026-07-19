# Contribuer à Nacrelume

## Avant toute contribution

Lire `AGENTS.md` puis `docs/00_START_HERE.md`. Les décisions déjà validées ne doivent pas être rediscutées ou remplacées sans demande explicite.

## Branches et pull requests

- Créer une branche courte et descriptive : `feature/...`, `docs/...`, `art/...` ou `prototype/...`.
- Une pull request correspond à un objectif principal.
- Expliquer ce qui change, pourquoi, comment cela a été vérifié et ce qui reste ouvert.
- Utiliser une pull request en brouillon tant qu’une décision visuelle ou technique n’est pas validée.

## Documentation

- Toute décision structurante est ajoutée à `docs/DECISION_LOG.md`.
- Toute nouvelle image est ajoutée à `docs/ASSET_CATALOG.md`.
- Toute modification du monde ou des raccords est reportée dans `docs/WORLD_AND_MAPS.md` ou dans un registre régional dédié.
- Ne pas supprimer l’historique d’une décision : marquer plutôt ce qui est remplacé et par quelle décision.

## Assets

- Conserver les sources lorsqu’elles existent.
- Éviter les fichiers temporaires, doublons et générations rejetées.
- Les images de `docs/images/` servent de références visuelles et ne sont pas automatiquement des assets de production.
- Ne pas recopier d’assets provenant d’un jeu existant.

## Validation minimale

- Vérifier tous les liens Markdown.
- Vérifier les dimensions et formats des images ajoutées.
- Pour une carte découpée, réassembler les chunks et comparer avec la carte maîtresse.
- Pour Tiled, vérifier collisions, occlusions, navigation, triggers et ordre des calques.

