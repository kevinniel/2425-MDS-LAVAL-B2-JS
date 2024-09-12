# COURS

## Comment intégrer du JS ?

- balises ```<script></script>```
- positionnées juste avant la fermeture de la balise ```</body>```

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