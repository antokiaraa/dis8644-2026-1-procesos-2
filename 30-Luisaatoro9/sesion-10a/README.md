# Sesión 10a - martes 19 mayo 2026

Esta sesión fue súper completa porque mezclamos una charla inspiradora en el auditorio con un repaso técnico bien denso en la sala, enfocado en cómo vamos a armar el proyecto final de filtros.

1. Charla en el auditorio: Escaneo LiDAR 🌸

Vinieron Jim, Patrick y Simon a mostrarnos su trabajo. Lo que más me voló la cabeza fue el modelo 3D de una flor hecho con un escáner LiDAR.

* **Dato técnico:** El láser solo captura la superficie exterior (donde rebota), por lo que el interior queda vacío. Es como una "cáscara" de puntos con colores reales y transparencias.
* **Mi lectura:** Cada punto que marca el láser es como un dato que el sistema procesa. Me hizo clic con lo que vemos en electrónica: sensores que captan la realidad y la convierten en información.

2. Pensamiento Sistémico: El "Bosque" y no solo el "Árbol" 🌲

Antes de lanzarnos a los chips, hablamos de una metodología clave: el Pensamiento Sistémico.

* **¿Qué es? Entender que todo está conectado. Si mueves una pieza aquí, hay una consecuencia allá.**
* **Ejemplo práctico:** Si mi LED no prende, el pensamiento lineal dice "el LED está quemado". El pensamiento sistémico me hace preguntar: "¿Será el código?, ¿la conexión a internet?, ¿o es que la protoboard no tiene energía?".

3. Repaso de Chips para el Proyecto de Filtros 

Después de la charla, bajamos a tierra con el profe para ver qué integrados nos sirven para "limpiar" el audio.
Los osciladores y la lógica:

* **CD4046:** Es una máquina que convierte gestos en frecuencia. A mayor voltaje, frecuencia más rápida. Es un oscilador controlado por voltaje (VCO). Según lo que entendí, sirve más para secuenciadores, así que para mi grupo de filtros quizás no sea el protagonista.
* **CD4093:** Este es pura lógica. Convierte resistencia en frecuencia.
* **CD4040 (Binary Counter):** Este es interesante. Recibe un clock y sus salidas entregan la mitad de esa frecuencia (va dividiendo). Hace que el sonido cambie según la salida que elijas (0,1,2,3,40,1,2,3,4).

Los Amplificadores Operacionales (Op-Amps) - El corazón del filtro:

Como nuestro proyecto es de filtros, necesitamos "limpiar" la señal (input y output). Estas son las opciones que barajamos:

* **TL072 / TL082:** Mis favoritos. Son de bajo ruido (ideal para audio) y traen dos operacionales en un solo chip.
* **LM358:** El plan B. Consume poquísima batería, ideal si queremos que el filtro sea portátil, aunque no es tan "limpio" como el TL072.
* **LM324:** Si el filtro es muy complejo (de cuarto orden, por ejemplo), este nos salva porque trae cuatro operacionales adentro.

### Libro Hacia una filosofía de la fotografía, continuación de la lectura...

Cap 2: El Aparato y la Caja Negra (KiCad vs. Realidad)
<p>
 Al leer sobre el 'Aparato', no pude evitar pensar en el KiCad. Flusser dice que un aparato es una 'caja negra' porque usamos su programa sin saber exactamente qué pasa en el código interno. En el ramo, cuando pasamos del esquema al PCB y lo vemos en 3D, estamos usando un aparato que ya tiene 'pre-programado' cómo debe verse una placa. El riesgo, como dice Flusser, es quedarnos solo en la superficie. Por eso, aprender a leer los circuitos y entender qué hace cada componente en la protoboard es como intentar abrir esa caja negra para no ser solo usuarios que aprietan botones, sino diseñadores que entienden la lógica interna.
</p>

Cap 3: El Gesto de Fotografiar (Cazar el diseño del Filtro)
<p>
  Flusser habla del 'gesto' como una cacería de posibilidades dentro de un programa. Esto me pasó tal cual eligiendo las propuestas para el proyecto de filtros. No es que inventé la electricidad, sino que 'cacé' las mejores combinaciones de resistencias y condensadores dentro de lo que la teoría de filtros permite. Mi 'gesto' en el KiCad, moviendo componentes y ruteando pistas, es exactamente esa búsqueda que describe Flusser, elegir entre las infinitas opciones que el programa me da para que el filtro funcione y se pueda mandar a fabricar.
</p>

Cap 4: La Fotografía (La placa 3D como Imagen Técnica)
<p>
  Este capítulo dice que las imágenes técnicas son conceptos convertidos en imágenes. La visualización 3D de nuestra placa de filtros no es la placa real todavía, es una 'imagen técnica' basada en las leyes de la física y la electrónica que el software traduce. Lo que Flusser advierte es que no debemos confundir esa imagen con la realidad. Por eso es tan importante armar el circuito en la protoboard, ahí es donde la teoría (el concepto) se choca con la materia real y vemos si el filtro de verdad filtra o si solo se veía bonito en el render del KiCad.
</p>

Cap 5: La Distribución (De la pantalla a la fabricación)
<p>
  Flusser explica que en la era de los aparatos lo que importa es la información, no la materia, porque la info se puede reproducir mil veces. Esto lo veo directo en nuestro flujo de trabajo, una vez que terminamos el diseño de los filtros en KiCad, lo que mandamos a la fábrica no es una placa física, es un archivo (información). La fábrica es el aparato que 'distribuye' nuestro diseño en serie. Como dice Flusser, mi rol cambia, ya no soy un artesano que lija cobre, soy un programador de hardware que genera información para que una máquina la ejecute.
</p>

Conclusión Personal: **La Libertad y la Rebeldía de Diseñar**

Lo que más me marcó de esta lectura fue el concepto de 'funcionario'. Flusser advierte que, si solo seguimos las reglas del aparato, dejamos de ser creadores. Al venir del mundo de la ingeniería, sentía que a veces te enseñan a seguir patrones, fórmulas dadas, recopilar datos y ver problemáticas de forma estructurada. Pero al entrar en Diseño, entendí que esta carrera te entrega libertad, aunque es una libertad que hay que ganar.

Siento que para diseñar de verdad hace falta una cuota de rebeldía interna. Si no tienes ese cuestionamiento mental o esa madurez para ver más allá, terminas simplemente cumpliendo con lo que el sistema te pide. La originalidad nace de esa rebeldía de querer forzar al aparato (ya sea el KiCad o la vida misma) a que haga algo más, algo que salió de tu cabeza y no de un manual. Mi meta con este proyecto de filtros es esa, usar la técnica no para repetir patrones, sino para demostrar que lo que uno crea en la mente puede ser real si no dejas que el 'programa' limite tu visión. Es, finalmente, dejar de ser funcionaria para ser una artesana con pensamiento propio.

 **"No te fijes solo en los árboles, fíjate en quién plantó el bosque".**

---

### Referencias

- [Polycam — app de escaneo 3D](https://poly.cam)
- [TL072 — datasheet y aplicaciones](https://www.ti.com/lit/ds/symlink/tl072.pdf)
- [LM358 — características y usos](https://wraycastle.com/es/blogs/knowledge-base/lm358-pinout)
- [LM324 — amplificador operacional cuádruple](https://www.ti.com/lit/ds/symlink/lm324.pdf)

