# Documentation.
C'est une API pour application ILORIA.


## Artisan
Récupération, l'ajoute, connexion, déconnection et modification tous les artisans dan la base de donnée.
### récupération tous les artisans
Il faut appelée URL avec méthode **GET** sans paramètre
``` url
https://vps356969.ovh.net/api/artisan
METHOD : GET
``` 
#### Retour de server
``` json
{
   "current_page": 1,
   "data": [
       {
           "id": 1,
           "email": "zahir-1@gmail.com",
           "prenom": "zahir-1",
           "nom": "mokrani-1",
           "photo": "user.png",
           "categorie": "cat-4",
           "images": "",
           "created_at": "2023-05-19T21:29:24.000000Z",
           "updated_at": "2023-05-19T21:29:24.000000Z"
        },
       {
           "id": 2,
           "email": "zahir-2@gmail.com",
           "prenom": "zahir-2",
           "nom": "mokrani-2",
           "photo": "user.png",
           "categorie": "cat-4",
           "images": "",
           "created_at": "2023-05-19T21:29:42.000000Z",
           "updated_at": "2023-05-19T21:29:42.000000Z"
        
        },
       {
        
           "id": 3,
           "email": "zahir-3@gmail.com",
           "prenom": "zahir-3",
           "nom": "mokrani-3",
           "photo": "user.png",
           "categorie": "cat-4",
           "images": "",
           "created_at": "2023-05-19T21:29:52.000000Z",
           "updated_at": "2023-05-19T21:29:52.000000Z"
        },
       {
           "id": 4,
           "email": "zahir-4@gmail.com",
           "prenom": "zahir-4",
           "nom": "mokrani-4",
           "photo": "user.png",
           "categorie": "cat-4",
           "images": "",
           "created_at": "2023-05-19T21:30:00.000000Z",
           "updated_at": "2023-05-19T21:30:00.000000Z"
        },
       {
           "id": 5,
           "email": "zahir-5@gmail.com",
           "prenom": "zahir-5",
           "nom": "mokrani-5",
           "photo": "user.png",
           "categorie": "cat-5",
           "images": "",
           "created_at": "2023-05-19T21:30:09.000000Z",
           "updated_at": "2023-05-19T21:30:09.000000Z"
        },
       {
           "id": 6,
           "email": "zahir-6@gmail.com",
           "prenom": "zahir-6",
           "nom": "mokrani-6",
           "photo": "user.png",
           "categorie": "cat-6",
           "images": "",
           "created_at": "2023-05-19T21:30:17.000000Z",
           "updated_at": "2023-05-19T21:30:17.000000Z"
        }
    ],
   "first_page_url": ["https://vps356969.ovh.net/api/artisan?page=1"](https://vps356969.ovh.net/api/artisan?page=1),
   "from": 1,
   "last_page": 1,
   "last_page_url": ["https://vps356969.ovh.net/api/artisan?page=1"](https://vps356969.ovh.net/api/artisan?page=1),
   "links": [
    
       {
        
           "url": null,
           "label": "&laquo; Previous",
           "active": false
        
        },
       {
        
           "url": ["https://vps356969.ovh.net/api/artisan?page=1"](https://vps356969.ovh.net/api/artisan?page=1),
           "label": "1",
           "active": true
        
        },
       {
        
           "url": null,
           "label": "Next &raquo;",
           "active": false
        
        }
    
    ],
   "next_page_url": null,
   "path": ["https://vps356969.ovh.net/api/artisan"](https://vps356969.ovh.net/api/artisan),
   "per_page": 50,
   "prev_page_url": null,
   "to": 6,
   "total": 6

}
```
``` head
code request server : 200
```
### Un artisans spécifique
{variable} : c'est une variable
Il faut appelée URL avec méthode **GET** avec paramètre **id_artisan**
``` url
https://vps356969.ovh.net/api/artisan/{id_artisan}
METHODE : GET
``` 
#### Retour server
Exemple artisan existe pour cette requête " **id_arisan** : 1 " : 
``` url
https://vps356969.ovh.net/api/artisan/1
```
``` json
{

   "id": 1,
   "email": "zahir-1@gmail.com",
   "prenom": "zahir-1",
   "nom": "mokrani-1",
   "photo": "user.png",
   "categorie": "cat-4",
   "images": "",
   "created_at": "2023-05-19T21:29:24.000000Z",
   "updated_at": "2023-05-19T21:29:24.000000Z"

}
```

``` head
code request server : 200
```
### List des artisans un type catégorie

