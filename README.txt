## Projet d'application météo

1. DESCRIPTION

Application meteo avec interface graphique, qui affiche la meteo du jour
et les previsions sur 7 jours pour une ville francaise. Les donnees
viennent de l'API gratuite Open-Meteo (open-meteo.com), qui ne demande
pas de cle.

L'application comprend deux ecrans :
- Ecran d'accueil : nom de la ville, icone de la meteo actuelle,
  temperature actuelle, temperatures minimale et maximale du jour.
- Ecran des previsions : graphique des temperatures minimales et
  maximales sur 7 jours, avec un bouton de retour a l'accueil.


2. PREREQUIS

- Python (developpe avec Python 3.14)
- Une connexion internet (pour interroger l'API)
- Les bibliotheques : pillow, matplotlib, requests
- Les supports decours


3. INSTALLATION

Dans un terminal, depuis le dossier du projet :

    pip install pillow matplotlib requests


4. LANCEMENT

Dans le dossier du projet (les chemins vers assets/ sont
relatifs) :

    python main.py


5. STRUCTURE DU PROJET

main.py             Programme principal : cree la fenetre et le canvas
menu.py             Ecrans (accueil, previsions) et fond d'ecran
plot.py             Creation du graphique Matplotlib
weather.py          Conversion du code meteo en nom d'icone
weather_queries.py  Requetes a l'API Open-Meteo
constants.py        Constantes : villes et coordonnees, taille, URL de l'API
assets/             Images : fonds d'ecran (blue_sky, night_sky) et icones