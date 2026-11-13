# SDD I module 4 : Importation et remaniement des données

Ce projet nécessite d'avoir assimilé l'ensemble des notions du quatrième module du cours de science des données biologiques 1. Il correspond au dépôt GitHub <https://github.com/BioDataScience-Course/A04Ia_transformation>. Il est distribué sous licence [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Objectifs

Ce projet est **individuel**, **court** et **cadré**. Il permet de démontrer que vous avez acquis les compétences suivantes :

-   Être capable d'importer des données depuis différents formats et différentes sources avec la fonction `read()`.

-   Maîtriser le remaniement de données, filtrer un tableau et le résumer pour en extraire l'information importante.

-   Comprendre et utiliser l'opérateur `%>.%` pour le chaînage des instructions.

## Consignes

Complétez les zones manquantes dans les fichiers `coral.qmd` et `pima.qmd`. Compilez les versions finales au format HTML. Vous avez une batterie de tests à votre disposition (onglet "Construire" -> bouton "Construire tout") pour vérifier l'état de votre travail. Note : utilisez ces tests à la fin. Concentrez-vous d'abord sur vos analyses, puis faites un rendu final des documents lorsque tout est complété, et seulement après, utilisez les tests. Il est contre-productif d'activer les tests à chaque nouvelle ligne de code ajoutée dans votre document ! Assurez-vous que vos documents Quarto compilent sans erreurs à la fin de votre travail **(très important : un document qui ne compile pas sans erreur devra être sanctionné de manière importante)**. Vérifiez aussi à la fin que vos derniers commits ont bien été pushés sur GitHub.

### Croissance de coraux en mésocosme

Complétez le fichier `coral.qmd` en suivant les instructions qui s'y trouvent. Le tableau de données est disponible via le lien suivant :

> <https://filedn.com/lzGVgfOGxb6mHFQcRn9ueUb/coral/corals.csv>

Le jeu de données reprend des mesures de croissance de différentes espèces de coraux. La masse des coraux est mesurée au début de l'expérience (temps t0) puis une seconde fois après sept jours (temps t7). Les variables du jeu de données sont :

-   **localisation :** aquarium dans lequel la bouture de corail est placée. Les installations sont composées de deux unités indépendantes (A et B) et de plusieurs aquariums par unité, reliés entre eux,
-   **species :** espèce étudiée,
-   **id :** code de la bouture de corail,
-   **salinity :** salinité mesurée en t7, grandeur sans unité,
-   **temperature :** température mesurée dans l'eau en t7, en °C,
-   **date :** date de la mesure en t7,
-   **time :** nombre de jours écoulés entre la mesure initiale et finale,
-   **gain :** gain de masse entre t0 et t7, en g,
-   **gain_std :** gain/masse initiale, sans unité.

### Cas de diabète chez des femmes PIMA

Complétez le fichier `pima.qmd`. Le jeu de données employé provient du package {MASS}. Vous avez à votre disposition une page d'aide pour mieux appréhender les variables de ce dernier (`?MASS::Pima.tr2`).

## Évaluation : un document qui compile, sur GitHub

**Un projet dont le(s) document(s) ne compile(nt) pas à partir de la version présente sur GitHub obtient la note de zéro pour ce travail.** Un document qui compile sur votre ordinateur, mais pas depuis GitHub (fichier oublié dans le commit, push non effectué...), est considéré comme ne compilant pas.

## Utilisation de l’IA

Dans le cadre de votre travail, vous avez le droit d’être aidé par l’intelligence artificielle. Le chatbot SciViews est disponible dans votre RStudio sur Saturn Cloud via l’addin Help. Il répond aux questions concernant le langage R, les statistiques et la science des données.

Vous restez responsables de tout ce que contiennent vos documents : vérifiez le code et les interprétations proposés par l'IA, et assurez-vous de pouvoir les expliquer.

L'utilisation de l'IA doit être déclarée dans les deux documents (`coral.qmd` et `pima.qmd`), dans la sous-section **Déclaration sur l'utilisation de l'IA** de la partie Matériel et méthodes : cochez la case qui correspond à votre situation dans le chunk `ai_comment` (remplacez `[]` par `[X]`), puis précisez en dessous l'utilisation que vous avez faite de l'IA et citez le ou les modèles employés.
