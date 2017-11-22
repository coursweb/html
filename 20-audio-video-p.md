---
layout: page
title: Audio, Video, Images
permalink: /html/audio-video-images/
---

Les balises image, picture, figure, audio et video

La balise image est proposée par Marc Andreessen [sur la liste de discussion "WWW-Talk"](http://1997.webhistory.org/www.lists/www-talk.1993q1/0182.html) le 25 février 1993 (il est alors étudiant à l'université d'Illinois, âgé de 22 ans).

```
I'd like to propose a new, optional HTML tag:
IMG
Required argument is SRC="url". 
This names a bitmap or pixmap file for the browser to attempt to pull
over the network and interpret as an image, to be embedded in the text
at the point of the tag's occurrence.
An example is:
<IMG SRC="file://foobar.com/foo/bar/blargh.xbm"> 
```

Voici un exemple simple de balise image:

```html
<img src="images/fichier.jpg" alt="description de l'image" height="42" width="42">
```

### Compression d'images

Il est nécessaire de compresser les images utilisées sur le web, afin d'optimiser la vitesse de chargement.

Un utilitaire pour obtenir des compressions maximales: [ImageOptim](https://imageoptim.com/fr), une application MacOS gratuite et open-source. ImageOptim permet notamment de réduire le poids des images PNG, pour lesquelles des applications comme Photoshop n'offrent pas de réglages de compression. Les images PNG sont ainsi réduites d'un tiers de leur taille en moyenne.

![Statistiques de compression dans ImageOptim](/cours-html/img/ImageOptim-stats.png)

### Propriété CSS utile: object-fit

Une propriété CSS longtemps attendue, qui permet de spécifier comment une image (ou vidéo) doit s'adapter à son conteneur. 

Les valeurs possibles sont: 

* `fill` : déformation de l'image, pour remplir le cadre à tout prix.
* `contain` : essaie de remplir le cadre tout en gardant toute l'image visible, en la rapetissant s'il le faut.
* `cover` : masquage partiel de l'image, pour remplir entièrement le cadre, sans déformation.
* `scale-down` : l'image se rétrécit pour rentrer dans le cadre. Peut se comporter comme contain.
* `none` : comportement classique, affichage de l'image à taille réelle des pixels.

Exemples : 

* [Un exemple conçu par Jen Simmons](http://labs.jensimmons.com/2016/examples/grace-hopper-page.html).
* [Exemple sur Mozilla.org](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit)

Support navigateurs: cette propriété n'est pas supportée dans Internet Explorer, elle sera dans Edge dès la version 16. [Voir Caniuse.com](http://caniuse.com/#search=object-fit) pour le statut actuel.


La balise Figure
===

Les balises `<figure>` et `<figcaption>` permettent de grouper une image avec sa légende (en anglais: *caption*).

Exemple d'utilisation:

~~~
<figure>
    <img src="monchat.jpg" alt="Un chat faisant la sieste.">
    <figcaption>Voici une photo de mon chat.</figcaption>
</figure>
~~~

Images responsives
===

`<picture>` ... élément permettant des images responsives, alternative à `<img>`.

Exemple de code:

~~~
<picture>
  <source 
    media="(min-width: 650px)"
    srcset="images/kitten-stretching.png">
  <source 
    media="(min-width: 465px)"
    srcset="images/kitten-sitting.png">
  <img 
    src="images/kitten-curled.png" 
    alt="a cute kitten">
</picture>
~~~

Et voici un autre exemple trouvé sur le site [sketchapp.com](https://www.sketchapp.com/features/). On notera qu'il utilise le format [WebP](https://fr.wikipedia.org/wiki/WebP), nouveau format compressé développé par Google.

~~~
<picture>
  <source 
   srcset="/images/features/mirror.webp 1x,
   /images/features/mirror@2x.webp 2x" 
   type="image/webp">
  <img src="/images/features/mirror-png8.png" 
   srcset="/images/features/mirror-png8@2x.png 2x">
</picture>
~~~

Enfin, une méthode trouvée sur [un site de Google](https://design.google.com/articles/introducing-pixate-and-form-1-3/) en novembre 2016: 

~~~
<div class="_image js-responsive-image loaded" 
  data-knowndimensions="1600x1050" 
  data-preserveaspectratio="true" 
  data-src="form.jpg" 
  data-target="#fig-2" 
  style="background-image: url(&quot;form-1240@2x.jpg&quot;);">
</div>
~~~

On notera qu'il n'y a pas de balise image (&lt;img&gt;), l'image est affichée comme image de fond en css (background-image). Son conteneur est un simple `<div>`.

## Références sur les images responsives

- [http://caniuse.com/#feat=picture](http://caniuse.com/#feat=picture)
- [https://github.com/scottjehl/picturefill - un polyfill]()
- [https://responsiveimages.org/](https://responsiveimages.org/)
