**TODO : Ajouter le sketch de l'arduino pour être sûr qu'il soit disponible.**
# Oscillateur à fréquence variable asservi par GPS de 1 à 112,5MHz
Ultra précis (0.1Hz avec le module GPS) cet oscillateur à signaux carrés programmable dispose de deux sorties d'horloge.

Ce projet propose un PCB compact, s'enfichant à l'arrière du LCD et supportant le l'oscillateur SI5351. **TODO : Le GPS est relié par des câbles ?**.

Ce PCB repose sur le [schéma créé par W3PM](http://www.knology.net/~gmarcus/Si5351/Si5351_VFO_QEX.pdf) (voir la [page de l'auteur](http://www.knology.net/~gmarcus/)).


# Réalisation

Après avoir fait réaliser le PCB, souder les composants dans cet ordre :

- les condensateurs et les résistances ;
- la diode Schottky ;
- le régulateur de tension en l'appliquant bien sur le PCB pour évacuer la chaleur efficacement ;
- les deux potentiomètres ;
- les connecteurs.

Éviter de souder l'arduino directement, utiliser plutôt des connecteurs.

# BOM

L'ensemble des composants coûte environ 30€ hors boitier et PCB.

| Référence | Quantité | Valeur | Source | Prix |
|----|-----|-----|-----|-----|
| C1, C2, C4, C5 | 4 | 0.1µF boitier CMS 0805 || 0,04€ |
| C3, C6 | 2 | 4.7µF boitier CMS 0805 || 0,02€ |
| J2, J3, J4, J9 | 4 | Connecteur dupont mâle vertical 1x2 broches pas 2,54 mm || 0,04€ |
| J1 | 1 | Connecteur dupont mâle vertical 1x3 broches pas 2,54 mm || - |
| J5 | 1 | Connecteur dupont femelle vertical 1x7 broches pas 2,54 mm || 1,00€ |
| J10 | 1 | Connecteur dupont femelle vertical 1x4 broches pas 2,54 mm || 1,00€ |
| J8 | 1 | Connecteur dupont femelle vertical 1x16 broches pas 2,54 mm || 1,00€ |
| D1 | 1 | Diode schottky boitier CMS SS24 || 0,0299€ |
| U1 | 1 | Régulateur linéaire L78M05 boitier CMS TO-252 || 0,189€|
| RV1, RV2 | 1 | potentiomètre 10k boitier CMS 3x3 || 0,216€ |
| A1 | 1 | Arduino nano v3.0|| 1,70€|
| LCD | 1 | Écran LCD 16x2 à controlleur HD44780 || 5,00€ |
| SI5351 | 1 | Module SI5351 à 7 broches || 6,00€ |
| GPS | 1 | Module GPS avec antenne || 15,00€ |
| Boutons poussoir | 3 ||| 1,50€ |
| Encodeur rotatif | 1 | Encodeur rotatif avec son bouton || 0,50€ |
| Coaxial | qsp | Câble coaxial RG316 || 0,50€|
| Boitier |||||

