# Catalogue des références et assets

## Statuts

- **Officiel** : source de vérité validée.
- **Prototype** : sert à tester une idée ou une méthode.
- **Production** : prêt à être intégré au jeu.
- **Rejeté** : ne doit pas servir de référence.

## Références officielles

| Fichier | Statut | Usage | Ne pas faire |
|---|---|---|---|
| `images/reference/personnage-base.jpeg` | Officiel | identité du héros | redessiner librement le visage ou la tenue |
| `images/reference/premiere-evolution-4-couleurs.png` | Officiel concept | couleurs et forme de la lueur | utiliser comme spritesheet de production |
| `images/reference/quartier-opalin-reference-officielle.png` | Officiel | architecture, palette, densité, caméra | découper directement comme tileset final |
| `images/reference/quartier-opalin-palette-officielle.png` | Officiel | couleurs d’ancrage | transformer toute l’image en bleu/violet uniforme |
| `reference/quartier-opalin-style-tokens.json` | Officiel | paramètres lisibles par outils/IA | modifier sans mettre à jour la charte |

## Prototypes de cartes

| Fichier | Statut | Usage |
|---|---|---|
| `images/maps/prototype-region-3x3.png` | Prototype | cohérence régionale et circulation |
| `images/maps/prototype-region-3x3-grille.png` | Prototype | coordonnées et découpage des chunks |

## Assets de production

Aucun asset n’est encore classé **Production**.

La future bibliothèque devra contenir au minimum :

- tiles de sol et transitions ;
- eau et rives animables ;
- routes et pavés ;
- murs et clôtures ;
- maison modulaire avec base, murs, toit et occlusion séparés ;
- arbres avec tronc et canopée séparés ;
- ponts et escaliers ;
- mobilier ;
- sprites du personnage ;
- sprites des monstres et effets de combat.

## Règle d’ajout

Pour chaque nouveau fichier, renseigner : nom, chemin, statut, propriétaire, origine, dimensions, palette, usage prévu et décision de validation.

