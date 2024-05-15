---
layout: page
title: FAQ
permalink: faq.html
---

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
