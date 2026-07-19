# Instructions obligatoires pour les agents IA

Ce fichier s’applique à l’ensemble du dépôt **Nacrelume**.

## 1. Lecture obligatoire avant de travailler

Toujours lire, dans cet ordre :

1. `docs/00_START_HERE.md`
2. `docs/PROJECT_MEMORY.md`
3. le document métier correspondant à la tâche ;
4. `docs/DECISION_LOG.md`
5. `docs/ASSET_CATALOG.md` si des images ou assets sont concernés.

Ne jamais supposer que le contexte d’un chat précédent est disponible. Les fichiers du dépôt sont la mémoire officielle.

## 2. Identité du projet à ne pas perdre

- Nacrelume est un MMO / action-RPG en **2D isométrique trois-quarts haute**.
- Les combats sont **en temps réel**, jamais au tour par tour.
- Le monde paraît ouvert mais est techniquement composé de **grandes zones chargées par chunks**.
- **Tiled est recommandé mais pas encore imposé.** Quel que soit l’éditeur retenu, les cartes finales doivent séparer assets, collisions, occlusions et données de gameplay.
- La direction artistique officielle s’appelle **Quartier opalin**.
- Le cristal est un accent minoritaire ; le monde n’est ni futuriste ni entièrement cristallin.
- L’inspiration isométrique générale n’autorise jamais à copier Dofus ou un autre jeu.

## 3. Règles visuelles obligatoires

Avant toute génération ou création de décor, ouvrir :

- `docs/images/reference/quartier-opalin-reference-officielle.png`
- `docs/images/reference/quartier-opalin-palette-officielle.png`
- `docs/ART_DIRECTION.md`
- `docs/reference/quartier-opalin-style-tokens.json`

Maintenir : caméra, échelle, lumière haut-gauche, palette nacrée/bleu-violet/cyan, maisons crédibles et végétation florale.

Interdictions : futurisme, structures flottantes, dômes de verre, lasers, anneaux énergétiques, maisons entièrement en cristal, portails circulaires surdimensionnés, dérive de saturation, copie d’assets ou de silhouettes reconnaissables d’un autre jeu.

## 4. Règles concernant le personnage

Toujours consulter `docs/CHARACTER.md` et les images officielles avant de créer un sprite.

- Forme de base : aucune aura.
- Première évolution : lueur diffuse proche du corps, sans particules.
- Couleurs validées : rouge, vert, blanc et rose.
- Ne pas modifier silencieusement le visage, les cheveux, les vêtements ou la main portant le bâton.

## 5. Règles concernant les cartes

- Ne jamais générer une carte voisine indépendamment sans registre de raccord.
- Concevoir d’abord une carte maîtresse régionale.
- Documenter routes, rivières, reliefs, sorties, ponts et largeur des passages.
- Produire les chunks depuis une même source ou une même bibliothèque d’assets.
- Prévoir au minimum les couches : sol, eau, sous-décor, bâtiments, collisions, occlusion, premier plan, entités, triggers et navigation.
- Une différence visuelle nulle entre crops ne rend pas la carte jouable : collisions et occlusions restent obligatoires.
- Conserver des espaces dégagés pour le déplacement et le combat en temps réel.

## 6. Règles de conception technique

- Ne pas inventer le moteur, le langage, la taille des tuiles ou l’architecture réseau : ils ne sont pas encore validés.
- Présenter les choix structurants avec leurs conséquences avant de les verrouiller.
- Inscrire chaque décision validée dans `docs/DECISION_LOG.md`.
- Mettre à jour `docs/TECHNICAL_DECISIONS.md` lorsqu’une question ouverte est résolue.
- Préférer des fichiers et formats standards, versionnables et reproductibles.

## 7. Règles de contribution

- Travailler sur une branche dédiée.
- Limiter chaque pull request à un objectif cohérent.
- Ne jamais écraser un asset officiel sans décision explicite.
- Ajouter toute nouvelle référence à `docs/ASSET_CATALOG.md`.
- Mettre à jour la documentation dans la même pull request que le changement correspondant.
- Signaler clairement les hypothèses, prototypes et éléments non prêts pour la production.

## 8. Critères de fin de tâche

Avant de déclarer une tâche terminée, vérifier :

- conformité aux documents officiels ;
- absence de dérive artistique ou de décision technique implicite ;
- liens Markdown et chemins d’assets valides ;
- mise à jour du journal de décisions si nécessaire ;
- distinction claire entre concept, prototype et asset de production ;
- résumé de ce qui a changé et de la prochaine action recommandée.
