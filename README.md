# MOVIE RECOMMENDATION SYSTEM 🎬
### Machine learning project
## *Author: Balkis Joudi* 
**LinkedIn:** https://www.linkedin.com/in/balkis-joudi-332076328/

---
---


## **I/OBJECTIF:** <br>
Centaines de platformes de streaming, milliers de films et millions de séries.... On trouve souvent des difficultés à choisir des films adaptés à nos gouts, et les méthodes traditionnelles de recherche, au lieu de nous aider, aggravent ce problème. D’ou, il est temps de concevoir un système de recommendation des films basé sur le machine learning, capable d'analyser les préférences de l’utilisateur et lui suggérer des films pertinents.

---
---
## **II/DATASET UTILISE:** <br>
  https://www.kaggle.com/datasets/ashfakyeafi/netflix-movies-and-shows-dataset

FEATURES <br>
1/show_id: Identifiant de chaque série ou film. <br>
2/type: Il s’agit d’un Movie ou d’un TV Show. <br>
3/title: Titre du contenu. <br>
4/director: Nom du ou des réalisateurs. <br>
5/cast: Liste des acteurs ptincipaux. <br>
6/country: Pays de production. <br>
7/date_added: Date d'ajout du contenu sur la plateforme(Netflix). <br>
8/release_year: Année de sortie du film ou de la série. <br>
9/rating: Classification par âge (TV-MA, PG-13, R, TV-14, etc.). <br>
10/duration: Durée du film (en minutes) ou nombre de saisons pour une série. <br>
11/listed_in: Catégorie du contenu (Action,comedy, Drama, Documentaries...). <br>
12/description: Résumé ou description du contenu. <br>

TARGET (CIBLE) <br>
  Les résultats des systèmes de recommendation ne sont pas une classe binaire (comme le système de mesure de la qualité d’eau: le résultat est potable ou non potable). Il mesure ,plutot, la similarité entre les films et les préférences de l’utilisateur. Donc, l’objectif est la proposition des contenus les plus pertinents pour un utilisateur.

---
---
## **III/EDA:** <br>
   Le dataset utilisé cette fois-ci est différent de ceux auxquels nous avons été habitués. La plupart des attributs sont catégoriques d’ou les instructions ne seront pas les memes: <br>
   *Les attributs show_id, title, director, cast, country, date_added, duration, listed_in et description présentent des centenus uniques qui ne se répètent pas donc il est inutile de les visualiser.

---
---
## **IV/PRETRAITEMENT:** <br>
   Dans ce projet, on va traiter des variables sous formes de string, alors, pour les cases nulles, on va les transformer en une chaine vide (Pour les projets précédents, les variables numériques sont remplacées par la médiane de la colonne).
   Une des solutions qu’on peut implémenter est de concevoir une autre colonne qui rassemble les données de toutes les autres pour faciliter le traitement. Donc, on a créé une nouvelle apppelée “movies”.

---
---
## **V/MODELE DU MACHINE LEARNING:** <br>
   Pour un système de recommendation, le traitement n’est pas le meme qu’un de classification: <br>
      *Puisque les variables sont alphanumériques, on a besoin de les transformer en des valeurs numériques ou des vecteurs avec la fonction TF-IDF (Term Frequency - Inverse Document Frequency).

---
---
## **VI/EVALUATION:** <br>
Les métriques precision_at_k, recall_at_k et f1_score_at_k sont utilisés pour évaluer les K premiers résultats retournés par un modèle:
Dans notre exemple:
Precision@10=10/10=1 → 100% des résultats affichés sont pertinents.
Recall@10=1,97% → Le système a trouvé 1,97% des films pertinents disponibles.
F1@10=3,87%: C’est l’équilibre entre la précision et le rappel.

---
---
## **VII/Conclusion:** <br>
Ce projet a montré que le Machine Learning ne se limite pas à un domaine spécifique et une application singulaire. C’est une technologie polyvalente capable de répondre à des problématiques variées meme celles de divertiisement. Et on a prouvé, grace à ce projet, qu’il est capable, en suivant un démarche d’instructions précis, d’améliorer l’expérience de l’utilisateur des platformes de streaming et faciliter la découverte de nouveaux films et séries correspondant à ses goûts. <br>
        Toutefois, ce modèle peut etre amélioré de plus en intégrant davantage d'informations sur les utilisateurs, en utilisant des techniques plus avancées telles que les modèles basés sur le Deep Learning afin de fournir des recommandations encore plus précises et personnalisées.

## Author
**Balkis Joudi**
-LinkedIn: https://www.linkedin.com/in/balkis-joudi-332076328/
