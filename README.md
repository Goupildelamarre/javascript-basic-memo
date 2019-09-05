# 

# Types
### Six **types** primitifs
```javascript
    let string = 'Un texte'
    let number = 12.4
    let boolean = true;
    let null = null
    let undefined = undefined;
    let symbol = Symbol('Symbole');
```
### Puis les **objets**
```javascript
    let object = {cle: 'valeur'}

    let array = [1, 'deux', false]

    function unefonction() {

    }
```

# Vocabulaire de base
```javascript
    let coffee = 5 + 4
```
* 'let' est le mot clé réservé 
* 'cafe' est la variable 
* '=' est l'opérateur 
* '5 + 4' est l'expression
* 
#L'Objet
Un objet est un type de donnée en JavaScript utilité pour contenir une combinaison de données grâce à une simple paire clé-valeur
```javascript
let user = {
    name: 'Jean Bon',
    yearOfBirth: 1990,
    calculateAge: function () {
        // Code de la fonction
    }    
}
```
# La fonction 
Une fonction est un bout de code encadré dans une section. 
Ce bout de code est SEULEMENT exécuté quand la fonction est appelée

Une fonction a deux parties : La déclaration / définition et la partie utilisation 
```javascript
function add(param1, param2) {
    let a = param1 + param2;
    return a;
}
```

#Opérateurs#

[Les opérateurs sont est mots-réservés qui exécutent une action sur les valeurs ou variables](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)


#Conditions#
###IF/Else###
```javascript
if (a > 0) {
    // run this code
} else if (a < 0) {
    // run this code
} else {
    // run this code
}
```
### Opérateur ternaire###
```javascript
(expression) ? : ifTrue : ifFalse
```

### Switch
```javascript
switch (expression) {
    case choice1:
    // run this code
    break;
    case choice1:
    // run this code
    break;
    default:
    // run this code
}
```
# Boucles
###Boucle for
```javascript 
for (initial-expression; condition; second-expression){
    // run this code in block
}
```

###Boucle while
```javascript 
while (i<3){
    // run this code in block
    i++;
}
```

### Boucle do while
```javascript 
do {
// run this code in block
i++;
} while (i<3);
```

#Manipuler le DOM (Document Object Modal)
### Récupérer des éléments
```javascript 
// Preferred way:
document.querySelector('css-selectors')
document.querySelectorAll('css-selectors', ...)
// Old ways, and still work:
document.getElementsByTagName('element-name')
document.getElementsByClassName('class-name')
document.getElementById('id')
```
### Créer et cloner des éléments
```javascript 
document.createElement('div')
document.createTextNode('some text here')
node.cloneNode()
node.textContent = 'some text here'
```

### Ajouter un node au document 
```javascript 
parentNode.appendChild(nodeToAdd)
parentNode.insertBefore(nodeToAdd, childNode)
```

### Modifier un élément 
```javascript 
node.style.color = 'red'
node.style.padding = '10px',
node.style.fontSize = '200%'
node.setAttribute('attr-name', 'attr-value')
node.removeAttribute('attr-name')
```
### Récupérer et modifier la classe d'un élement 
```javascript 
node.classList
node.classList.add('class-name', ...)
node.classList.remove('class-name', ...)
node.classList.toggle('class-name')
node.classList.contains('class-name')
node.classList.replace('old', 'new')
```

### Supprimer un node
```javascript 
parentNode.removeChild(nodeToRemove)
// Hack to remove self
nodeToRemove.parentNode.removeChild(nodeToRemove)
```

### Les événements
```javascript 
    node.addEventListener('event-name', fonction);
    node.removeEventListener('event-name', fonction);
```
[Les différents types d'événements](https://developer.mozilla.org/fr/docs/Web/Events)


### Qu'est-ce que un "Node" ? 
**Node** : Chaque élément dans l'arbre du DOM est appelé un node. Il y a deux types de nodes: un "text node" et un "element node"

** Node Enfant** : Un node qui est l'enfant d'un autre 
** Node Parent** : Un node qui est le parent d'un autre 
** Node Sisbling** : Un node qui partage le même parent 

# Propriétés auto-héritées aux types
* [String](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/String)
* [Number](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/Number)
* [Boolean](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/Boolean)
* [Array](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/Array)


Inspiré et traduit de l'anglais depuis [javascript-cheatsheet](https://github.com/iLoveCodingOrg/javascript-cheatsheet)

[Pour aller plus loin: devhints.io/es6](https://devhints.io/es6)