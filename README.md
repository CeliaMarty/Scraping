## HappyHourProject
Description
Le projet HappyHourProject vise à collecter, analyser et présenter les informations sur les happy hours des bars à Toulouse. Il comprend des étapes de webscraping, d'analyse de données, de visualisation, et d'envoi d'informations via e-mail.

## Étapes du Projet
Partie 1 : Extraction des Données
Scraping des informations nécessaires à partir du site Schlouk Map :
URL: Schlouk Map - Toulouse Happy Hour
Données collectées :
Nom du bar
Heures d'ouverture
URL de la page spécifique du bar
Services disponibles (uniquement les services "oui")
Prix des boissons pendant et hors happy hour
Stockage des données :
Les données extraites sont stockées dans un DataFrame pandas et sauvegardées dans data/raw_data.csv.
Partie 2 : Analyse des Données
Analyse des prix des différents bars :
Identifier les cinq bars proposant les meilleurs deals durant les happy hours.
Les résultats de cette analyse sont stockés dans data/processed_data.csv.
Partie 3 : Rapport par E-mail
Configuration de l'envoi d'e-mails :
Suivre le tutoriel de Mailtrap : Mailtrap Blog - Python Send Email
Utiliser smtplib et email.mime pour configurer l'envoi d'e-mails.
Préparation d'un e-mail au format HTML :
Inclure le top 5 des meilleurs deals en happy hour à Toulouse, basé sur l'analyse effectuée.
Utiliser le template HTML templates/html/report_template.html.
Partie 4 : Cartographie (Bonus)
Création d'une carte interactive avec Leaflet :
Récupérer les données de localisation de chaque bar pour afficher leur position sur la carte.
Marquer chaque bar avec des détails comme le nom, les horaires d'happy hour, et les prix.
