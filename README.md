# Exprimidor · Visor 3D

[Abrir la presentación](https://edward9909.github.io/exprimidor-interactivo/).

También puedes descargar `index.html` y abrirlo con Chrome o Edge. El HTML incluye el modelo y el visor. Para reproducir la presentación sin conexión, descarga también la carpeta `film` junto al HTML.

## Controles

- Arrastra para girar; rueda o gesto de pinza para acercar. Clic en una pieza para seleccionarla y aislarla.
- **Mover:** apertura de la palanca de 0° a 90°, giro de la copa de 0° a 65° y control manual del movimiento. «Reproducir · 4 min» abre la presentación gráfica de cuatro minutos sin audio. Los textos se superponen al render completo. El indicador aparece durante el giro de la copa y al alcanzar la apertura máxima de la palanca. El reproductor permite pausar y avanzar. Al terminar o salir se recupera el visor.
- **Piezas:** separación regulable, unión y selección de los siete cuerpos. Al separar o aislar se ajusta el encuadre.
- **Corte:** botón junto al visor para activarlo; plano frontal, lateral u horizontal, posición y rayado. Se puede volver a Mover conservando el corte.
- **Materiales:** aluminio satinado, agarres azules y recipiente de plástico translúcido. En «Materiales y vista» se cambia el color de los agarres y la translucidez, y se activan numeración, medidas u ocultación de la carcasa.
- Selector de acabado: Materiales, Neutro, Por pieza o Bordes.
- Cámara: 3D, Frente, Lateral, Superior y Encuadrar. El botón de cámara descarga un PNG.
- «Controles» pliega el panel. «Restablecer» devuelve los valores iniciales.
- Teclado: Tab para navegar, flechas en pestañas y sliders; con el visor enfocado, flechas para girar y +/− para zoom. Escape quita la selección.

La interfaz toma la nueva referencia gráfica proporcionada por el autor: panel marfil (#E8DFD5), texto y estados activos en azul profundo (#272D4E), acción principal naranja (#FF7124) y estudio grafito (#202124). Los controles se organizan en un panel lateral sólido, con líneas finas y radios de 4 px. El encuadre reserva espacio para el panel sin tapar el modelo. La interfaz concentra la exploración en el modelo y conserva los ajustes al cambiar de herramienta. En móvil el panel se sitúa debajo del visor y puede plegarse.

## Materiales de exploración

El estudio usa fondo grafito con una variación tonal suave que distingue el plástico translúcido, iluminación de entorno HDR calculada con softboxes, reflejos PBR, mapas procedurales de rugosidad y microrelieve, y transmisión/refracción para el recipiente. Los recursos se generan localmente; el visor sigue funcionando sin conexión.

La apariencia toma como referencia visual `exprimidor_final.png`: aluminio satinado y agarres de acabado mate. El recipiente se representa como **plástico translúcido**, confirmado por el autor. La distribución azul/metal en los dos cuerpos unidos usa máscaras locales, por lo que acompaña el movimiento sin modificar la geometría. Los límites de los agarres y los parámetros ópticos son aproximaciones visuales; no son una definición de materiales de fabricación. En corte se desactiva temporalmente la transmisión del recipiente para conservar la legibilidad de la sección.

## Alcance

Modelo actualizado el 9 de noviembre de 2026 a partir de `Configuración 1.fbx` (ensamble «Configuración 1 v9»). Se conservan sus siete cuerpos, sus posiciones relativas y las normales de superficie. Las coordenadas importadas se convierten de metros a milímetros y se reorientan para colocar la base horizontal.

Envolvente aproximada de la malla en la posición del archivo: 208.791 × 177.097 × 241.158 mm (X, Y, Z). Se redondea a 209 × 177 × 241 mm en la presentación. Son medidas de referencia visual, no cotas de fabricación.

Los siete cuerpos son base/recipiente, copa con mango, carcasa/cesta, palanca, enlace posterior, casquillo central y un cuerpo auxiliar lateral identificado como Body38. Este último se mantiene en la ubicación del FBX; no se le asigna una función mecánica no confirmada. Las siete mallas tienen topología cerrada y orientación de caras coherente al verificar sus vértices coincidentes.

Se mantiene el principio confirmado por el autor: la palanca baja la copa y el mango lateral permite girarla. El FBX no contiene animaciones. La apertura de 0° a 90° articula el brazo principal y el enlace posterior por separado. Los centros de los dos pasadores se ajustaron a los círculos de 2.5 mm de radio del FBX. La unión central coordina una salida vertical inicial y una inclinación posterior de la copa, conforme a la aclaración del autor. La copa conserva un punto interior sobre el eje de la canasta durante el recorrido. El giro se limita a 0°–65°; se centra durante la salida inicial (apertura mayor que 0° y menor que 35°) para evitar interferencias observadas con la malla. El cierre recupera la posición del archivo.

La trayectoria es una representación cinemática para inspección visual. La verificación de intersecciones se realiza sobre las superficies trianguladas del émbolo y la canasta en posiciones muestreadas; no equivale a una certificación continua de holguras, fuerzas, tolerancias o viabilidad de fabricación. El visor no calcula colisiones en tiempo real. La comprobación VTK de esta trayectoria revisó 1,083 combinaciones (apertura cada 0.25° y giros solicitados de 0°, 32.5° y 65°, con el centrado inicial aplicado) y no detectó intersecciones entre las dos mallas en esas muestras.

El acabado neutro y los colores por componente siguen disponibles como vistas alternativas. El despiece facilita la inspección y no define una secuencia de montaje. El corte se actualiza con el movimiento y marca las caras seccionadas mediante rayado.

Importación del FBX con Blender 4.5; visor con Three.js 0.180.0. [Documentación de Three.js](https://threejs.org/docs/).
