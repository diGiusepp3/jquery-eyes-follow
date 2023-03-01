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


////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Introduction

jquery-eyes-follow-mouse is a lightweight jQuery plugin that allows you to add eye-tracking effects to any element on your web page. With this plugin, you can define a 'watched' element and specify which elements within it should follow the mouse. The eyes smoothly track the mouse movement, even if it's outside the watched element.
Features

    Easy to use: simply include the plugin script and call the eyesFollowMouse() method on your target element(s).
    Customizable: adjust various settings, such as the size and color of the eyes, to fit your website's design.
    Lightweight: the plugin is only a few kilobytes in size and won't slow down your website's loading time.
    Cross-browser compatible: works on all major browsers, including Chrome, Firefox, Safari, and Internet Explorer.

Usage

To use jquery-eyes-follow-mouse, simply include the plugin script in your HTML file and call the eyesFollowMouse() method on your target element(s) using jQuery. For example:

javascript

$('.my-element').eyesFollowMouse();

You can also pass in an options object to customize the plugin's behavior. For a full list of available options and their default values, see the Options section below.
Options

jquery-eyes-follow-mouse supports several options that you can use to customize the plugin's behavior. To use these options, simply pass in an options object when calling the eyesFollowMouse() method on your target element(s). Here are the available options:

    eyeSize: the size of the eyes in pixels (default: 20)
    eyeColor: the color of the eyes (default: 'black')
    pupilSize: the size of the pupils in pixels (default: 6)
    pupilColor: the color of the pupils (default: 'white')
    watchedElement: the element to watch for mouse movement (default: the target element(s) passed to the eyesFollowMouse() method)
    watchedArea: the area within the watched element to track with the eyes (default: the entire watched element)

Examples

To see jquery-eyes-follow-mouse in action, check out the included demo.html file. This file contains several examples of how to use the plugin, along with explanations of the different options and their effects.
