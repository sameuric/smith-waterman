# INFO-H-304 Projet - Algorithme de Smith-Waterman pour l'alignement de séquences

Ce projet a été réalisé au second quadrimestre de l'année 2018-19 en groupe, pour le cours de complément de programmation et d'algorithmique.

Mots-clefs : C++, STL, programmation dynamique, algorithme, Smith-Waterman, Makefile, séquences de protéines, bioinformatique

### Introduction

L’alignement de séquences est l’un des problèmes les plus communs en bioinformatique. Le but de l’alignement de séquences est de comparer deux séquences (ou plus), typiquement une séquence inconnue et une autre provenant d’une base de données, au moyen d’une certaine mesure de similarité. Les séquences à aligner peuvent être soit des séquences d’acides nucléiques (pour l’ADN et l’ARN), soit des séquences de peptides (pour les protéines).

L’algorithme de Smith-Waterman est un des algorithmes les plus utilisés pour ce problème et utilise la programmation dynamique pour réaliser l’alignement de séquences.

## Étapes d'implémentation du programme

Le but du projet est de réaliser un programme similaire à Swipe, utilisant l’algorithme de Smith-Waterman pour aligner les séquences de protéines.

1. **Base de données de protéines**  
   Une base de données de protéines contient toutes les séquences de protéines connues. Nous allons utiliser une des bases de données les mieux maintenues, appelée Swiss-Port. Cette base de données consiste en un fichier unique pouvant être téléchargé sur le site web UniProt.

2. **Protéine de requête**  
   Puisqu’il n’est pas réaliste pour un projet informatique de partir d’une protéine inconnue, on utilisera à la place des protéines connues, déjà présentes dans la base de données, comme protéines de requête. Le site web UniProt propose une interface facile à utiliser permettant de rapidement trouver toute protéine connue au moyen d’un identifiant.

3. **Convertir la base de données en format binaire**  
   La base de données que vous avez téléchargée est dans le format FASTA, qui est un simple format texte. En raison des surcoûts dù à l’encodage du texte et aux accès au système de fichiers, utiliser directement un fichier texte pour aligner les séquences serait beaucoup trop lourd. Dès lors, il est nécessaire de convertir le fichier FASTA vers un format binaire nommé BLAST, initialement développé par le US National Center for Biotechnology Information (NCBI).

4. **Matrices BLOSUM**  
   Dans l’algorithme de Smith-Waterman que vous allez implémenter pour effectuer l’alignement de protéines [SW81, Got82], la mesure de la similarité entre deux séquences de protéines se base sur des matrices de scores appelées BLOSUM et standardisées par le NCBI.

5. **Le programme Swipe**  
   Pour réaliser l’alignement de la protéine de requête P00533 avec toutes les protéines présentes dans la base de données, et ce avant de créer votre propre programme, nous allons utiliser un programme existant, nommé Swipe, qui se base sur le même algorithme que celui que vous devrez implémenter. La description détaillée et l’analyse de performance de Swipe sont détaillées dans l’article scientifique [Rog11].




Merci de vous référer à [https://uv.ulb.ac.be/course/view.php?id=106605](https://uv.ulb.ac.be/course/view.php?id=106605) pour les explications complètes du projet.

---

© Tous les codes C++ de ce projet sont la proriété de Sacha Meurice et des membres de son groupe de projet. Merci de ne pas copier les codes sans autorisation écrite préalable.
