Pour afficher ou masquer des éléments HTML à l'aide de CSS, tu peux utiliser la propriété display. Tu peux utiliser différentes valeurs pour la propriété display :

- Dans ta feuille de style CSS, tu peux utiliser `display: none;`. Cette valeur masque complètement l'élément, qui n'occupera aucun espace sur la page.

--- code ---
---
language: css
filename: 
line_numbers: true
---
    
.hide {
    display: none;
}
    
--- /code ---

Ensuite, dans ton fichier HTML, tu pourras appliquer la classe aux éléments que tu souhaites masquer.

--- code ---
---
language: html
filename: 
line_numbers: true
---
    
    <div class="hide">Cet élément est masqué.</div>

--- /code ---

- Pour afficher un élément, tu peux également créer un sélecteur dans ta feuille de style CSS et utiliser la propriété `display: block;`.

--- code ---
---
language: css
filename: 
line_numbers: true
---
    
.hide {
    display: none;
}

.show {
    display: block; /* ou inline, inline-block, etc. */
}

--- /code ---

--- code ---
---
language: html
filename: 
line_numbers: true
---
    
    <div class="hide">Cet élément est initialement masqué.</div>
    <div class="show">Cet élément est initialement visible.</div>

--- /code ---

- Tu peux également utiliser JavaScript pour activer/désactiver la visibilité d'un élément HTML. Cela le fera apparaître et disparaître.

--- code ---
---
language: js
filename: 
line_numbers: true
---
    
var element = document.querySelector(#myElement);

// Pour masquer l'élément
element.style.display = "none";

// Pour afficher l'élément
element.style.display = "block";

--- /code ---
