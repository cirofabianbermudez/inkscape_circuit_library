# inkscape_circuit_library
Repositorio para hacer circuitos de calidad utilizando Inkscape y Circuitikz

Para todos estos ejemplos se utilizó lo siguiente:
* [Inkscape 1.0](https://inkscape.org/release/inkscape-1.0/), software de vectores gráficos.
* [TextText](https://textext.github.io/textext/), complemento de Inkscape para renderizar LaTeX.
  * Recommended Install [GtkSourceview 3 for Inkscape 1.0 64-bit](https://github.com/textext/gtksourceview-for-inkscape-windows/releases/download/1.0.0/Install-GtkSourceView-3.24-Inkscape-1.0-64bit.exe).
* [TeX Live](http://mirrors.ibiblio.org/CTAN/systems/texlive/Images/), distrubución de LaTeX multiplataforma.

Circuitikz es un paquete que te permite realzizar circuitos de calidad en LaTeX, sin embargo su utilización no es sencilla,
tiene una curva de aprendizaje grande y se requiere de bastante código para poder hacer circuitos sencillos.

Utilizando Inkscape en combinación con Circuitikz este problema desaparece porque se pueden realizar las conexiones de manera muy rápida
y editar los componente como se desee.

Es importante saber utilizar lo básico de Inkscape:
* Group                                         Ctrl + G
* Ungroup                                     Shift + Ctrl + G
* Object/Align and Distribute       Shift + Ctrl + A
* Object/Fill and Stroke                 Shift + Ctrl + F
  * Stroke style/Width: 0.127
* Enable snapping
* When scaling objects, scale the stroke width by the same proportion __disable__
* Extensions/Text/Text Text
  * Scale Factor 1.5
* Rotate 90° 
* Flip horizontally and vertically

Un tutorial muy bueno y completo para aprender Inkscape es el siguiente:
[TJ FREE Inkscape Tutorial](https://www.youtube.com/watch?v=8f011wdiW7g&list=PLqazFFzUAPc5lOQwDoZ4Dw2YSXtO7lWNv&ab_channel=TJFREE)

Este es un ejemplo del resultado final que se puede obtener:

![Ejemplo](images/super_mesh.png)


La idea general de esta etodología de trabajo es la siguiente:
* Abrir Inkscape
* Abrir la carpeta __inkscape_library__
* Arrastar los compenentes necesarios
  * Colocarlos donde se desee
  * Conectarlos utilizando la herramienta __Draw Bezier curves and straight lines__
* Con Text Text poner el texto en LaTeX

