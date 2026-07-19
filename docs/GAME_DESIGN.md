# Game design — Nacrelume

## Promesse du jeu

Nacrelume est un MMO / action-RPG en 2D isométrique où le joueur explore un monde de fantasy opaline, affronte des monstres en temps réel et développe son personnage au sein de grandes régions continues.

Le projet ne cherche pas à reproduire Dofus. La vue isométrique et le genre fantasy sont des codes généraux ; le rythme, le combat, la structure du monde et la direction artistique doivent former une identité propre.

## Piliers validés

### 1. Combat en temps réel

- Les attaques, déplacements, esquives et compétences se déroulent sans passage en tour par tour.
- Le joueur et les monstres partagent l’espace d’exploration.
- Les zones doivent laisser assez de place pour lire les menaces, se déplacer et combattre.
- Les limites techniques de chunks ne doivent jamais être utilisées comme échappatoire visible.

### 2. Monde ouvert par grandes zones

- Le joueur perçoit une région continue.
- Le moteur charge et décharge des chunks autour du joueur.
- Les transitions visibles sont réservées aux régions lointaines, bâtiments, grottes, donjons et instances.
- Les monstres peuvent poursuivre le joueur dans toute une zone logique.

### 3. Lisibilité isométrique

- Silhouettes claires et contrastes fonctionnels.
- Chemins praticables moins détaillés que les bordures.
- Décors hauts gérés avec occlusion, transparence ou masquage.
- Le personnage reste lisible grâce à sa palette chaude sur le décor froid.

### 4. Progression et transformations

- Le personnage possède une forme de base et des évolutions visuelles.
- La première évolution reste simple : changement de couleur et lueur diffuse, sans surcharge d’effets.
- Les transformations futures devront traduire une progression sans copier les codes visuels d’une licence existante.

## Boucle de jeu provisoire

Cette boucle est une hypothèse de travail, pas encore un système verrouillé :

1. explorer une région ;
2. rencontrer des monstres ou événements ;
3. combattre en temps réel ;
4. récupérer ressources, expérience ou objets ;
5. améliorer le personnage et ses capacités ;
6. accéder à de nouvelles zones, quêtes ou instances.

## Règles de frontière en combat

La solution recommandée est d’éviter les frontières visibles à l’intérieur d’une grande zone. Entre deux zones réellement distinctes, l’une de ces règles devra être choisie :

- désengagement avant transfert ;
- zone de transition sans apparition de monstres ;
- poursuite limitée par un système de leash cohérent ;
- transfert serveur de l’entité, option plus complexe réservée à une architecture MMO avancée.

## Ce qui n’est pas encore décidé

- contrôle clavier, souris, manette ou tactile ;
- nombre de directions de déplacement et d’animation ;
- ciblage libre, verrouillage de cible ou système hybride ;
- collision des projectiles ;
- statistiques, classes, compétences et ressources ;
- mort, réapparition et pénalités ;
- PvP ;
- économie, artisanat et échanges ;
- persistance et capacité multijoueur visée.

Toute proposition sur ces sujets doit être présentée comme une option, jamais comme une décision acquise.

