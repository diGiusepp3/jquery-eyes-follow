# jquery-eyes-follow

Dutch is on top, English is at the bottom

jquery-eyes-follow-mouse is een lichtgewicht plugin waarmee je eenvoudig oog-tracking effecten kunt toevoegen aan elk element op een webpagina. De plugin stelt je in staat om een 'gevolgd' element te definiëren en aan te geven welke elementen er binnenin moeten meebewegen met de muis. De ogen volgen de muisbeweging soepel, zelfs als deze zich buiten het gevolgde element bevindt. Perfect om persoonlijkheid toe te voegen aan het ontwerp van je website!

Installatie

    Download de jquery-eyes-follow-mouse plugin en sla het op in je project.

    Voeg de jQuery library toe aan je HTML bestand:

    html

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>

Voeg de jquery-eyes-follow-mouse plugin toe aan je HTML bestand:

html

<script src="jquery-eyes-follow-mouse.js"></script>

Initialiseer de plugin in je JavaScript bestand:

javascript

    $(".watched-element").eyesFollowMouse();

Gebruik

De plugin kan worden aangepast met een aantal opties:
Optie	Default waarde	Beschrijving
eyeSelector	".eye-retina"	Selector voor het oog element
centerSelector	null	Selector voor het centerpunt element. Als er geen centerpunt is opgegeven, zal het gevolgde element het centerpunt worden.
cursorXOffset	0	De horizontale offset van de cursorpositie in pixels.
cursorYOffset	0	De verticale offset van de cursorpositie in pixels.
minLeft	25	De minimum horizontale positie van het oog element in procenten.
maxLeft	75	De maximum horizontale positie van het oog element in procenten.
minTop	25	De minimum verticale positie van het oog element in procenten.
maxTop	75	De maximum verticale positie van het oog element in procenten.

Om jquery-eyes-follow-mouse in actie te zien, bekijk het meegeleverde demo.html bestand. Dit bestand bevat verschillende voorbeelden van hoe je de plugin kunt gebruiken, samen met uitleg over de verschillende opties en hun effecten.

///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


jquery-eyes-follow-mouse is a lightweight plugin that allows you to easily add eye-tracking effects to any element on a webpage. The plugin enables you to define a 'watched' element and specify which elements inside should move along with the mouse. The eyes smoothly follow the mouse movement, even when it's outside the watched element. Perfect for adding personality to your website design!

Installation

Download the jquery-eyes-follow-mouse plugin and save it in your project.

Add the jQuery library to your HTML file:

html

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
Add the jquery-eyes-follow-mouse plugin to your HTML file:

html

<script src="jquery-eyes-follow-mouse.js"></script>
Initialize the plugin in your JavaScript file:

javascript

$(".watched-element").eyesFollowMouse();

Usage

The plugin can be customized with a number of options:

Option Default Value Description
eyeSelector ".eye-retina" Selector for the eye element
centerSelector null Selector for the center point element. If no center point is specified, the watched element will be the center point.
cursorXOffset 0 The horizontal offset of the cursor position in pixels.
cursorYOffset 0 The vertical offset of the cursor position in pixels.
minLeft 25 The minimum horizontal position of the eye element in percentages.
maxLeft 75 The maximum horizontal position of the eye element in percentages.
minTop 25 The minimum vertical position of the eye element in percentages.
maxTop 75 The maximum vertical position of the eye element in percentages.

To see jquery-eyes-follow-mouse in action, check out the included demo.html file. This file contains several examples of how to use the plugin, along with explanations of the different options and their effects.
