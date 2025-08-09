# Paso 2 – Desarrollo del programa

En esta segunda etapa se implementó un programa funcional aplicando las estructuras lógicas estudiadas (condicionales y repetitivas).  El programa elegido es un **juego del ahorcado**, cuyo objetivo es adivinar una palabra secreta letra a letra antes de quedarse sin vidas.  El código final se encuentra en el directorio `codigo_final`.

## Descripción del juego

El juego selecciona una palabra aleatoria de una lista predefinida y muestra un tablero con guiones bajo (`_`) en lugar de las letras.  El usuario introduce letras una a una.  Si la letra pertenece a la palabra, se revela en todas sus posiciones; de lo contrario, se descuenta una vida.  El juego termina cuando el usuario adivina todas las letras o se queda sin vidas.

### Estructuras utilizadas

* **Selección aleatoria:** se utiliza la función `random.choice()` de la biblioteca estándar para seleccionar la palabra secreta de una lista.  Esta función es una forma sencilla de obtener un elemento al azar.
* **Ciclo `while`:** el bucle principal del juego se ejecuta mientras queden vidas y no se hayan adivinado todas las letras.  Este tipo de estructura repetitiva permite ejecutar varias veces un conjunto de instrucciones mientras se cumpla una condición【764491155720622†L8-L33】.
* **Estructuras condicionales (`if/else`):** se utilizan para:
  - Verificar si la letra ya fue ingresada por el usuario.
  - Comprobar si la letra forma parte de la palabra secreta.
  - Determinar si el usuario ganó (todas las letras adivinadas) o perdió (vidas agotadas).
* **Listas y conjuntos:** se emplean listas para almacenar las letras adivinadas y la representación del tablero.  Se usa un conjunto para comparar rápidamente si una letra está en la palabra.

## Mejoras realizadas

En comparación con el avance inicial, el código final incluye las siguientes mejoras:

* **Gestión de entradas inválidas:** se verifica que el usuario ingrese una letra válida y se evita penalizar entradas repetidas.
* **Comentarios detallados:** se añadieron comentarios en español explicando cada función y los pasos del algoritmo, lo que facilita la comprensión y el mantenimiento.
* **Organización en funciones:** se separaron las tareas en funciones (`obtener_palabra()`, `mostrar_tablero()`, `jugar_ahorcado()`) para mejorar la legibilidad y permitir reutilizar el código.
* **Variables descriptivas:** se utilizaron nombres de variables en español que reflejan su propósito (por ejemplo, `vidas_restantes`, `letras_adivinadas`).

## Reflexión sobre contradicciones y alternativas

Durante el desarrollo se consideró implementar el juego en **C** para practicar la gestión manual de memoria; sin embargo, se optó por Python debido a la rapidez de desarrollo y la claridad del código para fines educativos.  También se analizó la posibilidad de añadir una interfaz gráfica mediante la librería `tkinter`, pero se descartó para mantener el foco en las estructuras de control y no incrementar la complejidad.

Como alternativa, un enfoque diferente podría utilizar un ciclo `for` para recorrer la lista de letras de la palabra en cada iteración; sin embargo, esto sería menos eficiente que mantener un conjunto de letras restantes y actualizarlo a medida que se adivinan.

Reconocer estas alternativas permite justificar las decisiones tomadas y comprender que existen múltiples formas de resolver el mismo problema.  Elegir una estructura u otra depende del contexto y de las restricciones de cada proyecto.

## Conclusiones

El desarrollo del juego consolidó el uso de **estructuras condicionales** y **estructuras repetitivas** de manera práctica.  La implementación en Python permitió centrarse en la lógica sin preocuparse por detalles de bajo nivel.  Se reforzó la importancia de escribir código claro, modular y bien documentado.  Además, se experimentó con la gestión de errores y la validación de entrada, habilidades esenciales en cualquier proyecto de software.

A nivel personal, este ejercicio me mostró que el aprendizaje autónomo requiere no sólo aplicar lo visto en clase sino también buscar fuentes adicionales, reflexionar sobre el proceso y justificar cada decisión.  En el futuro, me gustaría explorar la versión gráfica del juego y probar otros lenguajes para comparar desempeño y complejidad.

La carpeta `videos` permanece vacía porque no se elaboró un video explicativo; sin embargo, los README contienen suficiente explicación textual del proceso.
