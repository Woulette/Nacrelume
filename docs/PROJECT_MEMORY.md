# Mémo officiel du projet — Quartier opalin

**Statut :** décisions validées avant la production des vraies cartes  
**Mise à jour :** 19 juillet 2026

## Vision du jeu

- Jeu en **2D isométrique / 2,5D trois-quarts haute**.
- Orientation **MMO / action-RPG avec combats en temps réel**, et non combats au tour par tour.
- Le monde doit sembler ouvert et fluide au joueur.
- Structure technique retenue : **grandes zones continues divisées en chunks chargés discrètement**.
- Les transitions visibles ne sont réservées qu’aux changements importants : autre région, bâtiment, grotte, donjon ou instance.
- Outil de construction recommandé : **Tiled**, avec assets réutilisables, collisions, navigation, occlusions et premiers plans séparés.

## Personnage officiel

- Garçon chibi en pixel art.
- Cheveux bruns hérissés, yeux ambrés.
- Tunique beige, bas et bottes bruns.
- Bâton en bois tenu dans la main gauche.
- Forme de base sans aura.
- Première évolution : lueur diffuse proche du corps, sans particules ; variantes retenues rouge, verte, blanche et rose.

## Direction artistique officielle

- Nom de travail : **Quartier opalin**.
- Référence maîtresse : `images/reference/quartier-opalin-reference-officielle.png`.
- Charte : `ART_DIRECTION.md`.
- Palette : `images/reference/quartier-opalin-palette-officielle.png`.
- Paramètres : `reference/quartier-opalin-style-tokens.json`.

### Principes non négociables

- Fantasy chaleureuse, ancienne, élégante, florale et réellement habitée.
- Vraies maisons avec murs, portes, fenêtres, toits, cheminées, balcons et détails domestiques.
- Pierre claire et enduit nacré, toits bleu-violet, eau cyan, fer forgé, glycines et végétation bleu-vert.
- Le cristal reste un accent minoritaire : lanternes, vitres, fleurs ou quelques tuiles.
- Le personnage brun/beige doit rester très lisible au milieu de la palette froide.
- Même caméra, même échelle et même direction de lumière sur toutes les cartes.

### Interdictions

- futurisme, science-fiction ou architecture abstraite ;
- bâtiments flottants, dômes de verre, lasers, anneaux ou barrières énergétiques ;
- maisons entièrement cristallines ;
- portails circulaires surdimensionnés ;
- reprise d’assets, interfaces ou silhouettes propres à Dofus ou à un autre jeu ;
- variation arbitraire de palette, d’échelle ou de caméra entre deux zones.

## Méthode retenue pour les grandes cartes

1. Concevoir une **carte maîtresse régionale** avant les cartes individuelles.
2. Définir les routes, rivières, reliefs, portes et points de raccord.
3. Découper la région en chunks de dimensions fixes.
4. Réutiliser une bibliothèque commune d’assets pour obtenir des raccords de production exacts.
5. Construire les couches Tiled : sol, eau, bâtiments, collisions, occlusions, premiers plans, navigation et spawns.
6. Tester le réassemblage et les déplacements avant d’étendre le monde.

## Prototype validé

- Prototype visuel d’une région **3 × 3 chunks** réalisé autour du Quartier opalin.
- Organisation : centre urbain, forêt/vestiges, sortie nord, vergers, canaux, faubourg, prairie humide, route/pont et champs.
- Une rivière cyan et plusieurs routes traversent logiquement les secteurs.
- Réassemblage des neuf chunks contrôlé avec **0 pixel de différence** par rapport à la carte maîtresse.
- Références : `images/maps/prototype-region-3x3.png` et `images/maps/prototype-region-3x3-grille.png`.
- Ce prototype valide la méthode et la cohérence macro, mais il n’est pas encore une carte jouable finale.

## Prochaine phase

Le projet entre maintenant dans la production des **vraies cartes**. Avant de fabriquer la première zone finale, il reste à fixer :

- moteur de jeu et format d’export ;
- taille des tuiles isométriques ;
- dimensions d’un chunk de production ;
- vitesse et directions de déplacement ;
- système de collisions et de navigation des monstres ;
- règles de poursuite, désengagement et changement de zone en combat ;
- première région réellement jouable à produire.

Ce mémo et la charte visuelle constituent la source de vérité du projet. Toute nouvelle carte doit les respecter, sauf décision explicite de modification validée ultérieurement.
