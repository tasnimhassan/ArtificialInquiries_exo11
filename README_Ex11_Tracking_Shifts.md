# Ex11 - Tracking Shifts

## 1. Présentation de l'exercice

L'exercice **Tracking Shifts** consiste à observer comment notre manière
d'utiliser les LLM a changé depuis le début des exercices.

Pour faire cet exercice, il faut revenir sur les travaux réalisés
précédemment, consulter son **vademecum** et regarder son **historique
de conversations avec le LLM**. Cela permet de comparer les premières
utilisations avec les utilisations plus récentes.

L'idée est de ne pas regarder seulement le résultat obtenu avec le LLM,
mais aussi de s'intéresser à la manière dont on l'utilise.

Par exemple, on peut regarder comment les demandes étaient formulées au
début, comment elles sont formulées maintenant, si les demandes sont
devenues plus précises, si on vérifie davantage les réponses ou si on
utilise le LLM différemment selon les situations.

L'exercice demande aussi de prendre en compte plusieurs aspects de cette
pratique : **technique, professionnel, émotionnel et éthique**.

------------------------------------------------------------------------

## 2. Observer son utilisation des LLM

Pour réaliser l'exercice, il faut partir de situations réelles
rencontrées pendant les exercices.

Les conversations avec les LLM peuvent montrer plusieurs choses :

-   le type de demandes faites au LLM ;
-   la manière de formuler les demandes ;
-   les informations données dans les prompts ;
-   les réponses demandées ;
-   les corrections demandées après une première réponse ;
-   la manière de vérifier les résultats ;
-   les problèmes rencontrés ;
-   les changements dans la manière de travailler avec le LLM.

Il est important de ne pas seulement conserver une phrase générale comme
« j'utilise mieux les LLM maintenant ». Il faut pouvoir retrouver des
exemples dans l'historique qui permettent de voir cette évolution.

------------------------------------------------------------------------

## 3. Les différents aspects à observer

L'exercice demande de réfléchir à **tous les aspects de la pratique**.
Il ne s'agit donc pas uniquement de parler de programmation ou de
prompts.

### Aspect technique

L'aspect technique concerne la manière d'utiliser le LLM comme outil.

On peut par exemple observer :

-   la façon d'écrire les prompts ;
-   la précision des demandes ;
-   la quantité de contexte donnée au LLM ;
-   les demandes de code ;
-   les demandes de correction ;
-   les demandes d'explication étape par étape ;
-   les tests du code proposé ;
-   la vérification des erreurs.

Une évolution possible est de passer d'une demande très générale à une
demande beaucoup plus précise avec le contexte, l'erreur rencontrée et
le résultat attendu.

### Aspect professionnel

Le LLM peut aussi être utilisé dans le cadre des études et des projets
informatiques.

Il peut servir pour :

-   comprendre une technologie ;
-   apprendre un nouveau langage ;
-   résoudre un problème de programmation ;
-   préparer un projet ;
-   améliorer un document ;
-   préparer une présentation ;
-   trouver des idées pour un projet.

Il faut donc observer si la place du LLM dans la manière de travailler a
changé avec le temps.

### Aspect émotionnel

L'utilisation d'un LLM peut également provoquer différentes réactions.

Au début, on peut par exemple avoir moins confiance dans les réponses ou
ne pas savoir exactement comment utiliser l'outil.

Avec l'expérience, on peut être plus à l'aise pour poser des questions,
mais aussi devenir plus prudent lorsqu'une réponse semble incorrecte.

On peut donc observer :

-   la confiance ;
-   les hésitations ;
-   la frustration face à une réponse qui ne fonctionne pas ;
-   la satisfaction lorsqu'une solution fonctionne ;
-   la confiance qui augmente ou diminue avec l'expérience.

### Aspect éthique

L'utilisation d'un LLM demande également de réfléchir à certaines
limites.

Il faut notamment faire attention au fait qu'une réponse générée peut
être incorrecte.

Il est donc intéressant d'observer :

-   si les informations sont vérifiées ;
-   si le code proposé est testé ;
-   si l'on comprend réellement ce que l'on utilise ;
-   si l'on dépend trop du LLM ;
-   quelle part de réflexion personnelle reste présente ;
-   comment on utilise les réponses produites par le LLM.

------------------------------------------------------------------------

## 4. Comparer les différentes périodes

Le principe de **Tracking Shifts** est de suivre les changements dans le
temps.

Pour cela, les pratiques peuvent être regroupées en plusieurs périodes :

``` text
Début des exercices
        ↓
Premières utilisations du LLM
        ↓
Expérimentation
        ↓
Utilisation plus régulière
        ↓
Pratique actuelle
```

Cette comparaison permet de voir les changements progressivement.

Par exemple, au début une personne peut simplement demander une
solution. Plus tard, elle peut demander une explication, tester la
solution, signaler une erreur et demander une correction.

Cela montre que le changement ne concerne pas uniquement le contenu des
demandes, mais aussi la manière de travailler avec le LLM.

------------------------------------------------------------------------

## 5. Importance des exemples

L'exercice demande de **documenter sa pratique**.

Les exemples sont donc une partie importante du travail.

