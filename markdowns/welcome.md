
# HTML/CSS - Niveau 1

## Intro
Concrètement, une page web c'est quoi ? De simples fichiers texte !
Plus précisément : un fichier HTML, et un fichier CSS. L'html s'occupe de la structure. Le CSS de la déco.
Rendez-vous sur le site ... et faites clic-droit > afficher le code source de la page.
L'html est organisé de manière hiérarchique, comme des poupées russes.
Cliquez sur le lien css ...
Le css fonctionne de pair avec l'html. Le css dit : Pour toutes les balises H1, appliquer la couleur rouge.

## HTML
Prenons l'exemple d'un manuel scolaire (lien). Il est composé de chapitre, de sous-chapitre, de leçons, etc...
Une leçon contient un titre, une introduction, différentes sous-parties, des encarts ("A retenir", "Dates clés", etc).
On pourrai le représenter de cette manière :
- Manuel Scolaire
    - Chapitre 1
        - Leçon 1
            - Intro
            - Partie 1
            - Partie 2
            - Conclusion
        - Leçon 2
            - ...
    - Chapitre 2
        ...
Ou sous forme de poupée russe, selon la syntaxe html :
````html
<Book>
    <Chapter>
        <Lesson>
            <Intro>...</Intro>
            <Partie>...</Partie>
            <Partie>...</Partie>
            <Conclusion>...</Conclusion>
        </Lesson>
        <Lesson>...</Lesson>
    </Chapter>
    <Chapter>...</Chapter>
</Book>
````
Une page html serait représentée ici par "Lesson", et le site internet complet par "Book".

Pratique :
- Créez un fichier maPage.html
- Ecrivez : Hello !
- Ouvrez le fichier dans un navigateur

Pour que notre fichier html soit bien interprêté par le navigateur, nous allons rajouter des balises de bases :
Code...

Il existent plusieurs balises différentes en html. Ces balises vont jouer un rôle très important dans le référencement Google.
Les principales balises à connaître sont : ...
Voici comment nous pouvons les utiliser : ... (audio dictée)

Depuis le navigateur, faites clic-droit sur le texte > inspecter l'élément.

## CSS
Remarquez le panneau à droite, il indique ...
Le navigateur utilise du CSS "par défaut", une typo, une couleur, etc...
Par défaut, tous les éléments que nous allons rajouter, s'ajouteront les uns à la suite des autres.
- Modifiez le fichier html comme suit
- Observez chaque tag avec l'inspecteur élément
Remarquez que la balise em ne passe pas à la ligne. Certains éléments sont par défaut, en display: block, et d'autres en display: inline.
Ceux en display block, prennent toute la largeur disponible (ce qui force les éléments suivant à passer à la ligne), tandis que les éléments inline, s'adapate à la taille de leur contenu.

Nous allons modifier le style par défaut, pour centrer le titre :
- Créer un fichier monStyle.css
- Modifier le fichier html pour lui dire ce charger le fichier css
- Dans le fichier css : ajouter ...
- Rechargez la page html dans le navigateur
- Observer ce qui apparaît dans l'inspecteur CSS

Les principales propriétés à connaître sont : ...
Voici comment nous pouvons les utiliser : ... (audio dictée)

Comment faire pour coloriser tous les liens dans le header, sans toucher aux autres ?
Le sélecteur peut être plus précis. Par exemple "div a" permettra de cibler tous les a contenus dans un div.
Et pour cibler un élément en particulier ?
Nous pouvons utiliser des classes : modifiez l'html, puis le css
Notez l'utilisation du point pour les classes.

Retournez sur le lien ... observez les sélecteurs dans le fichier css, et remarquez tout ce qu'il est possible de faire.

Parmi les propriétés css, on retrouve celles qui permettent de positionner des éléments.
Notamment Flex...

## A retenir
- Strucutre html de base
- Principales balises html (cf appli)
- Principales propriétés css
- Disposition Flex

