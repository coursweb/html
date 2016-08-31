---
layout: page
title: Toutes les balises
permalink: /html/balises/
---

Liste des balises HTML disponibles

Balises générales
===

-----|-----:
`<!--...-->` | Defines a comment
`<!DOCTYPE>` | Defines the document type
`<base>` | Specifies the base URL/target for all relative URLs in a document  
`<head>` | Defines information about the document
`<html>` | Defines the root of an HTML document
`<iframe>` | Defines an inline frame
`<link>` | Defines the relationship between a document and an external resource (most used to link to style sheets)
`<meta>` | Defines metadata about an HTML document
`<noscript>` | Defines an alternate content for users that do not support client-side scripts
`<script>` | Defines a client-side script
`<style>` | Defines style information for a document  
`<title>` | Defines a title for the document

Eléments de structure d'un document
===

-----|-----:
`<body>` | Defines the document's body  
`<article>` | Defines an article  
`<aside>` | Defines content aside from the page content 
`<footer>` | Defines a footer for a document or section 
`<div>` | Defines a section in a document
`<h1>` to `<h6>` | Defines HTML headings
`<header>` | Defines a header for a document or section
`<hgroup>` | 
`<hr>` | Defines a thematic change in the content 
`<main>` | Specifies the main content of a document 
`<nav>` | Defines navigation links  
`<section>` | Defines a section in a document
`<span>` | Defines a section in a document

Balises de texte
===

-----|-----:
`<a>` | Defines a hyperlink  
`<abbr>` | Defines an abbreviation or an acronym  
`<address>` | Defines contact information for the author/owner of a document
`<b>` | Defines bold text
`<blockquote>` | Defines a section that is quoted from another source
`<bdi>` | Isolates a part of text that might be formatted in a different direction from other text outside it
`<bdo>` | Overrides the current text direction
`<br>` | Defines a single line break
`<cite>` | Defines the title of a work
`<code>` | Defines a piece of computer code
`<del>` | Defines text that has been deleted from a document
`<em>` | Defines emphasized text 
`<i>` | Defines a part of text in an alternate voice or mood
`<ins>` | Defines a text that has been inserted into a document
`<mark>` | Defines marked/highlighted text
`<p>` | Defines a paragraph
`<pre>` | Defines preformatted text
`<q>` | Defines a short quotation
`<s>` | Defines text that is no longer correct
`<samp>` | Defines sample output from a computer program
`<small>` | Defines smaller text
`<sub>` | Defines subscripted text
`<sup>` | Defines superscripted text
`<strong>` | Defines important text
`<time>` | Defines a date/time
`<u>` | Defines text that should be stylistically different from normal text
`<wbr>` | Defines a possible line-break

Listes, Définitions, etc
===

Balises pour les listes:

-----|-----:
`<ol>` | Defines an ordered list
`<ul>` | Defines an unordered list
`<li>` | Defines a list item
`<details>` | Defines additional details that the user can view or hide
`<summary>` | Defines a visible heading for a `<details>` element

Balises pour les définitions:

-----|-----:
`<dd>` | Defines a description/value of a term in a description list
`<dl>` | Defines a description list
`<dt>` | Defines a term/name in a description list
`<dfn>` | Represents the defining instance of a term

Balises de médias
===

-----|-----:
`<audio>` | Defines sound content
`<canvas>` | Used to draw graphics, on the fly, via scripting (usually JavaScript)
`<figure>` | Specifies self-contained content
`<figcaption>` | Defines a caption for a `<figure>` element
`<img>` | Defines an image
`<map>` | Defines a client-side image-map
`<source>` | Defines multiple media resources for media elements (`<video>` and `<audio>`)
`<svg>` | Fichier vectoriel SVG
`<track>` | Defines text tracks for media elements (`<video>` and `<audio>`)
`<video>` | Defines a video or movie

Formulaires, interactivité
===

-----|-----:
`<button>` | Defines a clickable button
`<fieldset>` | Groups related elements in a form
`<form>` | Defines an HTML form for user input
`<input>` | Defines an input control
`<kbd>` | Defines keyboard input
`<keygen>` | Defines a key-pair generator field (for forms)
`<label>` | Defines a label for an `<input>` element
`<legend>` | Defines a caption for a `<fieldset>` element
`<meter>` | Defines a scalar measurement within a known range (a gauge)
`<optgroup>` | Defines a group of related options in a drop-down list
`<option>` | Defines an option in a drop-down list
`<output>` | Defines the result of a calculation
`<param>` | Defines a parameter for an object
`<progress>` | Indique l'état d'avancement d'un travail (barre de progression). [support](http://caniuse.com/#feat=progress) dès IE10, Safari 6.
`<select>` | Defines a drop-down list
`<textarea>` | Defines a multiline input control (text area)
`<var>` | Defines a variable

Tableaux
===

-----|-----:
`<table>` | Définit un tableau. [W3C](https://www.w3.org/community/webed/wiki/HTML/Elements/table), 
`<tr>` | Définit un rang horizontal 
`<td>` | Définit une cellule 
`<th>` | Defines a header cell in a table  
`<caption>` | Représente le titre d'un tableau. [MDN](https://developer.mozilla.org/fr/docs/Web/HTML/Element/caption)  
 `<colgroup>` | Specifies a group of one or more columns in a table for formatting  
`<col>` | Specifies column properties for each column within a `<colgroup>` element 
`<thead>` | Regroupe l'en-tête d'un tableau  
`<tbody>` | Regroupe le corps d'un tableau
`<tfoot>` | Regroupe le pied d'un tableau. [W3C](https://www.w3.org/community/webed/wiki/HTML/Elements/tfoot). 

Balises récentes et expérimentales
===

-----|-----:
`<datalist>` | Specifies a list of pre-defined options for input controls
`<dialog>` | Defines a dialog box or window. Pas supporté par IE, Firefox, Safari.
`<menu>` | Defines a list/menu of commands
`<menuitem>` | Defines a command/menu item that the user can invoke from a popup menu

Autres balises
===

-----|-----:
`<area>` | Defines an area inside an image-map
`<embed>` | Defines a container for an external (non-HTML) application
`<object>` | Defines an embedded object
`<ruby>` | Defines a ruby annotation (for East Asian typography)
`<rp>` | Defines what to show in browsers that do not support ruby annotations
`<rt>` | Defines an explanation/pronunciation of characters (for East Asian typography)

Balises obsolètes
===

Balises qui ne sont plus supportées en HTML5:

-----|-----:
`<acronym>` | Use `<abbr>` instead. Defines an acronym.  
`<applet>` | Use `<embed>` or `<object>` instead. Defines an embedded applet (application Java).  
`<basefont>` | Use CSS instead. Specifies a default color, size, and font for all text in a document.  
`<big>` | Use CSS instead. Defines big text.  
`<center>` | Use CSS instead. Defines centered text.  
`<dir>` | Use `<ul>` instead. Defines a directory list. 
`<font>` | Use CSS instead. Defines font, color, and size for text.
`<frame>` | Defines a window (a frame) in a frameset.
`<frameset>` | Defines a set of frames.
`<noframes>` | Defines an alternate content for users that do not support frames. 
`<strike>` | Use `<del>` or `<s>` instead. Defines strikethrough text.  
`<tt>` | Use CSS instead. Defines teletype text.



