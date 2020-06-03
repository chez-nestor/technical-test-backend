### Chez Nestor - Test technique Back

-----

Le but de l'exercice est de créer un module de réservation de chambre pour le backoffice de Chez Nestor : nous gérons un parc d'appartements dans lesquels se trouve plusieurs chambres. Lorsque nos clients se rendent sur le site https://www.chez-nestor.com/ pour réserver une chambre dans l'un de nos appartements, ils doivent remplir un certain nombre d'informations avant de pouvoir payer leurs frais de service, qui valident leur réservation.

Vous devrez exposer une API qui permettra à un client de réserver une chambre, ainsi que de récupérer toutes les données du client, de la chambre, de l'appartement et tout ce qui vous semblera utile à l'utilisation des données par une interface utilisateur.

Vous êtes libres de créer de nouveaux modèles ainsi que d'ajouter les champs qui vous sembleront pertinents dans les modèles suivants :

```

Apartment
- `id` : String, UUID unique ;
- `name` : String, nom de l'appartement ;
- `street` : String, rue de l'appartement ;
- `zipCode` : String, code postal ;
- `city` : String, ville ;

Room
- `id` : String, UUID unique ;
- `number` : Integer, numéro de la chambre ;
- `area` : Float, surface de la chambre ;
- `price` : Integer, prix de la chambre (en centimes) ;
- une référence vers l'appartement dans laquelle elle se situe

Client
- `id` : String, UUID unique ;
- `firstName` : String, prénom ;
- `lastName` : String, nom ;
- `email` : String, adresse email ;
- `phone` : String, numéro de téléphone ;
- `birthDate` : String, date de naissance ;
- `nationality` : String, nationalité ;

``` 

**Technologie** : le langage, le framework, la base de données et plus généralement les outils sont libres, utilisez ce que vous connaissez le mieux ! :)

Le sujet est volontairement extrêmement large. Le temps recommandé pour le traiter est de 5 heures, mais vous êtes libres de prendre plus ou moins de temps, nous vous demandons simplement de nous indiquer le temps que vous avez mis pour traiter le sujet par mail à dev[AT]chez-nestor.com ainsi qu'un lien vers un repository GitHub avec un README clair et détaillé dans lequel vous indiquerez les endpoints de votre API.

Enfin, pour la notation, voici quelques pistes de ce qui nous intéresse dans le rendu :

- ✨ Propreté de code : découpage, gestion d'erreurs, nommage des variables / fonctions, etc.
- 📚 Utilisation de librairies / frameworks
- ⚙️ Tests techniques
- 🏦 Architecture de l'API utilisée (REST par exemple)
- 📖 Base de données : définition des modèles, optimisation des requêtes
- 🔀 Maîtrise de git : messages de commit, nombre de commits, etc.
- ☁️ En bonus : déploiement sur un hébergeur (Heroku, AWS, ...)

Si vous pensez avoir fait quelque chose qui mérite notre attention, n'hésitez pas à nous le signaler ! :) 
