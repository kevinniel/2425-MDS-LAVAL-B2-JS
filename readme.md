# COURS

## Comment intégrer du JS ?

- balises ```<script></script>```
- positionnées juste avant la fermeture de la balise ```</body>```

## Bases du JS

- commentaire : utiliser le double slash ```//```
- afficher une information dans la console : ```console.log()```

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