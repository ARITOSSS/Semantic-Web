# Semantic-Web

## Comment nous avons procédé :
Pour ce projet nous avons utilisé Tarql pour convertir notre csv en format ttl. Il suffit d'installer l'archive sur le git : https://github.com/tarql/tarql.

Une fois cela fait, il suffit de l'unzip de placer son fichier csv, et la reqûete sparql permettant la transaction avant de faire appel à l'utilitaire avec la commande :

java -jar tarql-x.x.jar nom_du_fichier_requete.sparql nom_du_csv.csv > _nom_du_ttl_souhaité.ttl

## Conseil : 
Pour voir les préfixes que nous avons utilisé il suffit d'ouvrir le ttl pour voir la structure d'un enregistrement.

## Schema :
Voici une représentation graphique d'une transaction:
<img width="2759" height="838" alt="rdf-grapher" src="https://github.com/user-attachments/assets/f590a4c0-1833-4c33-9db2-ce6fdf4187e3" />

