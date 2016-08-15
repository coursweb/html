---
layout: page
title: HTML
permalink: /html/
---

Introduction au HTML.

Ce support de cours donne une introduction au langage HTML.

Il vous aidera à: 

- Connaître les balises les plus utiles.
- Structurer vos documents HTML de manière sémantique.

Les balises
==

Le vocabulaire du langage HTML se compose de quelques 120 balises.

Quelques balises présentes depuis le début:

* L'hyperlien : `<a>`    
* Le titre : `<h1>` à `<h6>`    
* Le paragraphe : `<p>`

Un article au sujet des styles de liens:
[Signalétique des hyperliens](http://letrainde13h37.fr/43/signaletique-hyperliens/), par Romy Duhem-Verdière, 2013



## Les versions du langage HTML.

Durant ses 25 années d'existance, le standard HTML a connu diverses évolutions. La [première version](https://www.w3.org/History/19921103-hypertext/hypertext/WWW/MarkUp/Tags.html) proposée en 1991 comporte 18 éléments. Différentes versions du standard HTML sont publiées, jusqu'à la version HTML 4.0 en 1997. C'est en 1997 également que les feuilles de style CSS sont introduites.

S'ensuit une période de stagnation, durant laquelle le groupe de travail HTML du World Wide Web Consortium (W3C) focalise ses efforts sur un nouveau langage, le XHTML, qui s'avère une impasse.

En 2004, un groupe de travail "concurrent" se forme, nommé WHATWG (Web Hypertext Application Technology Working Group), rassemblant des représentants de Apple, Mozilla et Opera. Ce groupe élabore le futur standard HTML5 entre 2004-2007. En janvier 2008, la première spécification est publiée, qui est adoptée comme référence par le groupe de travail HTML du W3C.

## HTML5 ?

En 2010, les premiers éléments du HTML5 ont commencé à être supportés par les navigateurs, et des livres sur le HTML commencent à être publiés. Un logo officiel est dévoilé.

Ce n'est qu'en 2014 que le HTML5 devient une recommandation stable du W3C, alors que ses fonctionalités sont implémentées depuis longtemps dans les navigateurs.

Un article: [HTML5 et l’avenir du web](http://www.pompage.net/traduction/html5-et-le-futur-du-web), par Tim Wright, 2009

<h3>Balises structurantes</h3>

Les nouvelles balises structurantes du HTML5:

- header
- section
- article
- nav
- aside
- footer

Pourquoi on ne peut pas mettre de DIV dans un P
===

Historiquement, les éléments HTML peuvent se présenter de deux manières: sous forme de **bloc** ("block-level" elements) ou sous forme de **ligne** ("inline" elements). 

Un élément "bloc" va toujours occuper toute la largeur à disposition, contrairement à l'élément "ligne", qui se limite à la place nécessaire, et tolère des éléments voisins. 

Chaque élément possède un aspect par défaut, mais il est possible d'agir dessus avec la propriété CSS "display". On peut ainsi modifier simplement l'aspect d'un menu: en mode "display-bloc", ce sera un menu vertical. En mode "inline", cela devient un menu horizontal.

Avec HTML5, ce mode binaire se compléxifie, on se retrouve avec toute une liste de catégories de contenu: 

- **Flow content** - correspond de près au mode "block-level", et s'applique à la majorité des éléments. Notamment: div, article, blockquote, img, p...
- **Sectioning content** - les éléments qui définissent des sections: article, aside, nav, section
- **Heading content** - du contenu agissant comme en-tête: h1, h2, h3 etc.
- **Phrasing content** - le texte du document, tout ce qui peut être contenu dans un paragraphe, notamment: a, span
 
Là où cela devient important: certains éléments ne peuvent contenir que du "phrasing content". C'est le cas pour les balises `<p>` ou `<h1>`:  
 
 Plus d'informations dans [la spécification HTML](https://dev.w3.org/html5/spec-preview/content-models.html).