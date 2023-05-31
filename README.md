# Projet-Binome_Json_xml_yaml
# Projet-Binome_Json_xml_yaml

## 1 JSON (JavaScript Objet Notation) 

#### 1)C'est quoi Json? 

 JSON est un format de données semblable à la syntaxe des objets JavaScript, qui a été popularisé par Douglas Crockford. Malgré sa syntaxe très similaire à celle des objets littéraux JavaScript, JSON peut être utilisé indépendamment de ce langage et ainsi, de nombreux autres langages de programmation disposent de fonctionnalités permettant d'analyser la syntaxe du JSON et d'en générer. 

#### 2) Pourquoi  JSON?

 Il est habituellement utilisé pour structurer et transmettre des données sur des sites web (par exemple, envoyer des données depuis un serveur vers un client afin de les afficher sur une page web ou vice versa) Il sert à envoyer des informations, depuis un serveur vers un utilisateur, afin de les afficher sur une page web, ou inversement. Ces caractéristiques en font un langage d’échange de données idéal et universel.

 
#### 3) Nota bene

- JSON peut être combiné avec d'autres languages C++, Java, Python
- Les documents JSON sont relativement légers   
- Il est très facile d'usage - pas d'algorythlme. Un objet JSON est uniquement un format de données — il ne contient que des propriétés mais pas de méthodes.
-Attention à la securité tout de même car les fichiers json s'executent automatiquement sur toute page web solicitée par un navigateur - attaque par insertion dans le code javascript

#### 4) Syntaxe:

La notation JSON nécessite l'usage des guillemets pour être valide. Il est obligatoire d'utiliser des guillemets et non les apostrophes autour des chaînes de caractères et des noms de propriétés.
#### 5)Exemple concret

```
var courses = {
 "fruits": [
   { "kiwis": 3,
     "mangues": 4,
     "pommes": null
   },
   { "panier": true },
 ],
 "legumes":
   { "patates": "amandine",
     "figues": "de barbarie",
     "poireaux": false
   }
};
```
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
