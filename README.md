# Cinesa - El teu Blog de Cinema

**Cinesa** és un projecte web interactiu dedicat al cinema, centrat en la publicació de crítiques cinematogràfiques, la visualització de cartelleres i la geolocalització de sales de cinema a la província de Tarragona.

Aquest projecte combina una estètica visual moderna amb funcionalitats avançades de cartografia i un disseny totalment adaptat a dispositius mòbils. A més de ser un espai d'interacció a través de la pantalla, també es busca una interacció social personal a través de sortides a cinemes a veure estrens o a festivals cinematogràfics.

El Blog neix de la passió personal pel cinema i de la voluntat d'unir el desenvolupament web amb la cartografia digital. La motivació principal ha estat crear una plataforma que no només serveixi com a diari de crítiques cinematogràfiques, sinó també com una eina útil per a la comunitat de la província de Tarragona. Mitjançant la integració de mapes interactius, l'objectiu és facilitar la descoberta de sales de cinema locals i fomentar l'interès per la cultura cinematogràfica des d'una vessant pràctica i visual.

## Característiques Detallades

### 1. Crítiques i Valoracions Personalitzades
* **Anàlisi de Contingut:** El lloc web presenta ressenyes aprofundides (com la d' *El viatge de Chihiro*) que inclouen una breu fitxa tècnica i comentaris personals, a més d'un enllaç que et permet veure el tráiler de la pel·lícula.
* **Sistema de Puntuació:** S'ha implementat un sistema visual de 5 estrelles (★☆☆☆☆) per categoritzar les pel·lícules des de "Dolenta" fins a "Mestra", permetent una comprensió ràpida de la qualitat de la pel·lícula.
* **Secció Pròximament:** Un espai dinàmic on s'anuncien les futures entrades del blog, generant expectació sobre nous cicles com el de Studio Ghibli.

### 2. Mapes Interactius (Geolocalització)
Utilitzant la llibreria **Leaflet.js**, el projecte ofereix una experiència geoespacial:
* **Mapa de Cinemes:** Localització exacta de cinemes de la província de Tarragona (Vilallonga del Camp, Montblanc, etc.) amb finestres emergents (*popups*) que mostren horaris, preus i fotos reals de les sales.
* **Rutes de Sortida:** Una funcionalitat específica per visualitzar rutes cinèfiles (ex: trajecte Tarragona - Altafulla) mitjançant línies de recorregut (*polylines*) personalitzades amb l'estil visual del web.

### 3. Galeria i Interactivitat
* **Mural de Portades:** Una galeria d'imatges (portades de pel·lícules) organitzada per gèneres que permet a l'usuari explorar visualment el contingut.
* **Formulari de Feedback:** Inclou controls avançats com barres de satisfacció, selectors de gèneres preferits i àrees de text per a recomanacions.
* **Navegació Millorada:** Incorporació d'un botó "Back to Top" amb JavaScript que apareix en fer *scroll*, facilitant el retorn a la part superior de la pàgina.

---

## Disseny Responsiu (Responsive Design)

El projecte s'ha construït sota la premisa de la comoditat i l'estilització, assegurant que la interfície sigui intuïtiva en qualsevol mida de pantalla.

### Menú Hamburguesa
En pantalles de mòbil o tauleta, el menú de navegació tradicional es transforma en un **menú lateral desplegable**.
* S'ha utilitzat la tècnica del `checkbox hack` (`#menu-toggle`) per controlar l'obertura i tancament del menú sense dependre exclusivament de JavaScript.

### Adaptabilitat del Contingut (Media Queries)
Mitjançant l'ús de CSS modern i punts de tall (*breakpoints*) a `768px`:
* **Graelles Flexibles:** Els elements de la galeria i les columnes dels formularis es reordenen automàticament de forma vertical en pantalles estretes per evitar el desplaçament horitzontal.
* **Imatges Fluides:** L'ús de `background-size: cover;` i `background-attachment: fixed;` permet que les imatges de fons mantinguin la seva qualitat i posició  en qualsevol resolució.
* **Tipografia Adaptada:** Les mides de font s'ajusten per mantenir la llegibilitat tant en monitors de sobretaula com en pantalles de telèfons intel·ligents.

---

## Tecnologies Utilitzades

* **HTML5:** Estructura base de la web i accessibilitat.
* **CSS3:** Disseny avançat amb degradats, animacions i *Media Queries*.
* **JavaScript:** Control de l'interactivitat (p.e. Tornar a dalt).
* **Leaflet API:** Motor de mapes interactius.
* **Google Fonts:** Tipografies *Playfair Display* (elegància) i *Montserrat* (modernitat).

## Estructura de Fitxers

* `index.html` - Pàgina principal i crítiques.
* `infogeneral.html` - Sistema de puntuació i horaris.
* `galeria.html` - Mural visual de pel·lícules.
* `mapacine.html` - Mapa de cinemes de Tarragona.
* `sortides.html` - Traçat d'una ruta cinèfila.
* `contacte.html` - Formulari d'opinió.
* `estils.css` - Full d'estils centralitzat i responsive.

## Autora
Creat per **Sara Laguna** (2026).

---
*Aquest projecte ha estat creat amb finalitats acadèmiques/personals per explorar el desenvolupament web. S'ha desenvolupat en el marc de l'assignatura de **Producció i Disseny Cartogràfic** a la Universitat Rovira i Virgili.*