{variable} : c'est une variable
Il faut appelée URL avec méthode **GET** avec paramètre **catégorie**
``` url
https://vps356969.ovh.net/api/artisan/{categorie}
METHODE : GET
```
#### Retour de server
Exmple  " **categorie** : cat-4 ":

``` url
https://vps356969.ovh.net/api/artisan/cat-4
```
``` json
[

   {
    
       "id": 1,
       "email": "zahir-1@gmail.com",
       "prenom": "zahir-1",
       "nom": "mokrani-1",
       "photo": "user.png",
       "categorie": "cat-4",
       "images": "",
       "created_at": "2023-05-19T21:29:24.000000Z",
       "updated_at": "2023-05-19T21:29:24.000000Z"
    
    },
   {
    
       "id": 2,
       "email": "zahir-2@gmail.com",
       "prenom": "zahir-2",
       "nom": "mokrani-2",
       "photo": "user.png",
       "categorie": "cat-4",
       "images": "",
       "created_at": "2023-05-19T21:29:42.000000Z",
       "updated_at": "2023-05-19T21:29:42.000000Z"
    
    },
   {
    
       "id": 3,
       "email": "zahir-3@gmail.com",
       "prenom": "zahir-3",
       "nom": "mokrani-3",
       "photo": "user.png",
       "categorie": "cat-4",
       "images": "",
       "created_at": "2023-05-19T21:29:52.000000Z",
       "updated_at": "2023-05-19T21:29:52.000000Z"
    
    },
   {
    
       "id": 4,
       "email": "zahir-4@gmail.com",
       "prenom": "zahir-4",
       "nom": "mokrani-4",
       "photo": "user.png",
       "categorie": "cat-4",
       "images": "",
       "created_at": "2023-05-19T21:30:00.000000Z",
       "updated_at": "2023-05-19T21:30:00.000000Z"
    
    }

]
```
```
code request server : 200
```
### Ajouter un artisan
Il faut appelée URL avec méthode **POST** avec paramètres
```URL
https://vps356969.ovh.net/api/artisan/post
METHODE : POST
```

|Parametres      | Description |
| ----------- | ----------- |
| prenom      | Prenom de l'artisan       |
| nom   | Nom de l'artisan        |
| email   | Email artisan        |
| password   | mote de pass de l'artisan        |
| categorie   | Type de l'arisan        |


C'est paramètre en haut c'est obligatoire.
**En future il faut ajouté anti-robots (captcha)**
*car cette application est prive mai pas public donc n'a pas obligé d'ajouter la security anti-robot*

|Parametres      | Description | defaut value|
| ----------- | ----------- |	- |
| photo      | La photo de profil de l'artisan       |user.png|
| images   | Les images de l'artisan        |empty|


C'est paramètre en haut c'est facultative .

#### Retour de server
Une erreur sur les parametre : 
```json
{
	"prenom":  [
		"The prenom field is required."
	],
	"nom":  [
		"The nom field is required."
	],
	"email":  [
		"The email field is required."
	],
	"password":  [
		"The password field is required."
	],
	"categorie":  [
		"The categorie field is required."
	]
}
```

``` code
code request server : 500
```

L'artisan est bien ajouté a la base de donnée : 
```json
{

   "id": 1,
   "email": "zahir-1@gmail.com",
   "prenom": "zahir-1",
   "nom": "mokrani-1",
   "photo": "user.png",
   "categorie": "cat-4",
   "images": "",
   "created_at": "2023-05-19T21:29:24.000000Z",
   "updated_at": "2023-05-19T21:29:24.000000Z"

}
```
``` code
code request server : 201
```
### Connexion d'artisan
Il faut appelée URL avec méthode **POST**.

```url
https://vps356969.ovh.net/api/artisan/login
METHOD : POST
```
avec paramètres **Obligatoir** : 
|Parametres      | Description |
| ----------- | ----------- |
| email     | Email de l'artisan
| password| mote de passe de l'artisan

#### Retour de serveur
Une erreur sur les parametre : 
```json
{
	"email":  [
		"The email field is required."
	],
	"password":  [
		"The password field is required."
	]
}
```
```code
code request server : 500
```
erreur de connecté :

```json
{
	"message":  "Email ou mot de passe incorrect"
}
```
```code
code request server : 500
```

L'artisan est bien connecté : 
remarque ce token c'est un sécurité il faut sauvegarde dan le téléphone utilisateur(artisan/client)
```json
{
	"token":  "3|rjMH1ldgAZjC6yuiRqkSyaVaTJB2taE7iv7SN4VE"
}
```
```code
code request server : 200
```

