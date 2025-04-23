Om HTML-elementen met behulp van CSS weer te geven of te verbergen, kun je de eigenschap display gebruiken. Er zijn verschillende waarden voor de display-eigenschap die je kunt gebruiken:

- In je CSS stylesheet kun je `display: none;` gebruiken. Deze waarde verbergt het element volledig, en het neemt geen ruimte in beslag op de pagina.

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

Vervolgens kun je in je HTML-bestand de klasse toepassen op de elementen die je wilt verbergen.

--- code ---
---
language: html
filename: 
line_numbers: true
---
    
    <div class="hide">Dit element is verborgen.</div>

--- /code ---

- Om een element weer te geven, kun je ook een selector in jouw CSS-stylesheet maken en de eigenschap `display: block;` gebruiken.

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
    display: block; /* of inline, inline-block, etc. */
}

--- /code ---

--- code ---
---
language: html
filename: 
line_numbers: true
---
    
    <div class="hide">Dit element is in eerste instantie verborgen.</div>
    <div class="show">Dit element is in eerste instantie zichtbaar.</div>

--- /code ---

- Je kunt ook JavaScript gebruiken om de zichtbaarheid van een HTML-element in of uit te schakelen. Hierdoor verschijnt en verdwijnt het.

--- code ---
---
language: js
filename: 
line_numbers: true
---
    
var element = document.querySelector(#myElement);

// Om het element te verbergen
element.style.display = "none";

// Om het element weer te geven
element.style.display = "block";

--- /code ---
