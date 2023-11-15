# Scraper

Ce code Python est un script de scraping de base qui utilise les bibliothèques requests et BeautifulSoup pour extraire le texte des balises <p> d'une page web et le sauvegarder dans un fichier JSON. 
Voici une description détaillée de chaque partie du code :

Importation des bibliothèques :

requests: Permet d'envoyer des requêtes HTTP pour récupérer le contenu d'une page web.
BeautifulSoup: Une bibliothèque de parsing HTML qui facilite l'extraction d'informations à partir du code HTML.


Définition de la fonction scrape_and_save :

Prend en paramètres l'URL de la page à scraper (url) et le nom du fichier JSON de sortie (output_file).
Envoie une requête GET à l'URL spécifiée.
Si la requête réussit (statut 200), le contenu HTML de la page est analysé avec BeautifulSoup.
Le texte de toutes les balises <p> est extrait et stocké dans une liste appelée paragraphs.
Les données sont ensuite enregistrées dans un fichier JSON spécifié par output_file.


Variables d'URL et de fichier de sortie :

url_to_scrape: L'URL de la page web que vous souhaitez scraper, dans cet exemple, c'est la page d'accueil de 20 Minutes.
output_json_file: Le nom du fichier JSON dans lequel les données seront enregistrées.


Appel de la fonction scrape_and_save :

La fonction est appelée avec les paramètres correspondants à l'URL à scraper et au fichier de sortie.


L'objectif de ce script est d'extraire le texte des balises <p> de la page d'accueil de 20 Minutes et de le sauvegarder dans un fichier JSON. 
Le code est ajustable en fonction de vos besoins et de la structure HTML spécifique de la page que vous souhaitez scraper.
