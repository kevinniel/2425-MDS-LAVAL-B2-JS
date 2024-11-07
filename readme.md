# COURS

## Comment intégrer du JS ?

- balises ```<script></script>```
- positionnées juste avant la fermeture de la balise ```</body>```

## Les Types en JS

- ```Boolean``` : true (1) / false (0)
- ```String``` : Chaine de caractère
- ```Integer || Int``` : Nombre entier
- ```Float``` : Nombre à virgule

## Les boucles en JS

permet d'itérer sur des éléments. Exemple : 

```js
let tablo = [1, 2, 3, 4, 5]

// je veux afficher tous les nombres, un par un (console.log)

for ( let i = 0; i < tablo.length - 1; i++ ) {
    console.log(i)
    console.log( tablo[i] )
}
```

## Bases du JS

- commentaire : utiliser le double slash ```//```
- afficher une information dans la console : ```console.log()```
- ```tableau.length``` : donne le nombre de lignes

## Déclaration de variable en JS

Déclarons une variable "toto" de 3 manière différentes

- ```const toto``` : ```const``` : lorsque l'on sélectionne des éléments HTML
- ```let toto``` : ```let``` : le reste 😇
- ```var toto``` : ```var``` : ne jamais utiliser 😁

## Comment récupérer des informations en JS ?

- ```document.querySelector('[selecteur]')``` : ne récupère Qu'un seul élément : le premier qu'il trouve !
- ```document.querySelectorAll('[selecteur]')``` : récupère tous les éléments
- fonctionne à partir des sélecteurs CSS. On retrouve dans les plus communs : 

    - ```table``` : sélectionne la/les balise(s) ```<table>```
    - ```.toto``` : sélectionne la/les balise(s) qui contiennent la classe "toto"
    - ```#tata``` : sélectionne la/les balise(s) qui continnent l'id "tata"

Exemple :
- ```document.querySelector('table')```
- ```document.querySelector('.toto')```
- ```document.querySelector('#tata')```

### Récupération avancée en JS

Vous pouvez effectuer une sélection à partir d'un élément déjà sélectionner en JS

exemple : 
```js
// Cette ligne sélectionne la première balise <table> de la page
const toto = document.querySelector('table')
// Cette ligne sélectionne toutes les balises <td> de l'élément précédemment sélectionné <table>, stocké dans la variable "toto"
const ligne_1 = toto.querySelectorAll('td')
```

## Comment intégrer des valeurs dans du HTML en JS

- ```element.innerText = "toto"``` : insère ou remplace la valeur "toto" en tant que **CONTENU TEXTUEL** dans l'élément
- ```element.innerHTML = "toto"``` : insère ou remplace la valeur "toto" en tant que **CONTENU HTML** dans l'élément

## Les écouteurs d'événements

- Permettent d'écouter les évènements
- S'applique sur un element

Exemple :

```js
const element = document.querySelector("form")
// Ajouter un écouteur d'évènement dessus
element.addEventListener('submit', function(event) {
    // le code ici s'executera à la soumission de l'element

    // permet d'éviter le comportement natif du navigateur
    event.preventDefault()

    // exécuter le code souhaité
})
```

### Les types d'évenements

- ```submit``` : soumission d'un élément
- ```click``` : au clic d'un élément
- ```hover``` : au survol d'un élément


## Création de HTML

- ```document.createElement('td')``` : crée une balise ```<td></td>```
- ```element.classList``` : permet d'interagir avec les classes HTML des éléments
- ```element.append(toto)``` : ajoute "toto" à la fin de "element"

## Création de fonctions simples

Les fonctions permettent d'avoir du code réutilisable

- ```function nom() {// code ici}``` : permet de déclarer une fonction, qui s'appelle ici "nom"
- ```nom()``` : permet d'appeler une fonction pour qu'elle s'exécute !

## Les data-attributes

Gère des attributs customs dans le HTML

- ```element.dataset.id``` : permet de récupérer la valeur contenu dans ```data-id```
- ```element.dataset.toto``` : permet de récupérer la valeur contenu dans ```data-toto```
