# VORTEX — Studio créatif

Portfolio statique en français et anglais, réalisé à partir de la référence fournie.

## Lancer le site

Aucune compilation ni installation de dépendances. Depuis ce dossier :

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Sous Windows, utilisez `py -m http.server 8000 --bind 127.0.0.1`. Ouvrez ensuite http://localhost:8000.

## GitHub Pages

Dans Settings → Pages, sélectionnez « Deploy from a branch », la branche `main` et le dossier `/ (root)`, puis enregistrez. Le fichier `.nojekyll` permet de servir directement les fichiers statiques.

## Fichiers

`index.html` : structure, navigation et contenu bilingue.
`style.css` : composition, responsive, typographie et effets.
`app.js` : traduction, projets, services, témoignages, brief local et animation réversible au scroll.
`assets/header-mavrik-higgsfield.png` : header séparé sans texte, reconstruit avec Imagegen depuis la référence, avec le nouveau personnage fictif Mavrik.
`assets/prompt-higgsfield-vortex.txt` : prompt vidéo et instructions d’intégration.
`assets/mavrik-about.png` : portrait de Mavrik dans la section À propos.
`assets/reference.jpg` : référence fournie, utilisée comme source pour les visuels de projets et les marques.

Le site se publie sans compilation. Les polices sont hébergées avec le site.

Sur mobile (largeur maximale de 760 px), la signature Mavrik et ses deux lignes de texte sont masquées. Tous les textes de présentation du header sont blancs, en français comme en anglais. Ces règles sont limitées à la mise en page mobile.

## Animation

Le header utilise désormais `assets/header-mavrik-scroll.mp4`, généré dans Higgsfield avec MiniMax Hailuo 2.3 Fast. La génération a été demandée en 1080p et a livré un fichier panoramique 2112 × 960, 24 images par seconde, de 5,875 secondes. Coût observé : 7 crédits du portefeuille Higgsfield connecté au plugin, distinct du solde de l’API en dollars.

Le header reste fixé à l’écran pendant une distance de défilement d’environ 90 % de la hauteur de la fenêtre. Descendre avance la vidéo ; remonter la fait revenir aux images précédentes ; arrêter le défilement fige l’image. Le reste du portfolio défile normalement ensuite.

Le fichier est réencodé avec des images clés tous les six frames et le démarrage rapide MP4 pour améliorer les déplacements dans la vidéo. La version PNG reste le visuel de secours. Le mode de réduction des animations désactive le maintien à l’écran et conserve l’image fixe.

Le mouvement de caméra du clip est volontairement discret ; il ne contient pas de transformation importante du décor. Aucune génération supplémentaire n’est déclenchée par le site.

## Personnalisation

Le nom, les coordonnées, chiffres, références et témoignages sont des contenus de démonstration repris ou adaptés de la maquette. Les fiches de projets sont des études créatives illustrées, sans vidéo finale associée. Les profils sociaux restent à renseigner. Le formulaire permet uniquement de copier ou télécharger un brief ; aucun e-mail n’est envoyé.

Les images de la maquette sont limitées par sa résolution de 736 × 1307 pixels. Le header est une reconstruction de 1860 × 845 pixels. Il ne s’agit pas d’une extraction identique au pixel près. Remplacer ces visuels par les originaux haute définition pour une version définitive.

## Vérifications

Syntaxe JavaScript, intégrité des ancres HTML, unicité des identifiants, références aux fichiers locaux et présence des traductions vérifiées. La comparaison visuelle dans un navigateur n’a pas été réalisée dans cet environnement.