## Quiz
## Contrôle des connaissances
...
## Interprétation
Vous êtes un navigateur web. Dessinez :
````html runnable
<!DOCTYPE html>
<html>
  <head>
    <title>Mon Document</title>
    <meta charset="UTF-8">
    <style type="text/css">
        header {
            display: flex;
        }
        header img {
            flex: 1;
        }
        header ul li {
           display:inline;
        }

        h1 {
            text-align: center;
        }

        div {
            display: flex;
            width: 80%;
            margin: auto;
            border: 1px solid black;
        }

        article {
            flex: 1;
        }

        article p:last-child {
            text-align: center;
        }
    </style>
  </head>
  <body>
    <header>
        <img src="#" alt="Logo">
        <nav>
            <ul>
                <li>Accueil</li>
                <li>Portfolio</li>
                <li>À propos</li>
                <li>Contact</li>
            </ul>
        </nav>
    </header>
    <main>
        <h1>Titre de ma page</h1>
        <div>
            <article>
                <img src="#" alt="Image" />
                <h2>Mon article 1</h2>
                <p>Description</p>
                <p><a href="#">Lire</a></p>
            </article>
            <article>
                <img src="#" alt="Image" />
                <h2>Mon article 2</h2>
                <p>Description</p>
                <p><a href="#">Lire</a></p>
            </article>
            <article>
                <img src="#" alt="Image" />
                <h2>Mon article 3</h2>
                <p>Description</p>
                <p><a href="#">Lire</a></p>
            </article>
        </div>
    </main>
    <footer>Footer</footer>
  </body>
</html>

````
Comment est votre maquette :
- Beaucoup d'erreur
- Peu d'erreur
- Parfaite

## Résolution de problèmes
...
### FAQ - Bugs les plus courants
...

## Composition
Intégrez ce wireframes : ...

# HTML/CSS - Niveau 2 - Pour aller plus loin
Serveur web
Référencement Google
ID, Classes
Grid, Float, ...
After, first-child, ...
Typo
Media queries

# Examens - Intégration maquette en 1h + Debrief


# Test

Initialise la variable myVar à true
Crée le tableau myArray qui comprend les 3 élements suivant : A, B et C
Crée l'objet myObject qui a une les 2 propriétés : myProp1 qui vaut 1, et myProp2 qui vaut "hello"
Crée la fonction myFunc qui prend en paramètre myParam et qui le retourne

Boucle sur le tableau myArray, et log chaque item
Appel la fonction myFunc, en passant myVar en paramètre, et log le retour
Log la propriété myProp1 de myObject

Modifie myVar à false
Modifie le second item du tableau MyArray, en "b"
Modifie la propriété myProp2 de myObject, en "bonjour"


# Welcome!

This Nodejs template lets you get started quickly with a simple working example using npm. If it is your first contribution then you should have a look at the [Getting Started](https://tech.io/doc/getting-started-create-playground) document.


The source code is on [GitHub](https://github.com/TechDotIO/nodejs-template), please feel free to come up with proposals to improve it.

# Hands-on Demo

@[Luke, how many stars are there in these galaxies?]({ "stubs": ["universe.js"], "command": "node_modules/mocha/bin/mocha universe.spec.js --reporter list" })

Check out the markdown file [`welcome.md`](https://github.com/TechDotIO/nodejs-template/blob/master/markdowns/welcome.md) to see how this exercise is injected into the template.

# Template Resources

[`markdowns/welcome.md`](https://github.com/TechDotIO/nodejs-template/blob/master/markdowns/welcome.md)
What you are reading here is generated by this file. Tech.io uses the [Markdown syntax](https://tech.io/doc/reference-markdowns) to render text, media and to inject programming exercises.


[`nodejs-project`](https://github.com/TechDotIO/nodejs-template/tree/master/nodejs-project)
A simple Nodejs project dedicated to run the programming exercise above. A project relies on a Docker image to run. You can find images on the [Docker Hub](https://hub.docker.com/explore/) or you can even [build your own](https://tech.io/doc/reference-runner).


[`techio.yml`](https://github.com/TechDotIO/nodejs-template/blob/master/techio.yml)
This *mandatory* file describes both the table of content and the programming project(s). The file path should not be changed.