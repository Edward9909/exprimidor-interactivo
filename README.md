# Exprimidor · Forma y movimiento

[Abrir la presentación](https://edward9909.github.io/exprimidor-interactivo/).

También puedes descargar `index.html` y abrirlo con Chrome o Edge. Es un archivo autónomo: incluye el modelo y el visor, y funciona sin conexión.

## Controles

- Arrastra para girar; rueda o gesto de pinza para acercar. Clic en una pieza para seleccionarla y aislarla.
- **Mover:** apertura de la palanca, giro de la copa, reproducción, pausa y continuación de la secuencia.
- **Piezas:** separación regulable, unión y selección de los siete cuerpos. Al separar o aislar se ajusta el encuadre.
- **Corte:** botón junto al visor para activarlo; plano frontal, lateral u horizontal, posición y rayado. Se puede volver a Mover conservando el corte.
- **Materiales:** metal satinado, agarres azules y recipiente de plástico translúcido. En «Materiales y vista» se cambia el color de los agarres y la translucidez, y se activan numeración, medidas u ocultación de la carcasa.
- Selector de acabado: Materiales, Neutro, Por pieza o Bordes.
- Cámara: 3D, Frente, Lateral, Superior y Encuadrar. El botón de cámara descarga un PNG.
- «Controles» pliega el panel. «Restablecer» devuelve los valores iniciales.
- Teclado: Tab para navegar, flechas en pestañas y sliders; con el visor enfocado, flechas para girar y +/− para zoom. Escape quita la selección.

La interfaz concentra la exploración en el modelo y conserva los ajustes al cambiar de herramienta. En móvil el panel se sitúa debajo del visor y puede plegarse.

## Materiales de exploración

La apariencia toma como referencia visual `exprimidor_final.png`: metal satinado y agarres de acabado mate. El recipiente se representa como **plástico translúcido**, confirmado por el autor. La distribución azul/metal en los dos cuerpos unidos usa máscaras locales, por lo que acompaña el movimiento sin modificar la geometría. Los límites de los agarres y los parámetros ópticos son aproximaciones visuales; no son una definición de materiales de fabricación. En corte se desactiva temporalmente la transmisión del recipiente para conservar la legibilidad de la sección.

## Alcance

Modelo actualizado el 9 de noviembre de 2026 a partir de `Configuración 1.fbx` (ensamble «Configuración 1 v9»). Se conservan sus siete cuerpos, sus posiciones relativas y las normales de superficie. Las coordenadas importadas se convierten de metros a milímetros y se reorientan para colocar la base horizontal.

Envolvente aproximada de la malla en la posición del archivo: 208.791 × 177.097 × 241.158 mm (X, Y, Z). Se redondea a 209 × 177 × 241 mm en la presentación. Son medidas de referencia visual, no cotas de fabricación.

Los siete cuerpos son base/recipiente, copa con mango, carcasa/cesta, palanca, enlace posterior, casquillo central y un cuerpo auxiliar lateral identificado como Body38. Este último se mantiene en la ubicación del FBX; no se le asigna una función mecánica no confirmada. Las siete mallas tienen topología cerrada y orientación de caras coherente al verificar sus vértices coincidentes.

Se mantiene el principio confirmado por el autor: la palanca baja la copa y el mango lateral permite girarla. El FBX no contiene animaciones. La animación de la presentación usa articulaciones aproximadas ajustadas a la nueva posición del mecanismo y un recorrido ilustrativo. No verifica límites de carrera, contacto con fruta, roscado, fuerzas, tolerancias, colisiones ni viabilidad mecánica.

El acabado neutro y los colores por componente siguen disponibles como vistas alternativas. El despiece facilita la inspección y no define una secuencia de montaje. El corte se actualiza con el movimiento y marca las caras seccionadas mediante rayado.

Importación del FBX con Blender 4.5; visor con Three.js 0.180.0. [Documentación de Three.js](https://threejs.org/docs/).
