# Authorship Attribution using BERT

Ce projet est une évaluation de l'attribution d'auteur en utilisant un modèle BERT pour déterminer l'auteur des Federalist Papers. L'objectif est de classifier les textes en fonction de leur auteur (Alexander Hamilton ou James Madison) en utilisant des techniques de traitement du langage naturel (NLP).

## Contexte

Les Federalist Papers sont une série de 85 essais écrits entre 1787 et 1788 par Alexander Hamilton, James Madison et John Jay. Ces essais ont été publiés sous le pseudonyme "Publius" pour promouvoir la ratification de la Constitution des États-Unis. Cependant, l'auteur de certains de ces essais reste incertain. Ce projet vise à résoudre ce problème en utilisant un modèle BERT pour attribuer les essais à leur auteur probable.

## Structure du projet

Le projet est structuré en plusieurs étapes :

1. **Préparation des données** : Les données sont formatées pour être utilisées avec le modèle BERT.
2. **Configuration du modèle** : Les paramètres du modèle BERT sont configurés, y compris la longueur maximale des séquences, la taille du batch, et le modèle pré-entraîné à utiliser.
3. **Configuration de l'entraîneur** : Les paramètres de l'entraîneur sont définis, y compris le nombre d'époques, le niveau de précision, et le niveau de mélange automatique (AMP).
4. **Entraînement du modèle** : Le modèle est entraîné sur les données formatées.
5. **Inférence** : Le modèle est utilisé pour prédire l'auteur des essais disputés.

## Résultats

Les résultats de l'inférence sont les suivants :

- **test49.tsv** : HAMILTON
- **test50.tsv** : HAMILTON
- **test51.tsv** : HAMILTON
- **test52.tsv** : HAMILTON
- **test53.tsv** : HAMILTON
- **test54.tsv** : HAMILTON
- **test55.tsv** : HAMILTON
- **test56.tsv** : HAMILTON
- **test57.tsv** : HAMILTON
- **test62.tsv** : HAMILTON

Ces résultats indiquent que le modèle a attribué tous les essais disputés à Alexander Hamilton. Cependant, selon une analyse précédente utilisant des machines à vecteurs de support (SVM), James Madison serait l'auteur le plus probable de tous les essais disputés. Il est possible d'obtenir ce résultat en ajustant les paramètres du modèle.

## Comment exécuter le code

1. **Cloner le dépôt** :
   ```bash
   git clone https://github.com/votre-utilisateur/authorship-attribution-bert.git
   cd authorship-attribution-bert
2- Installer les dépendances :
Assurez-vous d'avoir installé les bibliothèques nécessaires, notamment nemo, pandas, et omegaconf.

3- Exécuter le notebook :
Ouvrez le notebook assessment.ipynb dans un environnement Jupyter et exécutez les cellules dans l'ordre.

4- Entraînement et inférence :
Le notebook contient des instructions pour entraîner le modèle et effectuer l'inférence sur les essais disputés.

Dépendances
Python 3.8

NeMo

Pandas

Omegaconf



Ce projet a été réalisé dans le cadre du cours NLP de NVIDIA DLI. Merci à NVIDIA pour leur support et leurs ressources éducatives.
