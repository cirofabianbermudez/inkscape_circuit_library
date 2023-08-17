# inkscape_circuit_library

## Overview

Este repositorio es una alternativa para hacer diagramas esquemáticos de circuitos eléctricos utilizando Inkscape y Circuitikz.

[Inkscape](https://inkscape.org/es/acerca-de/) es un software de vectores gráficos de calidad profesional para Windows, Mac OS X y GNU/Linux. Es usado por diseñadores profesionales y aficionados de todo el mundo para crear una gran variedad de gráficos como ilustraciones, iconos, logos, diagramas, mapas y diseños web. Inkscape es un software libre y de código abierto, que utiliza SVG (Scalable Vector Graphic), el estándar abierto de W3C, como formato nativo.

Circuitikz es un paquete que te permite realizar circuitos de calidad en LaTeX, sin embargo su utilización esta lejos de ser sencilla, tiene una curva de aprendizaje muy grande y se requiere de mucha codificación para poder hacer circuitos sencillos.

Utilizando Inkscape en combinación con Circuitikz se pueden realizar de manera muy sencilla todo tipo de circuitos eléctricos. Las ventajas de combinar estas dos herramientas son las siguientes:

- Se tiene acceso a todos los componentes de Circuitikz.
- Las conexiones entre componentes se realizan manualmente y sin esfuerzo.
- Se pueden exportar las imágenes terminadas como `.svg` ,`.eps`, `.png`, `.jpg`, `.pdf` entre otros.
- El tiempo de diseño es muy rápido.

## Instalación

Para poder utilizar la librería se requieren de las siguientes herramientas:
1. [TeX Live](http://mirrors.ibiblio.org/CTAN/systems/texlive/Images/), distribución de LaTeX multiplataforma.
2. [Inkscape 1.3](https://inkscape.org/release/inkscape-1.3/windows/64-bit/msi/?redirected=1), software de vectores gráficos.
3. [TexText 1.9](https://textext.github.io/textext/), complemento de Inkscape para renderizar LaTeX.
	- Recomendado instalar [GtkSourceview 3 for Inkscape 1.0 64-bit](https://github.com/textext/gtksourceview-for-inkscape-windows/releases/download/1.0.0/Install-GtkSourceView-3.24-Inkscape-1.0-64bit.exe).

> **Nota 1:** IInstalar TexText con el archivo `.bat` en Windows.
Es necesario desactivar las siguiente opciones:

- When scaling objects, scale the stroke width by the same proportion.
- When scaling rectangles, sclae the radii of rounded corners
- Move gradients (in fill or stroke) along with the objets.
- Move patterns (in fill or stroke) along with the objets.

## Atajos de Inkscape

Es importante saber utilizar lo básico de Inkscape, aquí hay una lista de los comandos y menús mas importantes:

|          Acción      			|        Atajo         	|
|-------------------------------|-----------------------|
|Group			 				|`Ctrl + g`      		|
|Ungroup         				|`Ctrl + Shift +  g`   	|
|Duplicate         				|`Ctrl + d`			   	|
|Copy         					|`Ctrl + c`			   	|
|Paste	         				|`Ctrl + v`			   	|
|Rotate	90° left   				|`Ctrl + [`			   	|
|Rotate	90° rigth 				|`Ctrl + ]`			   	|
|Flip vertically				|`h`			   		|
|Flip horizontally				|`v`			   		|


> **Note:** En los comandos **Flip** no es necesario apretar `Shift`.


## Menús
|         Menú      			|        Atajo    	 	|
|-------------------------------|-----------------------|
|Object/Align and Distribute 	|`Ctrl + Shift + a`		|
|Object/Fill and Stroke 	 	|` Ctrl + Shift + f`		|
|File/Document Properties	 	|`Shift + Ctrl + d`		|
|File/Document Properties/Resize to content 	|`Ctrl + Shift + r `	|

## Configuraciones extra

|         Configuración    		|        Descripción   	|
|-------------------------------|-----------------------|
|Stroke style/Width 												| Configurar a `0.141`				|
|Enable snapping		 	 										| Activar o desactivar con `%`		|
|When scaling objects, scale the stroke width by the same proportion| Esquina superior izquierda		|



Un excelente tutorial ara aprender Inkscape es el siguiente: [TJ FREE Inkscape Tutorial](https://www.youtube.com/watch?v=8f011wdiW7g&list=PLqazFFzUAPc5lOQwDoZ4Dw2YSXtO7lWNv&ab_channel=TJFREE)

Este es un ejemplo del resultado final que se puede obtener:

![Ejemplo](images/super_mesh.png)


La idea general de esta metodología de trabajo es la siguiente:
* Abrir Inkscape
* Abrir la carpeta __inkscape_library__
* Arrastar los compenentes necesarios
  * Colocarlos donde se desee
  * Conectarlos utilizando la herramienta **Draw Bezier curves and straight lines**
* Con TexText poner el texto en LaTeX

