Kebab Challenge
===================


Ce repositoriy se compose de plusieurs exercice permettant a un candidat de montrer l'entendu de ses connaissances en tant que lead technique. Les exercices sont à réaliser dans l'ordre. Le candidat devra forker se repository et proposer sa pull request qui permettra de valider le test. Seront jugés les points suivants :

- Pertinence des réponses
- Connaissance du candidat sur les sujets traités
- Rapidité d'exécution 

----------
**Préambule**
Je souhaite ouvrir mon premier restaurant en ligne. Salade, Tomates et Oignons seront les ingrédients nécessaires à la confection de mon plat. Tous les repas seront virtuels mais les problématiques seront elles bien réelles !

> **Note:**

> Organisez votre présentation comme vous le souhaitez. La nomenclature des livrables est entièrement libre

----------
1 / Conception
-------------

###### **Temps conseillé** : 1/2 heure

Avant de me lancer dans mon projet, je vais avoir besoin d'un MCD. Ce schéma sera très simple mais devra être évolutif car ma carte est susceptible de s'agrandir très vite. Sur un modèle **EAV**, merci de proposer un MCD permettant de gérer des clients, plats qui seront composés d'attributs que je ne connais pas encore a l'avance et de catégories qui me permettrons de gérer ma carte. 

> **Note:**

> Certains outils en ligne comme http://mocodo.wingi.net/ https://www.draw.io/ ou http://www.gliffy.com permettent de réaliser rapidement un MCD. Utilisez celui que vous souhaitez et créer le visuel sous formes d'image / schéma exploitable. 


2 / Architecture
-------------

###### **Temps conseillé** : 1/2 heure

Avant de commencer a développer mon application, je vais avoir besoin d'un environnement technique. Mon Architecte logiciel étant malade, il m'a indiqué l'ensemble des briques dont j'ai besoin mais n'a pas terminé le schéma pour me montrer les relations qu'auront les briques les unes avec les autres. Merci de finaliser le schéma d'une manière logique: [Schéma Gliffy](schema_exemple_archi.gliffy)

> **Note:**

> Les notions de clusters ne sont pas visuellement représentées dans la liste des éléments disponibles. N'oubliez pas que cette application sera scalable et disposera d'un pool de plusieurs machines pour les frontaux. Merci de faire apparaître cette notion. 

3 / Réalisation 
-------------

###### **Temps conseillé** : 2 heures ~

Maintenant que tout est prêt, je souhaite commencer rapidement mon prototype fonctionnel. Pour ce faire, vous pouvez utiliser le framework de votre choix mais devrez respecter les spécifications suivante :

- Partir d'un d'une image docker (ou docker-compose) me permettant d'embarquer mon applicatif et le rendre portable.
- Utiliser les patterns php adéquats me permettant de livrer un code SOLID

Cette application étant une POC, je n'ai pas besoin de BDD ni MVC mais uniquement de classes PHP pour fonctionner. Un système de stockage peux tout à fait être utilisé si vous le souhaitez ;) 
Afin de pouvoir tester mon application j'ai besoin :

- créer une commande CLI  mer permettant d'instancier un client ou une cliente
- créer une commande CLI permettant d'ajouter l'un des ingrédients suivants dans sa commande  : salade / tomate / oignon. Je peux en ajouter en tant que je veux
- créer une commande CLI me permettant de lister le nombre d'ingrédients dans ma commande


**Attention**  afin de prévenir mes clients que la Harissa est particulièrement corsé chez nous, l'application devra lever une exception afin de me prévenir en cas d'ajout d'harissa dans la liste des ingrédient

> **Note:**

> Rappel des patterns PHP > https://github.com/domnikl/DesignPatternsPHP 
> A partir de votre pull request, je dois être capable de cloner votre proposition et l’exécution selon le mode opératoire fourni. Une documentation me permettant de connaitre le moyen de setup votre projet, le runer et exécuter les commandes qui valideront ce test est le bienvenue ;)

Bon courage !
