#jquery-eyes-follow-mouse

Een demo van een jQuery-plugin waarmee de ogen op een pagina de muisbewegingen volgen.
Voorbeeld

Je kunt de demo bekijken op deze pagina.
Gebruik

Om deze plugin in je eigen project te gebruiken, kun je de volgende stappen volgen:

    Download de jquery.eyes-follow-mouse.js-bestand en voeg deze toe aan de scripts-map van je project.
    Voeg de demo.css-bestand toe aan de styles-map van je project.
    Voeg de volgende code toe aan de head-sectie van je HTML-pagina:

html

<link rel="stylesheet" type="text/css" href="styles/demo.css">
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="scripts/jquery.eyes-follow-mouse.js"></script>

    Voeg de volgende HTML-code toe aan de body-sectie van je pagina:

html

<div class='eyes'>
  <div class="eye">
    <span class="eye-lash up"></span>
    <span class="eye-retina"></span>
    <span class="eye-lash down"></span>
  </div>
  <div class="eye">
    <span class="eye-lash up"></span>
    <span class="eye-retina"></span>
    <span class="eye-lash down"></span>
  </div>
</div>

    Initialiseer de plugin door de volgende code toe te voegen aan je JavaScript-bestand:
    
//Eyes
const retina = $(".eye-retina");
const button = $(".eyes");

$(document).mousemove((e) => {
    e = e || window.event;

    //Offset of button from document
    const rect = button[0].getBoundingClientRect();
    const offsetLeft = rect.left + window.pageXOffset;
    const offsetTop = rect.top + window.pageYOffset;

    //Position of cursor in pixel
    const pageX = e.pageX;
    const pageY = e.pageY;

    //Cursor left position relative to button
    let left = (pageX - offsetLeft) / rect.width * 100;

    //Cursor top position relative to button
    let top = (pageY - offsetTop) / rect.height * 100;

    //Prevent the eye from getting hidden at the left and right end.
    left = left < 25 ? 25 : left;
    left = left > 75 ? 75 : left;

    //Prevent the eye from getting hidden at the top and bottom end.
    top = top < 25 ? 25 : top;
    top = top > 75 ? 75 : top;

    //Move the eye
    retina.each((i, f) => {
        //If the cursor is in center of both the eyes the keep the eye in center
        f.style.left = `${left > 45 && left < 55 ? 50 : left}%`;
        f.style.top = `${top > 45 && top < 55 ? 50 : top}%`;
    });
});
    
