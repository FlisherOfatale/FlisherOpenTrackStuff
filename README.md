# FlisherOpenTrackStuff
FlisherOpenTrackStuff

Voici mon guide pour l'utilisation d'[OpenTrack](https://github.com/opentrack/opentrack/).
SVP, *NE PAS* brancher la webcam avant d'avoir suivi les étapes.  Si vous ne le faites-pas, vous devrez probablement diagnostiquer et réparer l'installation des pilotes...

## Étape optionelle depuis OpenTrack 2021.1.2
Télécharger la dernière version des pilotes open source de la PS3 Eye Cam: https://github.com/jkevin/PS3EyeDirectShow/releases/tag/1.0b2

Notez que la dernière version d'OpenTrack possède un pilote natif un peu plus performant que celui à part, mais est parfois plus difficile à installer.

Exécuter le fichier pour installer les pilotes

## Étape #1: Téléchargement d'OpenTrack
Télécharger la dernières version d'Opentrack disponible sur la page https://github.com/opentrack/opentrack/releases

Le lien direct pour la dernière version au momment d'écrire ces lignes: [OpenTrack 2021.1.2](https://github.com/opentrack/opentrack/releases/download/opentrack-2021.1.2/opentrack-2021.1.2-win32-setup.exe)

## Étape #2: Installer OpenTrack
Exécuter le fichier pour installer OpenTrack.

## Étape #3: Brancher la WebCam
Vous devrier voir que votre ordinateur détecte un nouveau périphériques après quelques secondes.

## Étape #4: Lancer Opentrack
Lancer Opentrack

## Étape #5: Configuration d'un KeyBind pour recentrer:
Cliquez sur le bouton "options", puis assigner une touche pour le keybinding "Center" en cliquant sur "Bind".  
Pour ma part, j'utilie la touche à gauche du "1" sur le clavier.

## Étape #6: Configuration du mode utilisé par OpenTrack

Lors du lancement initial, les options suivantes devraient normalement être sélectionnées
![MainMenu](/images/MainMenu_1.png)

## Étape #7: Configuration de la webcam

* Cliquez le petit Marteau a droite de PointTracker
* Sélectionnez "PS3 eye open driver" 
* Fermer le menu en appyant sur "OK: en bas
* Lancer le test en appuyant sur "Start", vous deviez voir une image noir floues ou nette.

La webcam de PS3 a 2 niveaux de focus configurable en tournant la lentille.  
Pour la grande majorité des gens, le mode en tournant dans le sens contraire des aiguilles d'une montre est le plus efficace.
Notez que les webcam fournie par Flisher après Avril 2021 ont génalement un filtre, sauf indication contraire, bloquant la lumière visible, résultant en une image noire par défaut.  Vous verrez cependant les points infrarouge de la clip.

Vous devrez possiblement ajuster le Gain et l'Exposure pour bien voir les points, un exemple basée sur votre clip et caméra est inclue lors de la livraison.

## Étape 7: Configuration du modèle de la clip
* Assurez-vous d'avoir des batterie rechargeable NiMh, 1.2v.
* Mettez la switch à On. (vous devriez voir vois 3 points)
* Démarrer le tracking en appuyant sur "Start"
* Cliquez le petit Marteau a droite de PointTracker
* Choisissez l'onglet "Model"
* Choisissez le sous-onglet "Clip"
* Configurer les valeurs suivantes si le long bras est vers le bas (ou le contraire si le long bras est vers le haut)
![Clip](images/PointTracker_Clip.png)
* Démarrez la calibration en cliquant sur "Start Calibration"
* Effectuez des mouvements de gauche à droite et de haut en pas quelques fois.  NE PAS pencher, déplacer votre tête ou faire de diagonale pendant cette calibration.
* Terminer la calibration en cliquand sur "Stop Calibration"


## Troubleshooting:
### Effet de Flares
![Flare](images/flares.png)

Si vous avez des flares, vous pouvez réduire le "gain" de la webcam en retournant dans "PointTrackers Settings, et cliquer "Open" dans les options de caméras.
Exemple:
![FlareFixed](images/flare-fixed.png)

* Selon votre environnement et distance de la webcam, le gain et l'exposure sont 2 options à ajuster.
* SVP ajuster la taille des pixel avec de la marge de manoeuvre.  Notez que les valeur de 2 a 12 sont généralement bonnes, le minimum pourrait être légèrement plus haut si vous avez des points qui aparaissent comme sur la photos des flares.

### Les axes semblent mélangés dans OpenTrack: 
Vous avez probablement mal configué les mesures, ou installé la clip à l'envers
