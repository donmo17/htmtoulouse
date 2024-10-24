# HTML / CSS - Progression

## Progression

### mardi 30.04.2024

> **MATIN : 9h00 - 13h00**

- Chaque apprenant présente son parcours académique / professionnel
- Envoi d'un de partage au nuage Pcloud dans lequel les apprenants retrouveront en temps réel tous les enseignements dipensés
- Configuration Visual Studio Code (settings, extensions ...)
- Bases du HTML

  - historique
  - syntaxes des balises
  - titres (h1, h2, ...)
  - paragraphes
  - hr, br, mark, blockquote

- Mise en forme du texte
  - b, strong, sub, sup
- Listes
  - ul, ol, li
- Bloc de contenu

  - inline (span, img ...)
  - block (div, p, ...)

- Balises sémantiques

  - header, nav, main, section, article, aside, footer

- Images
  - formats (jpeg, jpg, png, svg)
  - attribut "alt" et "title"
  - figure et figcaption

* Présentation de la syntaxe **EMMET** afin de coder plus simplement et rapidement.
* Raccourcis Visual Studio Code pour faciliter le codage

* **EXERCICE (live-coding en groupe)** : `template.html`
  - **reset**
    - codage d'un reset css utile pour tous nos projets
    - notion d'unité `rem`

```css
*,
::before,
::after {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
  /*62.5 * 16 / 100 = 10px */
  scroll-behavior: smooth;
}
```

> **APRES-MIDI : 14h00 - 17h00**

- **EXERCICE (suite et fin du live-coding en groupe)** : `template.html`

  - **Accessibilité web**

    - attribut `role`
    - attribut `tabindex`
    - structure de la page web avec des balises sémantiques :
      - `header,` `nav`,
      - `main`, `article`, `section`, `aside`
      - `footer`

  - **Utilisation de sélecteurs CSS**

    - `elements`

    - `first-child`

    - `nth-child()`

  - **Recours aux boîte flexibles (Flexbox)**
    - `display: flex`
    - `flex: 1 1 auto`
    - `justify-content`
    - `aligns-items`

### jeudi 02.05.2024

**MATIN : 9h00 - 13h00**

- complément d'information sur l'accessibilité
  - `tabindex="0"`

- **Positionnement**
  - **EXERCICE (positionnement)** : `introduction/position.html`
    - `position: static`
    - `position: relative`
    - `position: absolute`
    - `position: fixed`
    - `position: sticky`

- **Pseudo-éléments** 
  - **EXERCICE (pseudo-éléments)** : `introduction/pseudo_element.html`
    - `::before`
    - `::after`

- Synthèse position + pseudo élément
  - **EXERCICE ** : `introduction/google.html`
    - codage du logo GOOGLE en HTML + CSS

**APRES-MIDI : 14h00 - 17h00**

* Codage de composants d'interface en Flexbox
  * **EXERCICE ** : `FLEXBOX/COMPOSANTS/team.html`
    - codage d'un composant affichant une équipe de travail
* Présentation de la méthodologie `BEM` (**Block Element Modifier**)
  * **EXERCICE ** : `FLEXBOX/COMPOSANTS/hero.html`
    - codage d'un **"hero"** (grand bandeau affiché juste après une barre de navigation sur un site web)
    - application de la méthodologie BEM pour le coder.


### vendredi 03.05.2024

> **MATIN : 9h00 - 13h00**

- Transitions et Transformations 2D et 3D en CSS
  - Appliqué la propriété `transform` **à l'état d'origine** et non `:hover`
  - **EXERCICE ** : `TRANSFORMATIONS/2D/2D.html`
    - rotation, scale, skew, translation
  - **EXERCICE ** : `TRANSFORMATIONS/3D/3D.html`
    - flip d'une div HTML
    - recours à `backface-visibility`

* Grilles CSS (CSS Grid)
  * Définition d'une grille
    * `display: grid;`
  * Grille explicite et implicite
    * **EXERCICE ** : `GRID/GRID_INTRO/grid_intro.html`
      - `grid-template-columns: 100px 1fr 2fr`
      -  `grid-template-columns: repeat(3, 1fr)`
      - `grid-template-rows: 80px 100px`
      -   `grid-auto-rows: auto`

> **APRES-MIDI : 14h00 - 17h00**

* Zones de grille (différentes syntaxe d'utilisation)
  * `grid-row : 2 / 3`
  * `grid-column : 3 / -1`
  * `grid-template-areas`

* Codage de layouts
  * **EXERCICES ** : `GRID/GRID_LAYOUTS/`
    * **layout_1.html** : mise en page de site web classique
    * **layout_2.html** : idem que **layout_1.html** mais avec `grid-template-areas`
    * **layout_3.html** : subgrid, grille imbriquée

* Grille CSS **auto-responsives** :
  * `auto-fit`
  * `auto-fill`
  * `grid-template-columns: repeat(auto-fit, minmax(100px, 1fr))`

* Fusion de cellules de grille
  *   `grid-row: span 2;`
  *   `grid-column: span 2;`
  *   grid-row: span 2;
  * **EXERCICE ** : `GRID/GALLERIY/grid-gallery.html`
    * codage d'un galerie en grille CSS
    * 


### lundi 06.05.2024

> **MATIN : 9h00 - 13h00**





> **APRES-MIDI : 14h00 - 17h00**







### mardi 07.05.2024

> **MATIN : 9h00 - 13h00**

* SASS

  * comparaison code SASS, SCSS, CSS

  * installation de l'extension `Live Sass Compiler` dans Visual Studio Code

    * paramétrage

    ```json
    "liveSassCompile.settings.formats": [
        {
          // Format can be _expanded_, _compact_, _compressed_ or _nested_. _Default is expanded._
          "format": "expanded",
          // Extension Name can be .css or .min.css. Default is .css.
          "extensionName": ".css",
          "savePath": "~/../css"
        }
      ],
    "liveSassCompile.settings.generateMap": false,
    "liveSassCompile.settings.autoprefix": []
    ```

  * variables SCSS

  * **nesting**

  * **mixins**

  * **pratials**

* **EXERCICES ** : `SASS/`

  * `sass_variables.scss` : couleur de fond, couleur de texte
  * `sass_nestins.scss` : ul > li > a
  * `sass_mixin.scss` : paramétrages de boutons
  * `sass_card.scss` : codage d'un système de cards
  * `sass_import.scss` : import de partials

> **APRES-MIDI : 14h00 - 17h00**







## FIN

Fin du document
