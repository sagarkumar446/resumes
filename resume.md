/_ Backbone CSS for Resume Template 1 _/

/_ Basic _/

#resume-preview [data-scope="vue-smart-pages"][data-part="page"] {
background-color: white;
color: black;
text-align: justify;
-moz-hyphens: auto;
-ms-hyphens: auto;
-webkit-hyphens: auto;
hyphens: auto;
}

#resume-preview p,
#resume-preview li,
#resume-preview dl {
margin: 0;
}

/_ Headings _/

#resume-preview h1,
#resume-preview h2,
#resume-preview h3 {
font-weight: bold;
}

#resume-preview h1 {
font-size: 2.13em;
}

#resume-preview h2,
#resume-preview h3 {
margin-bottom: 5px;
font-size: 1.2em;
}

#resume-preview h2 {
border-bottom-style: solid;
border-bottom-width: 1px;
}

/_ Lists _/

#resume-preview ul,
#resume-preview ol {
padding-left: 1.5em;
margin: 0.2em 0;
}

#resume-preview ul {
list-style-type: circle;
}

#resume-preview ol {
list-style-type: decimal;
}

/_ Definition Lists _/

#resume-preview dl {
display: flex;
}

#resume-preview dl dt,
#resume-preview dl dd:not(:last-child) {
flex: 1;
}

/_ Tex _/

#resume-preview :not(span.katex-display) > span.katex {
font-size: 1em !important;
}

/_ SVG & Images _/

#resume-preview svg.iconify {
vertical-align: -0.2em;
}

#resume-preview img {
max-width: 100%;
}

/_ Header _/

#resume-preview .resume-header {
text-align: center;
}

#resume-preview .resume-header h1 {
text-align: center;
line-height: 1;
margin-bottom: 8px;
}

#resume-preview .resume-header-item:not(.no-separator)::after {
content: " | ";
}

/_ Citations _/

#resume-preview [data-scope="cross-ref"][data-part="definitions"] {
padding-left: 1.2em;
}

#resume-preview [data-scope="cross-ref"][data-part="definition"] p {
margin-left: 0.5em;
}

#resume-preview [data-scope="cross-ref"][data-part="definition"]::marker {
content: attr(data-label);
}

#resume-preview [data-scope="cross-ref"][data-part="reference"] {
font-size: 100%;
top: 0;
}

/_ Dark & print mode _/
/_ You might want to comment out the following lines if you change the background or text color. _/

.dark #resume-preview [data-scope="vue-smart-pages"][data-part="page"] {
background-color: hsl(213, 12%, 15%);
color: hsl(216, 12%, 84%);
}

@media print {
.dark #resume-preview [data-scope="vue-smart-pages"][data-part="page"] {
background-color: white;
color: black;
}
}
