## Introduction
JSON, XLM et YAML sont des langages de sérialisation de données :
   > "Chaque fois que vous souhaitez envoyer une structure de données ou un objet sur des réseaux informatiques, par exemple Internet, vous devez le transformer en un format spécial pour le lire et le stocker. Le processus est généralement connu sous le nom de sérialisation et est d'une importance énorme sur le Web. Un exemple d'utilisation courant de sérialisation est la lecture de données à partir de bases de données et leur transfert sur le Web."

- XML prend en charge les types de données complexes tels que les graphiques, les images et d'autres types de données non primitifs. 
- JSON ne prend en charge que les chaînes de caractère (string) , les nombres, les tableaux, les booléens et les objets. 
- YAML, d'autre part, prend en charge les types de données complexes tels que les timesstamps, les séquences, les valeurs imbriquées et récursives et les types de données primitifs.


## 1 JSON (JavaScript Objet Notation) 

#### 1) Définition Json? 

 JSON est un format de données semblable à la syntaxe des objets JavaScript, qui a été popularisé par Douglas Crockford. Malgré sa syntaxe très similaire à celle des objets littéraux JavaScript, JSON peut être utilisé indépendamment de ce langage et ainsi, de nombreux autres langages de programmation disposent de fonctionnalités permettant d'analyser la syntaxe du JSON et d'en générer. 

#### 2) Pourquoi utiliser JSON?

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

## 3 YAML
#### Définition YAML?
 Pour certains, YAML est l'acronyme de Yet Another Markup Language, pour d'autres, c'est l'acronyme récursif de YAML Ain't Markup Language
 #### Pourquoi utiliser YAML?
Le langage YAML est principalement utilisé pour créer des fichiers de configuration. Il est recommandé de coder les fichiers de configuration en YAML plutôt qu'en JSON, car même si ces langages peuvent être utilisés de manière interchangeable dans la plupart des cas, YAML reste plus facile à lire et à utiliser

 
 #### Syntaxe
 YAML comporte des fonctions issues de Perl, C, XML, HTML et d'autres langages de programmation. 
Les symboles de formatage habituels, tels que les accolades, les crochets, les balises d'ouverture et de fermeture ou les guillemets, n'existent pas. Les fichiers YAML sont plus faciles à lire,  Les caractères de tabulation ne sont pas autorisés par défaut pour assurer la portabilité sur différents systèmes, alors il faut utiliser des espaces blancs à la place.

- objet : une collection de paires key-value.

- tableaux : un ensemble de valeurs ordonnées séquentiellement

- scalars : une valeur unique et indivisible, par exemple: string, boolean, int, float, null, date, etc.


## Comparasion de ces trois formats de données
#### 1) JSON
```
"devices": {
    "router": [
    {
      "name": "CSR1000V",
      "vendor": "Cisco",
      "type": "virtual"
    },
    {
      "name": "1921",
      "vendor": "Cisco",
      "type": "hardware"
    }
  ]
}
```
#### 2) XML
```
<?xml version="1.0" encoding="UTF-8" ?>
<devices>
  <router>
    <name>CSR1000V</name>
    <vendor>Cisco</vendor>
    <type>virtueal</type>
  </router>
   <router>
    <name>1921</name>
    <vendor>Cisco</vendor>
    <type>hardware</type>
  </router>
</devices>
```

#### 3) YAML
```
devices:
  router:
   - name: CSR1000V
     vendor: Cisco
     type: virtual
   - name: 1921
     vendor: Cisco
     type: hardware
```


