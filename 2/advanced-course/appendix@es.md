---
$title: Apéndice
$order: 4
leveled: cierto
---

[nivel de filtro = "principiante"]

## ¿Qué es JSON?

`<amp-list>` , `<amp-bind>` y `<amp-state>` pueden leer datos JSON. JSON es la abreviatura de JavaScript Object Notation. Es un "formato ligero de intercambio de datos". Aunque se basa en un subconjunto de JavaScript, es independiente del idioma, lo que significa que todos los idiomas pueden leerlo y entenderlo. Los datos JSON se representan, por lo general, de dos formas: ya sea como una colección de pares de clave (nombre) y valor, o como una lista ordenada de valores (lo que conocemos como una lista o matriz). La sintaxis JSON suele tener este aspecto:

[código fuente: json] {"personas": {"número": 2, "nombres": ["Alice", "Bob"]}} [/ código fuente]

Si desea una especificación completa, puede consultar la [documentación oficial](https://www.json.org/) .

## ¿Qué es Deep Merge?

We explained that when `AMP.setState()` is called, `<amp-bind>` will "deep-merge the provided object literal with the current state." The deep-merge functionality will not overwrite anything, but will rather merge the two objects. [In the example]({{g.doc('/content/amp-dev/documentation/components/reference/amp-bind.md', locale=doc.locale).url.path}}#deep-merge-with-ampsetstate) on the `<amp-bind>` documentation, we see that providing only an age for the employee will just update the value of the age of the employee in the state.

[código fuente: html] {% raw%} <button on = "tap: AMP.setState ({employee: {name: 'John Smith', age: 47, vehicle: 'Car'}})" ...> < button on = "tap: AMP.setState ({employee: {age: 64}})" ...> {% endraw%} [/ sourcecode]

El resultado después de presionar el segundo botón actualiza la edad:

[código fuente: json] {empleado: {nombre: 'John Smith', edad: 64, vehículo: 'Coche',}} [/ código fuente]

Si amp-bind estaba aplicando una fusión superficial, el resultado después de presionar el segundo botón sería el siguiente:

[código fuente: json] {empleado: {edad: 64,}} [/ código fuente]

Una copia superficial simplemente actualizaría toda la estructura. La fusión profunda se encarga de agregar al estado nuevos elementos fusionando las entradas existentes, en lugar de actualizarlas por completo.

## ¿Qué es Glitch?

Para completar los ejemplos de código incluidos en estos cursos, <a href="https://glitch.com/" target="_blank">usaremos Glitch</a> . Glitch es un editor de código en línea que le permite crear y ver sitios web y API de servidor sin tener que instalar nada en su computadora.

El entorno del editor de código Glitch se ve así:

{{image ('/ static / img / cursos / intermedio / image12.png', 533, 344, caption = 'El editor en línea de Glitch')}}

El cuadro rojo de arriba es el editor en línea donde ingresará HTML y CSS. El cuadro verde marca el botón que lo llevará a la versión en vivo de la página que está creando. El cuadro amarillo es el botón que le permite crear una copia de este proyecto y editarlo. El cuadro azul indica los archivos que tiene disponibles. En la carpeta de activos, puede encontrar sus imágenes.

A lo largo de estos cursos, necesitará varias imágenes para completar los ejercicios. Todas las imágenes que necesita para completar estos cursos ya se han agregado a los proyectos Glitch. Para ver las imágenes en su proyecto, haga clic en la entrada de activos en la lista de archivos en el lado izquierdo del editor Glitch. Para obtener el enlace a una sola imagen, seleccione la imagen de la lista de activos en el lado derecho y haga clic en el botón "copiar" junto a la URL en la ventana emergente que aparece. Puede usar ese enlace en cualquier lugar donde se necesite una imagen.

{{imagen ('/ estática / img / cursos / intermedio / imagen10.png', 1686, 936, caption = 'La vista de activos en Glitch')}}

{{image ('/ static / img / cursos / intermedio / image9.png', 1484, 1416, caption = 'La ventana emergente de detalles, incluida la URL, para una imagen en la colección de activos')}}

Abra <a href="https://glitch.com/edit/#!/enshrined-eyebrow" target="_blank">este proyecto</a> . Haga clic en el botón "Mezclar esto" en la parte superior derecha. Esto creará un nuevo proyecto que puede editar. Puede continuar utilizando este mismo editor para esta y futuras capacitaciones. Cada tutorial futuro le dará la oportunidad de comenzar con una versión de referencia de la solución hasta ese momento.

No es necesario utilizar Glitch para completar estos entrenamientos. Sin embargo, algunos de los códigos necesarios para completar los ejercicios no se tratan en estos cursos, pero están incluidos en los ejemplos de Glitch. Si desea utilizar otro editor, es posible que deba acceder a las muestras de Glitch para copiar el código CSS y del servidor en su solución local. [/ filter] [nivel de filtro = "avanzado"]

## ¿Qué es JSON?

`<amp-list>` , `<amp-bind>` y `<amp-state>` pueden leer datos JSON. JSON es la abreviatura de JavaScript Object Notation. Es un "formato ligero de intercambio de datos". Aunque se basa en un subconjunto de JavaScript, es independiente del idioma, lo que significa que todos los idiomas pueden leerlo y entenderlo. Los datos JSON se representan, por lo general, de dos formas: ya sea como una colección de pares de clave (nombre) y valor, o como una lista ordenada de valores (lo que conocemos como una lista o matriz). La sintaxis JSON suele tener este aspecto:

[código fuente: json] {"personas": {"número": 2, "nombres": ["Alice", "Bob"]}} [/ código fuente]

Si desea una especificación completa, puede consultar la [documentación oficial](https://www.json.org/) .

## ¿Qué es Deep Merge?

We explained that when `AMP.setState()` is called, `<amp-bind>` will "deep-merge the provided object literal with the current state." The deep-merge functionality will not overwrite anything, but will rather merge the two objects. [In the example](../../../documentation/components/reference/amp-bind.md#deep-merge-with-ampsetstate) on the `<amp-bind>` documentation, we see that providing only an age for the employee will just update the value of the age of the employee in the state.

[código fuente: html] {% raw%} <button on = "tap: AMP.setState ({employee: {name: 'John Smith', age: 47, vehicle: 'Car'}})" ...> < button on = "tap: AMP.setState ({employee: {age: 64}})" ...> {% endraw%} [/ sourcecode]

El resultado después de presionar el segundo botón actualiza la edad:

[código fuente: json] {empleado: {nombre: 'John Smith', edad: 64, vehículo: 'Coche',}} [/ código fuente]

Si amp-bind estaba aplicando una fusión superficial, el resultado después de presionar el segundo botón sería el siguiente:

[código fuente: json] {empleado: {edad: 64,}} [/ código fuente]

Una copia superficial simplemente actualizaría toda la estructura. La fusión profunda se encarga de agregar al estado nuevos elementos fusionando las entradas existentes, en lugar de actualizarlas por completo.

## ¿Qué es Glitch?

Para completar los ejemplos de código incluidos en estos cursos, <a href="https://glitch.com/" target="_blank">usaremos Glitch</a> . Glitch es un editor de código en línea que le permite crear y ver sitios web y API de servidor sin tener que instalar nada en su computadora.

El entorno del editor de código Glitch se ve así:

{{image ('/ static / img /ourses / advanced / image6.png', 533, 344, caption = 'El editor en línea de Glitch')}}

El cuadro rojo de arriba es el editor en línea donde ingresará HTML y CSS. El cuadro verde marca el botón que lo llevará a la versión en vivo de la página que está creando. El cuadro amarillo es el botón que le permite crear una copia de este proyecto y editarlo. El cuadro azul indica los archivos que tiene disponibles. En la carpeta de activos, puede encontrar sus imágenes.

A lo largo de estos cursos, necesitará varias imágenes para completar los ejercicios. Todas las imágenes que necesita para completar estos cursos ya se han agregado a los proyectos Glitch. Para ver las imágenes en su proyecto, haga clic en la entrada de activos en la lista de archivos en el lado izquierdo del editor Glitch. Para obtener el enlace a una sola imagen, seleccione la imagen de la lista de activos en el lado derecho y haga clic en el botón "copiar" junto a la URL en la ventana emergente que aparece. Puede usar ese enlace en cualquier lugar donde se necesite una imagen.

{{image ('/ static / img / course / advanced / image1.png', 1686, 936, caption = 'La vista de activos en Glitch')}}

{{image ('/ static / img / cursos / advanced / image11.png', 371, 354, caption = 'La ventana emergente de detalles, incluida la URL, para una imagen en la colección de activos')}}

Abra <a href="https://glitch.com/edit/#!/enshrined-eyebrow" target="_blank">este proyecto</a> . Haga clic en el botón "Mezclar esto" en la parte superior derecha. Esto creará un nuevo proyecto que puede editar. Puede continuar utilizando este mismo editor para esta y futuras capacitaciones. Cada tutorial futuro le dará la oportunidad de comenzar con una versión de referencia de la solución hasta ese momento.

No es necesario utilizar Glitch para completar estos entrenamientos. Sin embargo, algunos de los códigos necesarios para completar los ejercicios no se tratan en estos cursos, pero están incluidos en los ejemplos de Glitch. Si desea utilizar otro editor, es posible que deba acceder a las muestras de Glitch para copiar el código CSS y del servidor en su solución local. [/filtrar]
