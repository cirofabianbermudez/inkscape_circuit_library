# inkscape_circuit_library
Repositorio para hacer circuitos de calidad utilizando Inkscape y Circuitikz

Para poder utilizar la librería se requieren de las siguientes herramientas
1. [Inkscape 1.0](https://inkscape.org/release/inkscape-1.0/), software de vectores gráficos.
2. [TexText](https://textext.github.io/textext/), complemento de Inkscape para renderizar LaTeX.
	- Recomendado instalar [GtkSourceview 3 for Inkscape 1.0 64-bit](https://github.com/textext/gtksourceview-for-inkscape-windows/releases/download/1.0.0/Install-GtkSourceView-3.24-Inkscape-1.0-64bit.exe).
3. [TeX Live](http://mirrors.ibiblio.org/CTAN/systems/texlive/Images/), distrubución de LaTeX multiplataforma.

Circuitikz es un paquete que te permite realzizar circuitos de calidad en LaTeX, sin embargo su utilización esta lejos de ser sencilla, tiene una curva de aprendizaje grande y se requiere de bastante código para poder hacer circuitos sencillos.

Utilizando Inkscape en combinación con Circuitikz y el complemento TexText se pueden realizar de manera muy sencilla los cualquier tipo de circuito y se reduce tanto el tiempo de creación del gráfico como el manejo de este, ya que después de finalizar el diseño este se puede exportar tanto como **.eps** como **.pdf**, formatos muy amigables para LaTeX.

Es importante saber utilizar lo básico de Inkscape, aquí hay una lista de los comandos y menús mas importantes:

## Comandos 
|          Acción      			|        Atajo         	|
|-------------------------------|-----------------------|
|Group			 				|`Ctrl + G`      		|
|Ungroup         				|`Shift + Ctrl + G`   	|
|Duplicate         				|`Ctrl + D`			   	|
|Copy         					|`Ctrl + C`			   	|
|Paste	         				|`Ctrl + V`			   	|
|Rotate	90° left   				|`Ctrl + [`			   	|
|Rotate	90° rigth 				|`Ctrl + ]`			   	|
|Flip vertically				|`H`			   		|
|Flip horizontally				|`V`			   		|
> **Note:** En los comandos **Flip** no es necesario apretar `Shift`.


## Menús
|         Menú      			|        Atajo    	 	|
|-------------------------------|-----------------------|
|Object/Align and Distribute 	|`Shift + Ctrl + A`		|
|Object/Fill and Stroke 	 	|`Shift + Ctrl + F`		|
|File/Document Properties	 	|`Shift + Ctrl + D`		|

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

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$
