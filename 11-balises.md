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
`<article>` | Définit un article (une section de contenu indépendante) ([MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/article))
`<h1> - <h6>` | Définit un titre, sous-titre ou inter-titre (*heading*). Permet d'instaurer une structure interne à un document.
`<header>` | Section d'introduction d'un article, d'une autre section ou du document entier (par exemple: en-tête de page)
`<footer>` | Section de conclusion d'une section ou d'un article, voire du document entier (par exemple: pied de page) 
`<nav>` | Une section destinée à la navigation, possédant des liens de navigation principaux (au sein du document ou vers d'autres pages)

Éléments de structure génériques:

-----|-----:
`<div>` | Définit une section dans un document (formaté en display:block).
`<span>` | Définit une section dans un texte (formaté en display:inline).

## Eléments de contenu

-----|-----:
`<a>` | Un hyperlien, avec l'attribut `href` indiquant la cible. Permet de pointer vers une autre ressource en ligne
`<p>` | Un paragraphe de texte 
`<em>` | Du texte avec "emphase", rendu en italique. 
`<strong>` | Du texte avec une importance forte, rendu en gras.
`<br>` | Un retour de ligne simple (line break).

Un exemple de balise hyperlien:

```html
<a href="https://example.com">Un Lien</a>
```

## Listes

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

## Balises de médias

Balises pour les images:

-----|-----:
`<img>` | Définit une image
`<picture>` | Un conteneur d'image pouvant inclure [différentes variantes](https://cours-web.ch/media/25-balise-picture.html) – [W3C](http://w3c.github.io/html/semantics-embedded-content.html#the-picture-element) / [MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/picture)
`<figure>` | Permet de [grouper une image](https://cours-web.ch/media/20-balise-figure.html) avec la légende qui l'accompagne
`<figcaption>` | Permet de définir une légende, à l'intérieur d'un élément `<figure>`

Balises pour les médias:

-----|-----:
`<audio>` | Définit un contenu sonore.
`<video>` | Définit un contenu vidéo.
`<svg>` | Définit une image dans le format vectoriel SVG.
`<canvas>` | Conteneur pour des visuels codés en Javascript.


## Balises générales ( méta-éléments)

Ces balises se situent avant le contenu. Certaines de ces balises sont obligatoires pour un document HTML valide:

-----|-----:
`<!DOCTYPE>` | Définit le type de document. Doit se trouver tout en début du code.
`<html>` | Définit la racine d'un document HTML. Englobe tout le document (au début et à la fin du code). 
`<html>` | C'est la racine du document, se trouvant au début et à la fin du code.
`<head>` | L'en-tête, qui ne sera pas affiché, et contient diverses méta-informations au sujet du document (titre, auteur, mots-clés, liens vers des ressources à charger).
`<title>` | C'est le titre document. Il ne sera pas affiché dans le contenu de la page, mais dans la barre du navigateur (et dans les résultats de recherche Google).
`<body>` | Le corps du document. Tout le contenu visible se trouve dans cette balise.

Eléments optionnels mais fréquents:

-----|-----:
`<meta>` | Définit des métadonnées.
`<link>` | Définit une relation entre un document et une ressource externe (le plus souvent, des feuilles de styles CSS).
`<script>` | Définit un script qui sera exéctué par le navigateur.
`<style>` | Définit des styles pour le document.
`<!--...-->` | Définit un commentaire (code qui ne sera pas affiché).

Exemple:

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page</title>
  <meta charset="utf-8">
  <meta name="description" content="A description of my page.">
  <link rel="stylesheet" href="style.css">
  <style>
    h1 { color: #424242; }
  </style>
  <script src="https://jquery.com/base.js"></script> 
</head>
<body>
  <!-- Ici commence le contenu de la page -->
  <h1>Welcome to my page!</h1>
</body>
</html>
```

## Ressources

Les balises essentielles ont été établies sur la base des analyses suivantes:

- Information sur [les éléments les plus utilisés](https://web.archive.org/web/20131003124411/https://developers.google.com/webmasters/state-of-the-web/2005/pages), analyse statistique établie par Ian Hickson pour Google en 2005, portant sur 1 milliard de sites.
- [The Average Web Page](https://css-tricks.com/average-web-page-data-analyzing-8-million-websites/), analyse établie en 2016, portant sur 8 millions de sites.

Selon l'analyse de 2016, les sites web utilisent en moyenne **26 éléments différents** (19 dans la statistique de 2005).
