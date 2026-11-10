# Exprimidor · Forma y movimiento

[Abrir la presentación](https://edward9909.github.io/exprimidor-interactivo/).

También puedes descargar `index.html` y abrirlo con Chrome o Edge. Es un archivo autónomo: incluye el modelo y el visor, y funciona sin conexión.

## Controles

- Arrastrar: girar el modelo. Rueda o gesto de pinza: acercar y alejar.
- Clic en una pieza: ver su descripción. «Aislar pieza» permite examinarla sola.
- Capítulos inferiores o flechas izquierda/derecha: recorrer la presentación.
- Piezas: cambiar la separación del despiece y seleccionar componentes.
- Funcionamiento: abrir la palanca y girar la copa por separado, o reproducir una secuencia.
- Corte transversal: activar una sección con caras rellenas y rayadas desde cualquier capítulo.
- Interior: observar presión y giro con el corte activo; cambiar entre corte frontal, lateral y horizontal, desplazar el plano, ocultar la carcasa o desactivar el rayado. «Vista del corte» vuelve al encuadre ortográfico.
- Escala: consultar la envolvente aproximada en milímetros.
- PNG: guardar una imagen de la vista 3D actual.

## Alcance

Modelo actualizado el 9 de noviembre de 2026 a partir de `Configuración 1.fbx` (ensamble «Configuración 1 v9»). Se conservan sus siete cuerpos, sus posiciones relativas y las normales de superficie. Las coordenadas importadas se convierten de metros a milímetros y se reorientan para colocar la base horizontal.

Envolvente aproximada de la malla en la posición del archivo: 208.791 × 177.097 × 241.158 mm (X, Y, Z). Se redondea a 209 × 177 × 241 mm en la presentación. Son medidas de referencia visual, no cotas de fabricación.

Los siete cuerpos son base/recipiente, copa con mango, carcasa/cesta, palanca, enlace posterior, casquillo central y un cuerpo auxiliar lateral identificado como Body38. Este último se mantiene en la ubicación del FBX; no se le asigna una función mecánica no confirmada. Las siete mallas tienen topología cerrada y orientación de caras coherente al verificar sus vértices coincidentes.

Se mantiene el principio confirmado por el autor: la palanca baja la copa y el mango lateral permite girarla. El FBX no contiene animaciones. La animación de la presentación usa articulaciones aproximadas ajustadas a la nueva posición del mecanismo y un recorrido ilustrativo. No verifica límites de carrera, contacto con fruta, roscado, fuerzas, tolerancias, colisiones ni viabilidad mecánica.

El acabado neutro y los colores por componente son representaciones del visor, no especificaciones de material. El despiece facilita la inspección y no define una secuencia de montaje. El corte se actualiza con el movimiento y marca las caras seccionadas mediante rayado.

Importación del FBX con Blender 4.5; visor con Three.js 0.180.0. [Documentación de Three.js](https://threejs.org/docs/).
