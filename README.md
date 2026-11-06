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

Se usa la geometría de `exprimidor iges.iges`, exportado el 6 de noviembre de 2026. Sus seis entidades principales se han triangulado para visualización. La fuente declara centímetros; el importador transforma las coordenadas a milímetros.

Envolvente aproximada de la malla en la posición del archivo: 232.006 × 170.668 × 230.683 mm (X, Y, Z). Se redondea a 232 × 171 × 231 mm en la presentación. Las cotas son de referencia visual, no de fabricación.

El autor confirmó que la palanca baja la copa y el mango en L la hace girar mientras presiona el cítrico. La animación ilustra ese principio con un recorrido de demostración y articulaciones aproximadas. No verifica límites de carrera, contacto con fruta, relación de rosca, fuerzas, tolerancias, colisiones ni viabilidad del mecanismo. El movimiento animado no modifica el IGES.

Los colores identifican componentes y no son especificaciones de material. Los nombres se asignaron por inspección de la geometría. El despiece no es una secuencia de montaje. La sección rellena las caras cortadas y las distingue con rayado; se actualiza en cada fotograma con la posición del mecanismo.

La actualización del corte vuelve a triangular las superficies originales mediante Delabella, con reparación topológica y costura de tolerancia 0.01 mm. Se verificó que las 423 caras del IGES tuvieran triangulación; la malla anterior omitía una cara de la copa. Las seis entidades y sus superficies se conservan. La sección es una herramienta visual y no una validación dimensional o mecánica.

Conversión con Open CASCADE; visor con Three.js 0.180.0. [Documentación de Three.js](https://threejs.org/docs/).
