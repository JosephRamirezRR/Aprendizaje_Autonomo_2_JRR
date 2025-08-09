# Paso 1 – Inicio del desarrollo y configuración del entorno

En esta primera etapa se preparó el entorno de desarrollo, se configuró el repositorio y se diseñaron diagramas de flujo para comprender la lógica de distintos programas sencillos.  Además de los diagramas, se incluyó un primer avance del código en el directorio `avance_codigo`.

## Configuración del entorno

* **Repositorio y control de versiones.**  Se creó un nuevo repositorio en GitHub para documentar el trabajo.  Esta práctica permitió familiarizarse con Git (inicializar repositorio, crear ramas y hacer *commits*) y con la plataforma de colaboración.
* **Herramientas utilizadas.**  Se utilizó Python 3.x como lenguaje de programación por su sencillez y disponibilidad.  El entorno de desarrollo fue VS Code, junto con la terminal para ejecutar los programas.
* **Dependencias.**  Para estos ejemplos se utilizó únicamente la biblioteca estándar de Python (`random` para selecciones aleatorias).  No fue necesario instalar paquetes externos.

## Diagramas de flujo

En la carpeta `diagramas_flujo` se encuentran tres diagramas de flujo en formato PNG.  Cada uno describe la lógica de un mini‑programa diferente.  Los diagramas fueron creados para practicar la representación gráfica de algoritmos y utilizan la simbología recomendada: óvalos para inicio/fin y rectángulos para procesos.  Según la documentación de diagramas de flujo, un diagrama de flujo **representa gráficamente los pasos o procesos a seguir para alcanzar la solución de un problema** y su correcta construcción facilita la traducción a un lenguaje de programación【526061983532167†L29-L41】.  Las reglas básicas indican que debe existir un inicio y un fin, que las flechas conectan los procesos en orden y que la notación es independiente del lenguaje【526061983532167†L102-L116】.

### Generador de contraseñas

En este diagrama se describe un generador de contraseñas.  El proceso comienza solicitando al usuario la longitud deseada.  Luego se definen los conjuntos de letras, números y símbolos; se genera la contraseña mediante selección aleatoria y se muestra el resultado.  Este ejercicio ilustra un flujo secuencial sin decisiones.

### Adivinar número

El segundo diagrama describe un juego para adivinar un número.  Tras definir un número objetivo (puede ser fijo o aleatorio), se da la bienvenida al usuario y se le solicita adivinarlo.  Se utiliza una estructura condicional simple: si el número es correcto se felicita al jugador, de lo contrario se muestra un mensaje de error.  Según los principios de las estructuras condicionales, la decisión se basa en una condición que determina qué camino seguir【526061983532167†L137-L156】.

### Piedra, papel o tijera

El tercer diagrama muestra el flujo de un juego de piedra, papel o tijera.  Se definen las opciones disponibles, se pide una elección al usuario y la máquina selecciona aleatoriamente.  Se determinan las condiciones de victoria con una serie de decisiones (`if`).  Finalmente, se pregunta al usuario si desea jugar de nuevo; esta pregunta crea un ciclo (estructura repetitiva) hasta que el usuario decide terminar.

Estos diagramas no sólo ayudan a visualizar la lógica sino que obligan a pensar en la secuencia de pasos y en la necesidad de estructuras condicionales y repetitivas.  Como se indica en la teoría de las estructuras repetitivas, un ciclo permite ejecutar un conjunto de instrucciones varias veces mientras se cumpla una condición【764491155720622†L8-L33】.  Integrar esta idea en los diagramas facilita luego la codificación.

## Avance de código

En el directorio `avance_codigo` se incluye un primer avance del juego del ahorcado (`JuegoAhorcado.py`).  Este avance implementa las funciones básicas del juego (selección aleatoria de palabra, visualización del tablero, manejo de vidas y registro de letras adivinadas).  Se eligió este juego porque combina estructuras de control fundamentales (condicionales y ciclos) y permite aplicar la lógica representada en los diagramas.  El código está comentado en español para explicar los pasos y las decisiones tomadas.

## Reflexión y conclusiones del Paso 1

Elaborar los diagramas y configurar el repositorio ayudó a organizar el pensamiento antes de escribir código.  Los diagramas de flujo obligan a analizar cada paso de la solución, lo que evita errores lógicos y facilita la implementación.  Además, trabajar con Git y GitHub desde el inicio promueve buenas prácticas de ingeniería de software.

Como perspectiva personal, este ejercicio demuestra que **planificar** (a través de diagramas) resulta tan importante como escribir el programa.  En el futuro, planeo utilizar diagramas de flujo y pseudocódigo antes de codificar proyectos más complejos, ya que la claridad en la lógica se traduce en programas más robustos y mantenibles.

En cuanto a las fuentes consultadas, se revisaron materiales de algoritmos y diagramas de flujo para reforzar la teoría; por ejemplo, se consultó un artículo de la Universidad Anáhuac sobre la definición y las reglas de construcción de diagramas de flujo【526061983532167†L29-L41】, así como tutoriales sobre estructuras condicionales y repetitivas【764491155720622†L8-L33】.  Estos recursos permitieron validar que los diagramas creados cumplen con las buenas prácticas.
