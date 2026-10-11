# ArtificialInquiries_11 — Tracking Shifts

Outil numérique issu de l'**exercice 11 « Tracking Shifts »** du vademecum
*Artificial Inquiries – A Vademecum for Workers in the Age of AI* (Gabriel Alcaras, sept. 2025),
bloc n°03 « Prompting » (pp. 81-83 du livre).

## 1. Description de l'exercice

> « Reflect on your experience with LLMs since you began the exercises. Browse through your
> vademecum and your conversation history in your LLM of choice. »

Consignes (Brief 02 – *How to Describe Your Practices*) :

- **Going wide** : couvrir tous les aspects de la pratique (technique, professionnel, émotionnel, éthique…).
- **Documenting your practice** : appuyer chaque réponse sur des **exemples précis**.

Deux questions ouvertes :

1. *How has your practice evolved?* (Comment votre pratique a-t-elle évolué ?)
2. *What aspects of your practice have remained consistent?* (Quels aspects sont restés constants ?)

## 2. Transformation en outil numérique

Le formulaire papier est une page blanche : l'outil numérique doit apporter de la **structure**
et de la **traçabilité** (exemples documentés, liens vers les conversations LLM, dimensions de la pratique).

### Fonctionnalités

- Saisie de **deux réponses** (évolution / constance), versionnées dans le temps.
- Découpage de chaque réponse en **observations** rattachées à une ou plusieurs **dimensions**
  (technique, professionnelle, émotionnelle, éthique, autre).
- Pour chaque observation : au moins un **exemple documenté** (extrait de conversation, capture, date, lien
  vers un exercice du vademecum).
- **Frise chronologique** des évolutions (avant / après le début des exercices).
- Export JSON-LD / CSV et affichage dans Omeka S.

### Solution technique

| Brique | Choix | Rôle |
|---|---|---|
| Stockage / publication | **Omeka S** (Apache + PHP + MySQL) | Items, vocabulaires, médias |
| Modèle de données | Resource templates Omeka S (voir `diagram_class.md`) | `Participant`, `Reflexion`, `Observation`, `Exemple`… |
| Saisie | Module Omeka S *Contribute* ou *Webform* (à tester) | Formulaire web remplaçant le papier |
| Alternative | Page HTML/JS + API REST Omeka S (`/api/items`) | Formulaire sur mesure |
| Références | **Zotero** (groupe `THYP_26-27`) | Références & annotations (vademecum, protocole) |
| Visualisation | Mermaid / timeline JS | Frise des évolutions |
| Versionnement | GitHub | Dépôt `ArtificialInquiries_11` |

### Installation locale d'Omeka S

1. Installer Apache, PHP ≥ 8.1 (extensions `pdo_mysql`, `xml`, `intl`, `gd`/`imagick`), MySQL/MariaDB.
2. Créer la base : `CREATE DATABASE omekas CHARACTER SET utf8mb4;`
3. Télécharger Omeka S : <https://omeka.org/s/download/>, décompresser dans le dossier web.
4. Renseigner `config/database.ini` (user, password, dbname, host).
5. `chmod -R 775 files/` et activer `mod_rewrite`.
6. Ouvrir `http://localhost/omeka-s/install` puis créer le compte administrateur.
7. Tester l'API : `http://localhost/omeka-s/api/items`.

## 3. Structure du dépôt

```
ArtificialInquiries_11/
├── README.md
└── diagram_class.md
```
