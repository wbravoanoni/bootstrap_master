# Inicio Curso Bootstrap 4

## ¿Que es Bootstrap?

Bootstrap es un kit de herramientas de código abierto para desarrollar con HTML, CSS y JS. Haga un prototipo rápido de sus ideas o cree su aplicación completa con nuestras variables y mixins de Sass, sistema de cuadrícula sensible, componentes precompilados extensos y potentes complementos basados ​​en jQuery.


[Ir a Expo Bootstrap](http://expo.getbootstrap.com/ "Ir a Expo Bootstrap")

## Primeros Pasos

1. Descargar Bootstrap (Compiled CSS and JS)
2. Agregar el meta:vp
3. Agregar CSS de Bootstrap
4. Descargar Jquery e insertar al final del body (min)
5. Insertar Jquery de Bootstrap (min)

## Grid de Bootstrap

1. div.container
2. div.row
3. div.col (Determina tamaño automático según elementos)
4. div.col-12 (Determina tamaño extra pequeño)

~~~
	.col      Extra pequeño (Extra Small) - Smartphone Vertical  Menos de 544px
	.col-sm   Pequeño (Small)  - Smartphones Verticales          Más de 544px y Menos de 768px
	.col-md   Mediano (Medium) - Tablets			     Más de 768px y Menos de 992px
	.col-lg   Largo (Large) - Computadoras			     Más de 992px y Menos de 1200px
	.col-xl   Extra Largo (Extra Large) - Computadoras	     Más de 1200px
~~~

5. div.col-auto (Utiliza solo el espacio que necesita si se combina con div.col)
6. div.col-sm-auto (Se puede combinar con los tamaños de dispositivos)
7. div.w-100 (Crea una fila rapida)

## Alinear verticalmente


### estilos previos

~~~
	<style>
		.row {
			background-color:#e8e8e8;
			height:150px;
			margin-top:20px; 
		}

		.col {
			  background-color:#f2f2f2;
			  text-align: center;
			  padding:10px;
			  border: 1px solid #4d5061;
		     }

	</style>
~~~

### Alinear Filas

![Alineado Vertical](asset/img/alineacion_vertical.png)

1. div.row align-items-start  (alinear al principio toda la fila)
2. div.row align-items-center (alinear al centro toda la fila)
3. div.row align-items-end    (alinear al final toda la fila)

### Alineación independiente

![Alineado Independiente](asset/img/alineacion_independiente.png)

1. div.col align-self-start   (Alinear columna al principio)
2. div.col align-self-center  (Alinear columna al centro)
3. div.col align-self-end     (Alinear columna al final)


### Alineado Horizontal

![Alineado Horizontal](asset/img/alineado_horizontal.png)

1. Solo funciona para div.row
2. div.row justify-content-start   (Alinear Fila al princio)
3. div.row justify-content-center  (Alinear Fila al centro)
4. div.row justify-content-end     (Alinear Fila al final)
5. div.row justify-content-around  (Alinear Fila al rededor)
6. div.row justify-content-between (Alinear Fila entre espacios)


## Offseting

1. div.offset-2
2. div.offset-lg-4 (Centrar en dispositivo Largos, similar a justify-content-center)
3. div.offset-lg-0 (Reinicia offset)

## Reodenar columnas

- Indicar que columnas van primero y cuales despues sin tocar el HTML

1. div.row justify-content-between
2. div.flex-first
3. div.flex-last
4. div.flex-unordered


## Ocultar elementos

Existen elementos que ya no son compatibles con V4 Alpha
como por ejemplo .hidden-xs-down

[Nuevos Hidden](https://getbootstrap.com/docs/4.0/utilities/display/ "Nuevos Hidden")

1. div.col d-none d-sm-block (SM - Small)
2. div.col d-none d-md-block (MD - Medium)
3. div.col d-none d-lg-block (LG - Large)
4. div.col d-none d-xl-block (XL - Extra Large)

## Tipografia



1. small.text-muted (Textos mas suaves)
2. p.h1             (Parrafo con estilo de h1)
3. h1.display-1     (Encabezado con letras mas delgadas 1-4)
4. p.lead           (Parrafo resaltado)


## Tipografia 2 tag

<mark>   (Texto Destacado)
<del>    (Texto Tachado)
<s>	     (Texto Tachado)
<ins>    (Texto Subrayado)
<u>	     (Texto Subrayado)
<strong> (Texto en negritas)
<small>  (Texto mas pequeño)
<em>     (Texto en italic)

p.text-justify			(Texto Justificado)
div.card>div.card-block (Crear cartas)

### Alinear Textos

1. p.text-left     (Texto alineado a la izquierda)
2. p.text-center   (Texto centrado)
3. p.text-right    (Texto alineado a la derecha)

4. p.text-left text-sm-right (Texto sm alineado a la derecha)
5. p.text-left text-md-right (Texto md alineado a la derecha)
6. p.text-left text-lg-right (Texto lg alineado a la derecha)
7. p.text-left text-xl-right (Texto xl alineado a la derecha)

8. p.text-lowercase font-weight-bold   (Minusculas y negritas)
9. p.text-uppercase font-weight-normal (Mayusculas y normal)
10. p.text-capitalize font-italic      (Letras capitales e italic)

## Boques de codigo

~~~
<pre><code>&lt;h1&gt;Lorem ipsum dolor sit amet.&lt;/h1&gt;</code></pre>
~~~

la etiqueta kbd permite agregar atajos de teclas

<p>Para copiar texto Presiona <kbd>Ctrl + C </kbd></p>

## Imagenes


#### lorempixel
http://lorempixel.com/200/200


1. img-fluid     (Imagen se adapta al contenedor)
2. rounded       (Esquinas redondeadas)
3. img-thumbnail (Imagenes con border blancos)
4. float-left    (Imagen flotante a la izquierda)
5. float-right   (Imagen flotante a la derecha)

#### tag para imagenes

1. figure.figure  			 (Crear cuadro de figura)
2. img.img-fluid rounded 	 (Crear imagen responsiva)	
3. figcaption.figure-caption  (Crear Mensaje en pie de img)
4. p.text-center">Lorem ipsum (Centrar texto de pie de img)

## Tablas

1. table.table          (Modo tabla)
2. table.table-striped  (Sombreado a elementos pares)
3. table.table-bordered (Tabla con bordes)
4. table.table-hover    (Tabla marcada cuando se pasa el mouse)
5. table.dark 			(Similar a inverse)
6. table.thead-dark     (Similar a inverse pero para encabezados)

### Colores

![tabla](asset/img/tablas.png)

1.  tr.table-primary (Color azul claro)
2.  tr.table-success (Color verde claro)
3.  tr.table-warning (Color naranja claro)
4.  tr.table-danger  (Color rojo claro)
5.  tr.table-info    (Color celeste claro)
6.  tr.bg-primary    (Color azul oscuro)
7.  tr.bg-success    (Color verde oscuro)
8.  tr.bg-warning    (Color naranja oscuro)
9.  tr.bg-danger     (Color rojo oscuro)
10. tr.bg-info       (Color celeste oscuro)