Un exemple peut venir d'une conversation dans laquelle :

-   une première demande n'était pas assez précise ;
-   le LLM a donné une réponse incorrecte ;
-   une deuxième demande a permis de corriger le problème ;
-   le code proposé a été testé ;
-   une explication supplémentaire a été demandée ;
-   la même méthode a été utilisée plusieurs fois.

Les exemples permettent de montrer concrètement comment la pratique a
changé au lieu de simplement donner une impression générale.

------------------------------------------------------------------------

## 6. Données nécessaires

Pour réaliser une solution technique à partir de cet exercice, il faut
pouvoir conserver les informations importantes concernant les
différentes utilisations du LLM.

Les principales données sont les suivantes.

### Utilisateur

Cette classe représente la personne qui utilise le LLM.

Elle peut contenir :

-   `id`
-   `nom`
-   `description`

### Exercice

Cette classe représente un exercice réalisé.

Elle peut contenir :

-   `id`
-   `titre`
-   `description`
-   `date`

Cela permet de savoir dans quel exercice une pratique a été observée.

### Conversation

Cette classe représente une interaction avec le LLM.

Elle peut contenir :

-   `id`
-   `date`
-   `modele`
-   `objectif`

Elle permet de garder une trace du contexte de l'utilisation.

### Pratique

Cette classe représente une manière particulière d'utiliser le LLM.

Par exemple :

-   demander une explication ;
-   demander du code ;
-   demander une correction ;
-   vérifier une réponse ;
-   demander une reformulation.

Elle peut contenir :

-   `id`
-   `nom`
-   `description`

### Evolution

Cette classe permet de représenter un changement dans une pratique.

Elle peut contenir :

-   `id`
-   `avant`
-   `apres`
-   `changement`
-   `raison`

Par exemple, elle peut permettre de conserver la différence entre une
ancienne manière de travailler et une nouvelle manière.

### Aspect

Cette classe permet d'indiquer à quel aspect correspond une observation.

Les valeurs peuvent être par exemple :

-   technique ;
-   professionnel ;
-   émotionnel ;
-   éthique.

Elle peut contenir :

-   `id`
-   `nom`
-   `description`

------------------------------------------------------------------------

## 7. Organisation des données

Les données sont liées entre elles.

Un utilisateur peut réaliser plusieurs exercices.

Un exercice peut contenir plusieurs conversations avec un LLM.

Une conversation peut montrer plusieurs pratiques.

Une pratique peut changer au cours du temps et avoir plusieurs
évolutions.

Une évolution peut être associée à un ou plusieurs aspects de la
pratique.

On obtient donc une organisation de ce type :

``` text
Utilisateur
     |
     ↓
  Exercice
     |
     ↓
Conversation
     |
     ↓
  Pratique
     |
     ↓
 Evolution
     |
     ↓
  Aspect
```

Cette organisation permet de relier les conversations aux changements
observés dans la pratique.

------------------------------------------------------------------------

## 8. Solution technique

Pour représenter ces données, on utilise un **diagramme de classes**.

Le diagramme permet de représenter :

-   les différentes classes ;
-   leurs attributs ;
-   les relations entre les classes ;
-   les cardinalités.

Le diagramme est réalisé avec **Mermaid**, qui permet de créer
facilement des diagrammes à partir de code.

Le diagramme peut être créé avec **Mermaid Live Editor** :

https://mermaid.live/

Le fichier correspondant au diagramme est :

`diagram_class.md`

------------------------------------------------------------------------

## 9. Classes utilisées dans le diagramme

Le diagramme contient les classes suivantes :

``` text
Utilisateur
Exercice
Conversation
Pratique
Evolution
Aspect
```

Chaque classe correspond à une partie des informations nécessaires pour
suivre la pratique avec les LLM.

Les relations permettent ensuite de relier les informations entre elles.

Par exemple :

``` text
Utilisateur → Exercice
Exercice → Conversation
Conversation → Pratique
Pratique → Evolution
Evolution → Aspect
```

------------------------------------------------------------------------

## 10. Pourquoi utiliser un diagramme de classes ?

Le diagramme de classes permet de mieux organiser les données avant de
développer une éventuelle application.

Dans cet exercice, il permet de représenter les différentes informations
que l'on souhaite conserver sur l'utilisation des LLM.

Il permet également de visualiser les relations entre :

-   les exercices ;
-   les conversations ;
-   les pratiques ;
-   les évolutions ;
-   les différents aspects de la pratique.

Le diagramme constitue donc une première étape pour construire une
solution informatique capable de garder une trace de l'évolution de
l'utilisation des LLM.

------------------------------------------------------------------------

## 11. Résultat attendu

À la fin de l'exercice, on dispose d'une représentation structurée de la
pratique avec les LLM.

Le travail permet de garder une trace :

-   des différentes utilisations ;
-   des changements dans le temps ;
-   des pratiques qui restent présentes ;
-   des exemples associés ;
-   des aspects techniques, professionnels, émotionnels et éthiques.

Le but est ainsi de transformer une expérience personnelle avec les LLM
en informations organisées qui peuvent être représentées sous forme de
données et de diagramme de classes.
