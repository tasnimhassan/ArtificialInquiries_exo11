Ex11 - Tracking Shifts

1. Description de l'exercice

L'exercice Tracking Shifts consiste à réfléchir à l'évolution de notre pratique des LLM depuis le début des exercices.



L'objectif est d'identifier :



comment notre manière d'utiliser les LLM a changé ;

les pratiques qui sont restées les mêmes ;

les aspects techniques, professionnels, émotionnels et éthiques de cette évolution ;

des exemples précis permettant de justifier les observations.



Dans mon cas, l'évolution peut être observée à travers mes différentes conversations avec un LLM et les exercices réalisés.



Par exemple, au début, je pouvais utiliser le LLM principalement pour obtenir directement une réponse ou du code. Avec l'expérience, ma pratique peut devenir plus précise : je donne davantage de contexte, je précise mes contraintes et je vérifie davantage les réponses obtenues.



Certaines pratiques restent cependant constantes, comme l'utilisation du LLM pour comprendre une notion, corriger un problème ou m'aider à avancer dans un exercice.

2. Données à gérer

Pour représenter cet exercice sous forme de données, il est nécessaire de conserver plusieurs informations.

Utilisateur

L'utilisateur représente la personne qui utilise le LLM.



On peut conserver :



un identifiant ;

un nom ;

une description de sa pratique.

Exercice

Un exercice représente une activité réalisée dans le cadre du travail avec les LLM.



On conserve :



un identifiant ;

un titre ;

une description ;

une date.

Conversation

Une conversation représente une interaction avec un LLM dans le cadre d'un exercice.



On conserve :



un identifiant ;

une date ;

le modèle utilisé ;

l'objectif de la conversation.

Pratique

Une pratique représente une manière d'utiliser le LLM.



Par exemple :



demander une explication ;

demander du code ;

corriger une réponse ;

reformuler une question ;

vérifier une information.

Évolution

Une évolution permet de comparer une pratique à différents moments.



Elle permet de décrire :



la situation avant ;

la situation après ;

ce qui a changé ;

la raison du changement.

Aspect

Un aspect permet de classer les observations réalisées pendant la réflexion.



Les principaux aspects sont :



technique ;

professionnel ;

émotionnel ;

éthique.

3. Solution technique

La solution consiste à utiliser une structure de données relationnelle.



Les principales entités sont :



Utilisateur, Exercice, Conversation, Pratique, Evolution et Aspect.



Un utilisateur peut réaliser plusieurs exercices.



Un exercice peut contenir plusieurs conversations.



Une conversation peut être associée à plusieurs pratiques.



Une évolution permet de décrire le changement d'une pratique entre deux périodes.



Les aspects permettent de classer les évolutions observées.

4. Exemple de données

Un exemple d'évolution pourrait être :



Avant :

Je demandais directement au LLM de résoudre un problème.

Après :

Je donne davantage de contexte et je précise le résultat que je souhaite obtenir.

Évolution :

Ma manière de formuler les prompts est devenue plus précise.

Aspect :

Technique.

Un autre exemple peut concerner la vérification :



Avant :

Je pouvais utiliser directement la réponse donnée par le LLM.

Après :

Je prends davantage le temps de vérifier les informations et le code proposés.

Aspect :

Éthique et technique.

5. Objectif du modèle de données

Le diagramme de classes permet de représenter les informations nécessaires pour documenter l'évolution de la pratique avec les LLM.



Il permet notamment de conserver les exemples utilisés pour répondre aux deux questions principales de l'exercice :



How has your practice evolved?

What aspects of your practice have remained consistent?



Les données peuvent ensuite être utilisées pour produire une réflexion chronologique sur l'utilisation des LLM.