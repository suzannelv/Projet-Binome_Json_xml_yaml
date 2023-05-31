# Projet-Binome_Json_xml_yaml
## 2. XML(eXtensible Markup Language)
#### 1) Définiton
- C'est un **langage de balisage** qui fournit des règles pour définir toutes les données.
- C'est une format de transfert des données recommandé par W3C(World Wide Web Consortium).
- XML n'est pas prédéfini, on doit définir nos propres balises, et il est important de donner un sens à l'écriture des noms de balises.
   Par exemple: 
    ```
    <root>
       <school>Human Booster</school>
       <adress>Villeurbanne</adress>
    </root>
    ```
#### 2) Objectif
Le but principal de ce langage est le partage de données entre différents systèmes, tel qu'Internet, et de stocker les donner.
 --> En résumé,il s'agit de standardiser le format des données pour qu'elles soient structurées, faciles à lire et à manipuler.

#### 3) Règle de syntaxe
- XML a une structure fixe, la première ligne doit être **<?xml version="1.0" encoding="UTF-8" ?>**, avec un encodage optionnel. 
- Un document XML a  **un seul élément racine**, l'élément racine peut contenir n'importe quel nombre d'éléments enfants. Dans les éléments de balises, ils peuvent contenir des attributs, par exemple:
    ```
       <root lang="fr">Hello Git</root> 
    ```
- Tous les éléments XML doivent être des balises appariées.
