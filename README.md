# Servier_Test
**Objectif** : Réaliser un code clair et proprement structuré. Mettre en avant les éléments considérés comme essentiels pour du code utilisable dans un environnement de production. Mettre l’accent sur vos connaissances en conception de jobs de manipulation de données ainsi que les bonnes pratiques python.

**1. Les données**


Vous avez à votre disposition les 4 fichiers de données suivants :

drugs.csv : contient les noms de drugs (des médicaments) avec un id (atccode) et un nom (drug) pubmed.csv : contient des titres d’articles PubMed (title) associés à un journal (journal) à une date donnée (date) ainsi qu’un id (id).

pubmed.json : même structure que pubmed.csv mais en format JSON.

clinical_trials.csv : contient des publications scientifiques avec un titre (scientific_title), un id (id), un journal (journal) et une date (date).

**2. Data pipeline**

Votre data pipeline doit produire en sortie un unique fichier JSON qui représente un graphe de liaison entre les différents médicaments et leurs mentions respectives dans les différentes publications PubMed, les différentes publications scientifiques et enfin les journaux avec la date associée à chacune de ces mentions. La représentation ci-dessous permet de visualiser ce qui est attendu. Il peut y avoir plusieurs manières de modéliser cet output et vous pouvez justifier votre vision :

**Règles de gestion :**

- Un drug est considéré comme mentionné dans un article PubMed ou un essai clinique s’il est mentionné dans le titre de la publication.
- Un drug est considéré comme mentionné par un journal s’il est mentionné dans une publication émise par ce journal.
![image](https://user-images.githubusercontent.com/74152853/120648815-59696400-c47c-11eb-8c14-7533e45a98c0.png)

**CODE**

**Bibliothèque :**

-Pandas : Pandas est principalement utilisé pour l'analyse de données. Pandas permet d'importer des données à partir de différents formats de fichiers tels que les valeurs séparées par des virgules, JSON, SQL, Microsoft Excel. Pandas permet d'effectuer diverses opérations de manipulation des données, telles que la fusion, le remodelage, la sélection, ainsi que des fonctions de nettoyage et de traitement des données.

-Numpy : NumPy est une bibliothèque Python qui fournit une structure de données simple mais puissante : le tableau n-dimensionnel. Il s'agit de la base sur laquelle repose la quasi-totalité de la puissance de la boîte à outils de science des données de Python, et l'apprentissage de NumPy est la première étape du voyage de tout scientifique des données Python.
