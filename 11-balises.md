---
layout: page
title: Balises essentielles
permalink: balises-essentielles.html
---

Cette page présente une liste des balises HTML essentielles à connaître. Ce sont les plus fréquemment utilisées (selon les sources de données en bas de page).

## Eléments de structure

Éléments de structure sémantiques:

-----|-----:
`<section>` | Définit une section dans un document ([MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/section))
`<article>` | Définit un article (un contenu autonome) ([MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/article))
`<h1> - <h6>` | Définit un titre, sous-titre ou inter-titre (*headings*).
`<header>` | Définit l'en-tête d'un document ou d'une section
`<footer>` | Définit le pied d'un document ou d'une section 
`<nav>` | Définit une section destinée à la navigation 

Éléments de structure génériques:

-----|-----:
`<div>` | Définit une section dans un document (formaté en display:block).
`<span>` | Définit une section dans un texte (formaté en display:inline).

## Eléments de contenu

-----|-----:
`<a>` | Un hyperlien, avec l'attribut `href` indiquant la cible. 
`<p>` | Un paragraphe de texte 
`<em>` | Du texte avec "emphase", rendu en italique. 
`<strong>` | Du texte avec ume importance forte, rendu en gras.
`<br>` | Un retour de ligne simple (line break).


Listes, Définitions, etc
===

Balises pour les listes:

-----|-----:
`<ul>` | Définit une liste ("unordered list")
`<li>` | Définit un élément à l'intérieur d'une liste ("list item")

Exemple de navigation formatée avec les éléments NAV et UL : 

```html
<nav class="menu">
  <ul>
    <li><a href="#Accueil">Accueil</a></li>
    <li><a href="#Apropos">À propos</a></li>
    <li><a href="#Contact">Contact</a></li>
  </ul>
</nav>
```

Balises de médias
===

Balises pour les images

-----|-----:
`<img>` | Définit une image
`<picture>` | Un conteneur d'image pouvant inclure [différentes variantes](https://cours-web.ch/media/25-balise-picture.html) – [W3C](http://w3c.github.io/html/semantics-embedded-content.html#the-picture-element) / [MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/picture)
`<figure>` | Permet de [grouper une image](https://cours-web.ch/media/20-balise-figure.html) avec la légende qui l'accompagne
`<figcaption>` | Permet de définir une légende, à l'intérieur d'un élément `<figure>`

Balises pour les médias

-----|-----:
`<audio>` | Définit un contenu sonore.
`<video>` | Définit un contenu vidéo.
`<svg>` | Définit une image dans le format vectoriel SVG.
`<canvas>` | Conteneur pour des visuels codés en Javascript.


Balises générales ( méta-éléments)
===

Ces balises se situent avant le contenu.

-----|-----:
`<!DOCTYPE>` | Définit le type de document. Doit se trouver tout en début du code.
`<html>` | Définit la racine d'un document HTML. Englobe tout le document. 
`<head>` | Une section (invisible) en début de document, contenant des informations au sujet du document.
`<meta>` | Définit des métadonnées.
`<title>` | Définit le titre du document (affiché dans la barre du navigateur, pas dans le contenu de la page).
`<link>` | Définit une relation entre un document et une ressource externe (le plus souvent, des feuilles de styles CSS).
`<script>` | Définit un script qui sera exéctué par le navigateur.
`<style>` | Définit des styles pour le document.
`<!--...-->` | Définit un commentaire (code qui ne sera pas affiché).
`<body>` | Délimite le contenu visible du document.

Exemple:

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page</title>
  <meta name="description" content="A description of my page.">
  <style>
    h1 {
      color: #424242;
    }
  </style>
</head>
<body>
  <h1>Welcome to my page!</h1>
</body>
</html>
```

## Ressources

Les balises essentielles ont été établie sur la base des analyses suivantes:

- Information sur [les éléments les plus utilisés](https://web.archive.org/web/20131003124411/https://developers.google.com/webmasters/state-of-the-web/2005/pages), analyse statistique établie par Ian Hickson pour Google en 2005, portant sur 1 millard de sites.
- [The Average Web Page](https://css-tricks.com/average-web-page-data-analyzing-8-million-websites/), analyse établie en 2016, pourtant sur 8 millions de sites.