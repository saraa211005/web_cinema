# Cinesa: Blog de Pel·lícules

**Projecte de Producció i Disseny Cartogràfic** **Autora:** Sara Laguna Del Puerto  
**Curs:** 2025-2026

---

## Tema i motivació
**Cinesa** és un blog cinematogràfic creat amb l'objectiu de guiar els espectadors a l'hora de triar quina pel·lícula veure. La web conté crítiques, recomanacions i informació sobre l'actualitat del cinema.

El projecte té un clar **vincle amb la geografia** mitjançant la cartografia interactiva. No només es recomana què veure, sinó que es facilita la localització física de les sales de cinema de la província de Tarragona i la planificació de sortides a festivals locals (com l'Altafulla International Film Festival).

## Dades i Recursos
Per a la realització del projecte s'han utilitzat les següents fonts i tecnologies:
* **Fonts d'informació:** Crítiques de redacció pròpia, dades d'ubicació de cinemes de Tarragona i sinopsis i informació de fitxes tècniques de la web filmaffinity.
* **Recursos visuals:** Imatges i cartells obtinguts de repositoris digitals i Pinterest. També videos recuperats de youtube.
* **Tecnologies:** HTML5, CSS3 (ús intensiu de **Grid Layout**) i JavaScript.
* **Cartografia:** Biblioteca de codi obert [Leaflet.js](https://leafletjs.com/).

## Estructura de la Web
La web es divideix en 6 seccions principals:
1.  **Inici (`index.html`):** Presentació i recomanacions destacades com *Whiplash* o *El viatge de Chihiro*.
2.  **Informació (`infogeneral.html`):** Explicació del funcionament del blog, qui sóc i una guia visual de valoració per estrelles.
3.  **Galeria (`galeria.html`):** Recull visual de portades organitzades per gèneres (Terror, Aventura, Drama, Animació, etc.).
4.  **Mapa (`mapacine.html`):** Mapa interactiu amb marcadors dels cinemes de la zona.
5.  **Sortides (`sortides.html`):** Espai dedicat a esdeveniments culturals itinerants amb rutes cartografiades.
6.  **Contacte (`contacte.html`):** Formulari complet per rebre feedback i preferències dels usuaris.

## Ús de Bootstrap 5.3.8 (Exemples i Plantilles)
Per agilitzar el desenvolupament i assegurar un disseny professional i coherent, el projecte ha integrat i personalitzat diversos exemples oficials del framework **Bootstrap 5.3.8**, adaptant-los a les necessitats temàtiques del blog:

* **Plantilla "Blog":** Ha servit com a estructura principal de la web (especialment a l'`index.html` i `mapes.html`). D'aquí s'ha aprofitat la capçalera (header) amb la tipografia *Playfair Display*, la barra de navegació desplaçable (nav-scroller) per a les categories de cinema, i l'estructura de "Featurettes" (blocs on alternen text i imatge/mapa) per presentar el contingut de forma visualment atractiva. L'arxiu `blog.css` dona la identitat visual corporativa a tota la pàgina.
* **Plantilla "Album":** S'ha utilitzat a la secció de **Galeria** (`galeria.html`) per estructurar l'aparador de les pel·lícules. L'ús de les targetes ("Cards") d'aquest exemple ha estat ideal per mostrar de forma ordenada els cartells, les sinopsis, la valoració per estrelles i els botons d'acció (com l'enllaç al tràiler), aprofitant la quadrícula que s'adapta a qualsevol pantalla.
* **Plantilla "Checkout":** S'ha implementat i transformat a la pàgina de **Contacte** (`contacte.html`). Tot i ser un disseny originalment pensat per a passarel·les de pagament, s'ha aprofitat la seva sòlida estructura de formularis amb validació de dades. Els camps de targeta de crèdit s'han substituït per motius de contacte i àrees de missatge, i l'espai lateral del "carret de la compra" s'ha reconvertit en un útil panell informatiu amb les dades de contacte i les xarxes socials del blog. L'arxiu `checkout.css` assegura que el formulari quedi ben centrat.

## Disseny Web Responsive
S'ha aplicat un disseny adaptatiu per garantir que la web es vegi correctament en qualsevol dispositiu (mòbil, tauleta o PC):
* **CSS Grid:** S'utilitzen columnes flexibles que es reordenen automàticament.
* **Media Queries:** S'han definit punts de ruptura a `1024px` i `768px` per modificar el layout.
* **Imatges:** Gestió de l'alçada fixa (`height`) i `object-fit: cover` a la galeria per mantenir l'harmonia visual sense deformar els cartells.
* **Accessibilitat:** Menú desplegable lateral (hamburger menu) per a mòbils i contrastos de color (rosa sobre negre) per a una lectura clara.

## Cartografia
La integració cartogràfica s'ha realitzat mitjançant **Leaflet**:
* **Mapes de cinemes:** Inclouen popups personalitzats amb informació sobre la direcció, el pàrquing, l'accessibilitat i imatges reals de cada establiment.

* **Mapa sortida a Altafulla:** Inclou popus en els punts de trobada i informació addicional útil per al dia de la sortida (Hora de sortida de l'autobús, direcció concreta dels punts de trobada...)

## Dificultats i Millores
* **Dificultats:** Els reptes principals han estat la configuració dels popups de Leaflet per a que fossin responsius i la coordinació dels elements del formulari de contacte en pantalles petites. 
He tingut problemes a l'hora de treballar amb qgis2web ja que quan volís visualitzar la meva composició només hem deixaba treballar amb la línea (la ruta) i no hem permetía veure ni els punts, ni els popup.  

Fer la web responsiva també m'ha suposat un repte perque molts cops no aconseguía els resultats que esperaba. Amb l'ajut de la ia he pogut millorar aquests aspectes però encara falta millora.

* **Millores futures:** * 
    * Millorar el disseny responsive.
    * Possibilitat que els usuaris puguin puntuar directament les pel·lícules des de la web i a poder ser, crear un espai d'interacció social on la gent pugui pubicar les seves recomanacions i critiques.
    * Afegir el mapa a partir de qgis2web amb la ruta ben delimitada acord amb el recorregut del       autobús.

---
*Facultat de Turisme i Geografia - Universitat Rovira i Virgili*