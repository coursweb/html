---
layout: page
title: HTML
permalink: index.html
---

![](img/head-body-tag.jpg)

Ce support de cours a pour objectif de vous introduire au langage HTML.

Il vous aidera à: 

- Connaître les balises les plus utiles.
- Structurer vos documents HTML de manière sémantique.

Les balises
==

Le HTML n'est pas un langage de programmation, mais un langage de "marquage" (*markup* en anglais). Il permet de "baliser" un document afin de décrire sa structure.

Le vocabulaire du langage HTML se compose de quelques 120 balises. Il n'est pas nécessaire de les connaître intégralement, certaines étant très spécifiques (p.ex. les balises des tableaux, ou des formulaires).

Voici, pour commencer, les balises obligatoires pour un document HTML valide:

* `<html>` : C'est la racine du document, se trouvant au début et à la fin du code.
* `<head>` : L'en-tête, qui ne sera pas affiché, et contient diverses méta-informations (titre, auteur, mots-clés, liens vers des ressources à charger).
* `<title>` : C'est le titre document. Il ne sera pas affiché dans le contenu de la page, mais dans la barre du navigateur (et dans les résultats de recherche Google).
* `<body>` : Le corps du document. Tout le contenu visible se trouve dans cette balise.



* L'hyperlien - `<a>` - qui permet de pointer vers une autre ressource en ligne.     
* Les titres - `<h1>` à `<h6>` - permettant d'instaurer une structure interne à un document. Le H signifie *heading*.    
* Le paragraphe - `<p>` - qui identifie un paragraphe de texte.

Un exemple de balise hyperlien:

```html
<a href="http://example.com">Un Lien</a>
```

Voir la liste des [balises les plus essentielles](balises-essentielles.html).


### Balises structurantes

Les nouvelles balises structurantes du HTML5: 

- header  
- section
- article
- nav
- aside
- footer

Définitions:

- **header** = Section d'introduction d'un article, d'une autre section ou du document entier (en-tête de page).
- **section** = Section générique regroupant un même sujet, une même fonctionnalité, de préférence avec un en-tête, ou bien section d'application web.
- **article** = Section de contenu indépendante, pouvant être extraite individuellement du document ou syndiquée (flux RSS ou équivalent), sans pénaliser sa compréhension.
- **nav** = Section possédant des liens de navigation principaux (au sein du document ou vers d'autres pages).
- **aside** = Section dont le contenu est un complément par rapport à ce qui l'entoure, qui n'est pas forcément en lien direct avec le contenu, mais qui peut apporter des informations supplémentaires.
- **footer** = Section de conclusion d'une section ou d'un article, voire du document entier (pied de page).


## Pourquoi on ne peut pas mettre de DIV dans un P

Historiquement, les éléments HTML peuvent se présenter de deux manières: sous forme de **bloc** ("block-level" elements) ou sous forme de **ligne** ("inline" elements). 

Un élément "bloc" va toujours occuper toute la largeur à disposition, contrairement à l'élément "ligne", qui se limite à la place nécessaire, et tolère des éléments voisins. 

Chaque élément possède un aspect par défaut, mais il est possible d'agir dessus avec la propriété CSS "display". On peut ainsi modifier simplement l'aspect d'un menu: en mode "display-bloc", ce sera un menu vertical. En mode "inline", cela devient un menu horizontal.

Avec HTML5, ce mode binaire se complexifie, on se retrouve avec toute une liste de catégories de contenu: 

- **Contenu de flux (Flow content)** - correspond de près au mode "block-level", et s'applique à la majorité des éléments. Notamment: `<div>`, `<article>`, `<blockquote>`, `<img>`, `<p>`...
- **Contenu sectionnant (Sectioning content)** - les éléments qui définissent des sections: `<article>`, `<aside>`, `<nav>`, `<section>`
- **Contenu de titre (Heading content)** - du contenu agissant comme en-tête: `<h1>`, `<h2>`, `<h3>` etc.
- **Contenu phrasé (Phrasing content)** - le texte du document, tout ce qui peut être contenu dans un paragraphe, notamment: `<a>`, `<span>`. Correspond à peu près au mode "inline". Attention, `<a>` appartient à cette catégorie s'il contient *seulement* du contenu phrasé - sinon il devient Contenu de flux.
- **Contenu intégré** - `<audio>`, `<canvas>`, `<embed>`, `<iframe>`, `<img>`, `<math>`, `<object>`, `<svg>`, `<video>`...
- **Contenu interactif** - `<button>`, `<details>`, `<embed>`, `<iframe>`, `<keygen>`, `<label>`, `<select>`, et `<textarea>`.

Là où cela devient important: certains éléments ne peuvent contenir *que* du "phrasing content". C'est le cas pour les balises `<p>` ou `<h1>`.  
 
Plus d'informations: 
 
- [La spécification HTML](https://dev.w3.org/html5/spec-preview/content-models.html).
- *[Catégories de contenu](https://developer.mozilla.org/fr/docs/Web/HTML/Catégorie_de_contenu)*, documentation Mozilla Developer Network.
