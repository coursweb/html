---
layout: page
title: HTML
permalink: /html/
---

![](/cours-html/img/head-body-tag.jpg)

Ce support de cours a pour objectif de vous introduire au langage HTML.

Il vous aidera à: 

- Connaître les balises les plus utiles.
- Structurer vos documents HTML de manière sémantique.

Les balises
==

Le HTML n'est pas un langage de programmation, mais un langage de "marquage" (*markup* en anglais). Il permet de "baliser" un document afin de décrire sa structure.

Le vocabulaire du langage HTML se compose de quelques 120 balises.

Quelques balises présentes depuis le début:

* L'hyperlien - `<a>` - qui permet de pointer vers une autre ressource en ligne.     
* Le titre - `<h1>` à `<h6>` - permettant d'instaurer une structure interne à un document.    
* Le paragraphe - `<p>` - qui identifie un paragraphe de texte.

Un exemple de balise hyperlien:

```html
<a href="http://example.com">Un Lien</a>
```

Voir la liste de [toutes les balises](balises/).

Un article au sujet des styles de liens:
*[Signalétique des hyperliens](http://letrainde13h37.fr/43/signaletique-hyperliens/)*, par Romy Duhem-Verdière, le train de 13h37, 2013



## Les versions du langage HTML.

Durant ses 25 années d'existance, le standard HTML a connu diverses évolutions. La [première version](https://www.w3.org/History/19921103-hypertext/hypertext/WWW/MarkUp/Tags.html) proposée en 1991 comportait 18 éléments. Différentes versions du standard HTML sont publiées, jusqu'à la version **HTML 4.01** en 1999.

S'ensuit une période de stagnation, durant laquelle le groupe de travail HTML du World Wide Web Consortium (W3C) focalise ses efforts sur un nouveau langage, le **XHTML**, qui s'avère une impasse.

En 2004, un groupe de travail concurrent se forme, nommé **WHATWG** (Web Hypertext Application Technology Working Group), rassemblant des représentants de Apple, Mozilla et Opera. Ce groupe élabore le standard **HTML5** entre 2004-2007. En janvier 2008, la première spécification est publiée, qui est adoptée comme référence par le groupe de travail HTML du W3C.

![](/cours-html/img/standards-timeline-html.png)

## HTML5

Dès 2010, les premiers éléments du HTML5 ont commencé à être supportés par les navigateurs, et des livres sur le HTML commencent à être publiés. Un [logo officiel](https://www.w3.org/html/logo/), conçu par l'agence hawaïenne [Ocupop](http://ocupop.com/html5), est dévoilé en janvier 2011.

![Le logo HTML5](/cours-html/img/logo-html5.png)

Ce n'est qu'en 2014 que le HTML5 devient une recommandation stable du W3C, alors que ses fonctionnalités sont implémentées depuis longtemps dans les navigateurs.

En fin 2016, le W3C rend officielle la version HTML 5.1.

Actuellement, la spécification HTML est maintenue de manière parallèle par ces deux groupes de travail: 

- La spécification HTML du **W3C**: [https://w3c.github.io/html/](https://w3c.github.io/html/)
- La spécification HTML du **WHATWG**: [https://html.spec.whatwg.org/multipage/](https://html.spec.whatwg.org/multipage/)

> J'ai toujours dit que la standardisation au W3C, c'est de l'hémoglobine sur les murs dans une ambiance feutrée. – Daniel Glazman

**Références:**

- *[HTML5 et l’avenir du web](http://www.pompage.net/traduction/html5-et-le-futur-du-web)*, par Tim Wright, 2009
- *[The design of HTML5](https://adactio.com/articles/1704)*, présentation de Jeremy Keith, donnée à la conférence Fronteers 2010, Amsterdam.
- Un outil pour vérifer le support de votre navigateur: [http://html5test.com/](http://html5test.com/)

<h3>Balises structurantes</h3>

Les nouvelles balises structurantes du HTML5: 

- header  
- section
- article
- nav
- aside
- footer

Définitions:

- header = Section d'introduction d'un article, d'une autre section ou du document entier (en-tête de page).
- section = Section générique regroupant un même sujet, une même fonctionnalité, de préférence avec un en-tête, ou bien section d'application web.
- article = Section de contenu indépendante, pouvant être extraite individuellement du document ou syndiquée (flux RSS ou équivalent), sans pénaliser sa compréhension.
- nav = Section possédant des liens de navigation principaux (au sein du document ou vers d'autres pages).
- aside = Section dont le contenu est un complément par rapport à ce qui l'entoure, qui n'est pas forcément en lien direct avec le contenu mais qui peut apporter des informations supplémentaires.
- footer = Section de conclusion d'une section ou d'un article, voire du document entier (pied de page).


Pourquoi on ne peut pas mettre de DIV dans un P
===

Historiquement, les éléments HTML peuvent se présenter de deux manières: sous forme de **bloc** ("block-level" elements) ou sous forme de **ligne** ("inline" elements). 

Un élément "bloc" va toujours occuper toute la largeur à disposition, contrairement à l'élément "ligne", qui se limite à la place nécessaire, et tolère des éléments voisins. 

Chaque élément possède un aspect par défaut, mais il est possible d'agir dessus avec la propriété CSS "display". On peut ainsi modifier simplement l'aspect d'un menu: en mode "display-bloc", ce sera un menu vertical. En mode "inline", cela devient un menu horizontal.

Avec HTML5, ce mode binaire se complexifie, on se retrouve avec toute une liste de catégories de contenu: 

- **Contenu de flux (Flow content)** - correspond de près au mode "block-level", et s'applique à la majorité des éléments. Notamment: `<div>`, `<article>`, `<blockquote>`, `<img>`, `<p>`...
- **Contenu sectionnant (Sectioning content)** - les éléments qui définissent des sections: `<article>`, `<aside>`, `<nav>`, `<section>`
- **Contenu de titre (Heading content)** - du contenu agissant comme en-tête: `<h1>`, `<h2>`, `<h3>` etc.
- **Contenu phrasé (Phrasing content)** - le texte du document, tout ce qui peut être contenu dans un paragraphe, notamment: `<a>`, `<span>`. Attention, `<a>` appartient à cette catégorie s'il contient seulement du contenu phrasé - sinon il devient Contenu de flux.
- **Contenu intégré** - `<audio>`, `<canvas>`, `<embed>`, `<iframe>`, `<img>`, `<math>`, `<object>`, `<svg>`, `<video>`...
- **Contenu interactif** - `<button>`, `<details>`, `<embed>`, `<iframe>`, `<keygen>`, `<label>`, `<select>`, et `<textarea>`.

Là où cela devient important: certains éléments ne peuvent contenir *que* du "phrasing content". C'est le cas pour les balises `<p>` ou `<h1>`:  
 
Plus d'informations: 
 
- [La spécification HTML](https://dev.w3.org/html5/spec-preview/content-models.html).
- *[Catégories de contenu](https://developer.mozilla.org/fr/docs/Web/HTML/Catégorie_de_contenu)*, documentation Mozilla Developer Network.
