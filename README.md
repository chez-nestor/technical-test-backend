### Chez Nestor - Test technique Back

-----

Le but de l'exercice est de créer un module de réservation de chambre pour le backoffice de Chez Nestor : nous gérons un parc d'appartements. Nos clients, pour réserver une chambre dans l'un de nos appartements, doivent remplir un certain nombre d'informations afin de valider leur réservation.

Vous devrez **exposer une API NodeJS** qui permettra à un **client** de **réserver une chambre**, ainsi que de **récupérer toutes les données du client, de la chambre, de l'appartement** et tout ce qui vous semblera utile à l'**utilisation des données par une interface utilisateur**. Pour chaque modèle, il faut qu'on puisse **créer**, **lire**, **modifier** et **supprimer** (CRUD) des données.

De plus, vous veillerez à respecter les règles suivantes :
- Un appartement contient au moins 1 chambre.
- Un client ne peut pas réserver plusieurs chambres en même temps.
- L'adresse email d'un client est unique.
- Lorsqu'une chambre a été réservée par un client, elle ne peut plus être réservée.
- Une chambre peut être réservée seulement si le client a rempli toutes ses informations.


Vous êtes libres de créer de nouveaux modèles ainsi que d'ajouter les champs qui vous sembleront pertinents dans les modèles suivants :

```

Apartment
- `id` : String, ID unique ;
- `name` : String, nom de l'appartement ;
- `street` : String, rue de l'appartement ;
- `zipCode` : String, code postal ;
- `city` : String, ville ;

Room
- `id` : String, ID unique ;
- `number` : Integer, numéro de la chambre ;
- `area` : Float, surface de la chambre ;
- `price` : Integer, prix de la chambre (en centimes) ;
- une référence vers l'appartement dans laquelle elle se situe

Client
- `id` : String, ID unique ;
- `firstName` : String, prénom ;
- `lastName` : String, nom ;
- `email` : String, adresse email ;
- `phone` : String, numéro de téléphone ;
- `birthDate` : String, date de naissance ;
- `nationality` : String, nationalité ;

``` 

**Technologies recommendées** : 

- NestJs
- Concernant la base de données et plus généralement les autres outils, vous pouvez utiliser ceux que vous connaissez le mieux

Le sujet est volontairement extrêmement large. Il n'y a pas de limite de temps pour le réaliser, vous êtes libre le temps que vous jugez nécessaire.
Nous vous demandons simplement de nous indiquer le temps que vous avez mis pour traiter le sujet ainsi qu'un lien vers un repository GitHub.

Enfin, pour la notation, voici quelques pistes de ce qui nous intéresse dans le rendu :

- ✨ Propreté de code : découpage, gestion d'erreurs, nommage des variables / fonctions, etc.
- 📚 Utilisation de librairies / frameworks
- ⚙️ Tests (unitaires, d'intégration, etc.)
- 🏦 Architecture de l'API utilisée (REST par exemple)
- 📖 Base de données : définition des modèles, optimisation des requêtes
- 🔀 Maîtrise de git : messages de commit, nombre de commits, etc.
- ☁️ En bonus : déploiement sur un hébergeur (Heroku, AWS, ...)

Si vous pensez avoir fait quelque chose qui mérite notre attention, n'hésitez pas à nous le signaler ! :) 