### Desconnexion artisan
Il faut appelée URL avec méthode **POST**.

```url
https://vps356969.ovh.net/api/client/logout
METHOD : POST
```
avec paramètres **Obligatoir** : 
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur |

#### Retour de serveur

Erreur de authentification (Vous avez oublié d'envoyé le token): 
 ```json
 {
	"message":  "Unauthenticated"
}
 ```
 ```code
code request server : 401
```

Le client est bien déconnecte : 
 ```json
 {
	"message":  "Vous etes bien deconnecte"
}
 ```
 ```code
code request server : 201
```

### Modifié des donnée d'un artisan
Pour la modification d'artisan il faut une sécurité *authentification*.

J'ai  apte  pour  la  solution  la  plus  simple  possible  et  c'est  un  tocken.  en  grand  que  l'utilisateur  (artisan/client)  connect  avec  succès  en  va  génère  un  tocken  et  le stock  sur  base  de  donnée  et  return  ce  tocken.  apre  il  faut  stock  ce  token  dont  le  téléphone  et  la  récupérer  chacun  fois  qu'en  appel  à  api  protège  par  sécurité  authentification

Il faut appelée URL avec méthode **PUT** avec paramètres

```url
https://vps356969.ovh.net/api/artisan/update
METHOD : PUT
```
Paramètres **Obligatoir**.

|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur

Paramètres **facultative** mai il faut ou mois un paramètre.

|Parametres      | Description |
| ----------- | ----------- |
| prenom      | Prenom de l'artisan       |
| nom   | Nom de l'artisan        |
| email   | Email artisan        |
| password   | mote de pass de l'artisan        |
| categorie   | Type de l'arisan        |

#### Retour de server
Erreur de authentification (Vous avez oublié d'envoyé le token): 
 ```json
 {
	"message":  "Unauthenticated"
}
 ```
 ```code
code request server : 401
```
 La modification est bien fait : 
  ```json
{
   "id": 1,
   "email": "zahir-1@gmail.com",
   "prenom": "zahir-1",
   "nom": "mokrani-1",
   "photo": "user.png",
   "categorie": "cat-4",
   "images": "",
   "created_at": "2023-05-19T21:29:24.000000Z",
   "updated_at": "2023-05-19T21:29:24.000000Z"
}
 ```
 ```code
code request server : 201
```

### Supprimer un artisan.
Il faut appelée URL avec méthode **DELETE** avec paramètres
```URL
https://vps356969.ovh.net/api/artisan/delete
METHOD : DELETE
```

#### retour de serveur
Erreur de token : 
```json
{
	"message":  "Unauthenticated"
}
```
``` code
code request server : 500
```
Le artisan est bien supprimer de la base de donnée 
```json
{
	"id":  "1",
	"message": "Artisan est bien supprimer"
}
```
``` code
code request server : 201
```

## Client

Récupération, l'ajoute, connexion, déconnection et modification tous les client dan la base de donnée.

### récupération tous les client
Il faut appelée URL avec méthode **GET** sans paramètre
``` url
https://vps356969.ovh.net/api/client
METHOD : GET
``` 
#### Retour de server
``` json
  
{
   "current_page": 1,
   "data": [  
       {
           "id": 1,
           "email": "mouhoub-1@gmail.com",
           "prenom": "mouhoub-1",
           "nom": "mardas-1",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:23.000000Z",
           "updated_at": "2023-05-19T21:37:23.000000Z"
        },
       {
           "id": 2,
           "email": "mouhoub-2@gmail.com",
           "prenom": "mouhoub-2",
           "nom": "mardas-2",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:31.000000Z",
           "updated_at": "2023-05-19T21:37:31.000000Z"
        },
       {
           "id": 3,
           "email": "mouhoub-3@gmail.com",
           "prenom": "mouhoub-3",
           "nom": "mardas-3",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:37.000000Z",
           "updated_at": "2023-05-19T21:37:37.000000Z"
        },
       {
           "id": 4,
           "email": "mouhoub-4@gmail.com",
           "prenom": "mouhoub-4",
           "nom": "mardas-4",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:44.000000Z",
           "updated_at": "2023-05-19T21:37:44.000000Z"
        },
       {
           "id": 5,
           "email": "mouhoub-5@gmail.com",
           "prenom": "mouhoub-5",
           "nom": "mardas-5",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:51.000000Z",
           "updated_at": "2023-05-19T21:37:51.000000Z"
        },
       {
           "id": 6,
           "email": "mouhoub-6@gmail.com",
           "prenom": "mouhoub-6",
           "nom": "mardas-6",
           "photo": "user.png",
           "created_at": "2023-05-19T21:37:58.000000Z",
           "updated_at": "2023-05-19T21:37:58.000000Z"
        }
    ],
   "first_page_url": ["https://vps356969.ovh.net/api/client?page=1"](https://vps356969.ovh.net/api/client?page=1),
   "from": 1,
   "last_page": 1,
   "last_page_url": ["https://vps356969.ovh.net/api/client?page=1"](https://vps356969.ovh.net/api/client?page=1),
   "links": [
       {
           "url": null,
           "label": "&laquo; Previous",
           "active": false
        },
       {
           "url": ["https://vps356969.ovh.net/api/client?page=1"](https://vps356969.ovh.net/api/client?page=1),
           "label": "1",
           "active": true
        },
       {
           "url": null,
           "label": "Next &raquo;",
           "active": false
        }
    ],
   "next_page_url": null,
   "path": ["https://vps356969.ovh.net/api/client"](https://vps356969.ovh.net/api/client),
   "per_page": 50,
   "prev_page_url": null,
   "to": 6,
   "total": 6
}
```
``` head
code request server : 200
```
### Récupère un client spécifique
{variable} : c'est une variable
Il faut appelée URL avec méthode **GET** avec paramètre **id_artisan**
``` url
https://vps356969.ovh.net/api/client/{id_client}
METHODE : GET
``` 
#### Retour server
Exemple artisan existe pour cette requête " **id_client** : 1 " : 
``` url
https://vps356969.ovh.net/api/client/1
```
``` json
{
	"id": 1,
	"email": "mouhoub-1@gmail.com",
	"prenom": "mouhoub-1",
	"nom": "mardas-1",
	"photo": "user.png",
	"created_at": "2023-05-19T21:37:23.000000Z",
	"updated_at": "2023-05-19T21:37:23.000000Z"
}
```
``` head
code request server : 200
```

### Ajouter un client
Il faut appelée URL avec méthode **POST** avec paramètres
```URL
https://vps356969.ovh.net/api/client/post
METHODE : POST
```

|Parametres      | Description |
| ----------- | ----------- |
| prenom      | Prenom de client       |
| nom   | Nom de client        |
| email   | Email client        |
| password   | mote de pass de client |

C'est paramètre en haut c'est obligatoire.
**En future il faut ajouté anti-robots (captcha)**
*car cette application est prive mai pas public donc n'a pas obligé d'ajouter la security anti-robot*

|Parametres      | Description | defaut value|
| ----------- | ----------- |	- |
| photo      | La photo de profil de l'artisan       |user.png|

C'est paramètre en haut c'est facultative .

#### Retour de server
Une erreur sur les parametre : 
```json
{
	"prenom":  [
		"The prenom field is required."
	],
	"nom":  [
		"The nom field is required."
	],
	"email":  [
		"The email field is required."
	],
	"password":  [
		"The password field is required."
	]
}
```

``` code
code request server : 500
```

L'artisan est bien ajouté a la base de donnée : 
```json
{

   "id": 1,
   "email": "mouhoub-1@gmail.com",
   "prenom": "mouhoub-1",
   "nom": "mardas-1",
   "photo": "user.png"
   "created_at": "2023-05-19T21:29:24.000000Z",
   "updated_at": "2023-05-19T21:29:24.000000Z"

}
```
``` code
code request server : 201
```

### Connexion client
Il faut appelée URL avec méthode **POST**.

```url
https://vps356969.ovh.net/api/client/login
METHOD : POST
```
avec paramètres **Obligatoir** : 
|Parametres      | Description |
| ----------- | ----------- |
| email     | Email de l'artisan
| password| mote de passe de l'artisan

#### Retour de serveur
Une erreur sur les parametre : 
```json
{
	"email":  [
		"The email field is required."
	],
	"password":  [
		"The password field is required."
	]
}
```
```code
code request server : 500
```
erreur de connecté :

```json
{
	"message":  "Email ou mot de passe incorrect"
}
```
```code
code request server : 500
```

L'artisan est bien connecté : 
remarque ce token c'est un sécurité il faut sauvegarde dan le téléphone utilisateur(artisan/client)
```json
{
	"token":  "3|rjMH1ldgAZjC6yuiRqkSyaVaTJB2taE7iv7SN4VE"
}
```
```code
code request server : 200
```

### Desconnexion client
Il faut appelée URL avec méthode **POST**.

```url
https://vps356969.ovh.net/api/client/logout
METHOD : POST
```
avec paramètres **Obligatoir** : 
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur |

#### Retour de serveur

Erreur de authentification (Vous avez oublié d'envoyé le token): 
 ```json
 {
	"message":  "Unauthenticated"
}
 ```
 ```code
code request server : 401
```

Le client est bien déconnecte : 
 ```json
 {
	"message":  "Vous etes bien deconnecte"
}
 ```
 ```code
code request server : 201
```

### Modifié des donnée d'un client

Il faut appelée URL avec méthode **PUT** avec paramètres
```url
https://vps356969.ovh.net/api/client/update
METHOD : PUT
```
Paramètres **Obligatoir**.
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur

Paramètres **facultative** mai il faut ou mois un paramètre.

|Parametres      | Description |
| ----------- | ----------- |
| prenom      | Prenom de l'artisan       |
| nom   | Nom de l'artisan        |
| email   | Email artisan        |
| password   | mote de pass de l'artisan        |

#### Retour de server
Erreur de authentification (Vous avez oublié d'envoyé le token): 
 ```json
 {
	"message":  "Unauthenticated"
}
 ```
 ```code
code request server : 401
```
 La modification est bien fait : 
  ```json
{
   "id": 1,
   "email": "mouhoub-1@gmail.com",
   "prenom": "mouhoub-1",
   "nom": "mardas-1",
   "photo": "user.png",
   "created_at": "2023-05-19T21:29:24.000000Z",
   "updated_at": "2023-05-19T21:29:24.000000Z"
}
 ```
 ```code
code request server : 201
```

### Supprimer un client.
Il faut appelée URL avec méthode **DELETE** avec paramètres
```URL
https://vps356969.ovh.net/api/client/delete
METHOD : DELETE
```

#### retour de serveur
Erreur de token : 
```json
{
	"message":  "Unauthenticated"
}
```
``` code
code request server : 500
```
Le artisan est bien supprimer de la base de donnée 
```json
{
	"id":  "1",
	"message": "Client est bien supprimer"
}
```
``` code
code request server : 201
```

## Avis
### Récupération les avis de client
Il faut appelée URL avec méthode **GET** sans paramètre
``` url
https://vps356969.ovh.net/api/avis/client/{id_client}
METHOD : GET
``` 
### Récupération les avis de l'artisan
Il faut appelée URL avec méthode **GET** sans paramètre
``` url
https://vps356969.ovh.net/api/avis/artisan/{id_client}
METHOD : GET
``` 

### Récupération les avis de client pour un artisan
Il faut appelée URL avec méthode **GET** sans paramètre
``` url
https://vps356969.ovh.net/api/avis/{id_artisan}/{id_client}
METHOD : GET
```
### Ajoute un avis
Il faut appelée URL avec méthode **POST** avec paramètre
``` url
https://vps356969.ovh.net/api/avis/post
METHOD : POST
```
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur |
|id_artisan|identifiant de l'artisan|
|text|le text de client (avis)|
|note|La note donnée par client **(integer)**|

### Modifier un avis
Il faut appelée URL avec méthode **POST** avec paramètre
``` url
https://vps356969.ovh.net/api/avis/post
METHOD : POST
```
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur |
|text|le text de client (avis)|
|note|La note donnée par client **(integer)**|

#### Retoure server
Erreur token 
```json
{
	"message":  "Unauthenticated"
}
```
``` code
code request server : 500
```
Erreur avis n'exist pas
```json
{
	"message":"L'avis n'ai pas trouvee"
}
```
``` code
code request server : 404
```
Erreur client n'a pas autorisation modifier un avis d'un autre client
```json
{
	"message":"Vous n'avais pas authorisation de modifier l'avis"
}
```
``` code
code request server : 401
```
Avis est bien modifier
```json
{
	"id":  5,
	"id_client":  8,
	"id_artisan":  2,
	"text":  "ce message est modifier 2",
	"note":  4,
	"created_at":  "2023-05-20T16:41:28.000000Z",
	"updated_at":  "2023-05-20T17:04:52.000000Z"
}
```
``` code
code request server : 201
```

### Suppermie un avis
Il faut appelée URL avec méthode **DELETE** avec paramètre
``` url
https://vps356969.ovh.net/api/avis/delete/{id}
METHOD : DELETE
```
|Parametres      | Description |
| ----------- | ----------- |
| Authorization     | Token generé par le serveur |

#### Retoure server
Avis est bien supprimer
```json
{
	"id":1,
	"message":"Vous avez pas les autorisation de supprimer"
}
```
``` code
code request server : 201
```
