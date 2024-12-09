# Els llenguatges de Marques

##SVG (Scalable Vector Graphics)

**Elements:**

 `<svg>`, `<rect>`, `<circle>`, `<ellipse>`, `<line>`, `<polygon>`, `<polyline>`, `<path>`, `<text>`, `<g>`, `<use>`, etc.

**Etiquetes:**

 `<svg>`: És el contenidor principal de qualsevol gràfic SVG.

 `<rect>`: Dibuixa un rectangle.

 `<circle>`: Dibuixa un cercle.

 `<ellipse>`: Dibuixa una el·lipse.

 `<line>`: Dibuixa una línia.

 `<polygon>`: Dibuixa un polígon amb múltiples vèrtexs.

 `<path>`: Dibuixa formes complexes mitjançant un conjunt de comandos.

 `<g>`: Agrupa elements SVG.


**Propietats:**

 
 ***width, height:*** Dimensions del contenidor SVG.

 ***x, i:*** Posició dels elements en l'espai.

 ***fill:*** Color de farciment.

 ***stroke:*** Color de la vora.

 ***stroke-width:*** Gruix de la línia.

 ***transform:*** Aplica transformacions (translació, rotació, escala).

 ***viewBox:*** Definix l'àrea visible del gràfic.

 **Espai de Noms:**

Quan un document SVG està incrustat dins d'un document HTML o XML, l’espai de noms és necessari per a identificar clarament els elements SVG. Ací tens un exemple d'un espai de noms en SVG:

xml

`<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <!-- Dibuixos SVG ací --> </svg>`

    xmlns="http://www.w3.org/2000/svg": Defineix que els elements dins del contenidor <svg> pertanyen a l’espai de noms SVG estàndard.
    xmlns
    ="http://www.w3.org/1999/xlink": Defineix l’espai de noms per a l'atribut xlink, que s'utilitza en enllaços dins d'SVG.
 
 ---
 ---

##SGML (Standard Generalized Markup Language)

**Elements:**

SGML no definix elements específics com altres llenguatges. Proporciona una estructura per a definir altres llenguatges com a HTML i XML.

**Etiquetes:**

 No té etiquetes fixes. S'utilitza per a definir DTDs (Document Type Definitions) que especifiquen les etiquetes vàlides en un document SGML.

**Propietats:**

 ***DOCTYPE:*** Indica el tipus de document.

 ***PUBLIC:*** Definix la versió pública del document.

 ***SYSTEM:*** Definix la ubicació del DTD associat.

SGML és més una especificació per a la creació d'altres llenguatges basats en marques (com HTML o XML), per la qual cosa no té elements i propietats predefinits com a tals.

**Espai de Noms:**

Els espais de noms no s'utilitzen explícitament en SGML, però aquest llenguatge estableix la base per a llenguatges com XML, que sí que utilitzen espais de noms.

 ---
 ---

##HTML (HyperText Markup Language)

**Elements:**
 `<HTML>`, `<head>`, `<bodi>`, `<div>`, `<span>`, `<p>`, `<a>`, `<img>`, `<ul>`, `<li>`, `<table>`, `<tr>`, `<td>`, `<form>`, `<input>`, etc.

 **Etiquetes:**
 
 `<HTML>`: Contenidor principal del document HTML.

 `<head>`: Conté metadades, scripts i enllaços a fulls d'estil.

 `<bodi>`: Conté el contingut visible de la pàgina web.

 `<p>`: Definix un paràgraf.

 `<a>`: Definix un enllaç.

 `<img>`: Definix una imatge.

 `<div>`: Definix un contenidor de bloc.

 `<span>`: Definix un contenidor en línia.

**Propietats:**

 ***aneu:*** Identificador únic d'un element.

 ***class:*** Classe per a agrupar diversos elements amb el mateix estil.

 ***href:*** Atribut per a enllaços (en `<a>`).

 ***src:*** Atribut que definix la font d'una imatge (en `<img>`).

 ***alt:*** Text alternatiu d'una imatge.

 ***style:*** Definix estils CSS en línia.

 ***data:*** Atributs personalitzats per a emmagatzemar dades.

**Espais de Noms:**

En HTML5, no s'utilitzen espais de noms de la mateixa manera que en XML, però quan s'incrusten elements SVG o MathML, els espais de noms sí que són necessaris.

 ---
 ---

##XML (extensible Markup Language)
**Elements:**
 XML permet definir elements personalitzats. Alguns exemples d'etiquetes comunes en un arxiu XML podrien ser `<note>`, `<to>`, `<from>`, `<heading>`, `<bodi>`, encara que no estan predefinits.

**Etiquetes:**
 Les etiquetes en XML són definides per l'usuari o l'esquema del document. Cada etiqueta ha d'obrir-se i tancar-se: `<nom_etiqueta>`...`</nom_etiqueta>`.

**Espais de Noms:**

Els espais de noms en XML s'utilitzen per a identificar elements i evitar col·lisions de noms quan es combinen múltiples esquemes o llibreries. Exemple d'un espai de noms en XML:

xml

`<root xmlns="http://www.exemple.com/schema">
  <element>Contingut</element>
</root>`