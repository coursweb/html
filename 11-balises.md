---
layout: page
title: Balises essentielles
permalink: balises.html
---

Liste des balises HTML essentielles à connaître.

## Eléments de structure d'un document

Éléments de structure sémantique introduits avec HTML5:

-----|-----:
`<section>` | Définit une section dans un document
`<article>` | Définit un article (un contenu indépendant)  
`<h1> - <h6>` | Définit un titre, sous-titre ou inter-titre (*headings*).
`<header>` | Définit l'en-tête d'un document ou d'une section
`<footer>` | Définit le pied d'un document ou d'une section 
`<main>` | Désigne le contenu principal d'un document 
`<nav>` | Définit un menu de navigation  
`<aside>` | Définit un contenu annexe

Éléments de structure génériques:

-----|-----:
`<div>` | Définit une section dans un document (formaté en display:block).
`<span>` | Définit une section dans un document (formaté en display:inline).

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
`<ul>` | Defines an unordered list
`<li>` | Defines a list item


Balises de médias
===

Balises pour les images

-----|-----:
`<img>` | Définit une image
`<picture>` | Un contenur d'image pouvant inclure différentes variantes – [W3C](http://w3c.github.io/html/semantics-embedded-content.html#the-picture-element) / [caniuse](http://caniuse.com/#search=picture) / [MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/picture)
`<figure>` | Permet de grouper une image avec la légende qui l'accompagne
`<figcaption>` | Permet de définir une légende, à l'intérieur d'un élément `<figure>`

Balises pour les médias

-----|-----:
`<audio>` | Définit un contenu sonore.
`<video>` | Définit un contenu vidéo.
`<svg>` | Définit une image dans le format vectoriel SVG.
`<canvas>` | Conteneur pour des visuels codés en Javascript.


Balises générales ( méta-éléments)
===

Ces balises se situent avant le contenu:

-----|-----:
`<!DOCTYPE>` | Définit le type de document. Doit se trouver tout en début du code.
`<html>` | Définit la racine d'un document HTML. Englobe tout le document. 
`<head>` | Une section (invisible) en début de document, contenant des informations au sujet du document.
`<meta>` | Définit des métadonnes.
`<title>` | Définit le titre du document (affiché dans la barre du navigateur, pas dans le contenu de la page).
`<link>` | Définit une relation entre un document et une ressource externe (le plus souvent, des feuilles de styles CSS).
`<script>` | Définit un script qui sera exéctué par le navigateur.
`<style>` | Définit des styles pour le document.
`<!--...-->` | Définit un commentaire (code qui ne sera pas affiché).
`<body>` | Délimite le contenu visible du document.

## Ressources

- Information sur [les éléments les plus utilisés en 2005](https://web.archive.org/web/20131003124411/https://developers.google.com/webmasters/state-of-the-web/2005/pages), analyse statistique établie par Ian Hickson pour Google.
- [The Average Web Page](https://css-tricks.com/average-web-page-data-analyzing-8-million-websites/), analyse établie en 2016.