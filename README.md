### 📘 Ejercicio en Clase 3 – Modularización en Java

## Estudiantes:
# Edward Meyer Natareno García 
# José Yair Hernández Valenzuela

### 1️⃣ Identificación de Tareas Repetitivas


# ¿Qué partes del código pueden convertirse en métodos?



Las partes del código que pueden separarse en métodos son:

Mostrar el menú.

Agregar un estudiante.

Mostrar estudiantes.

Calcular el promedio.

Mostrar el estudiante con la calificación más alta.



# ¿Qué bloques de código se repiten?


El siguiente bloque se repite en más de una opción del programa:

if (calificaciones.isEmpty()) {
    System.out.println("No hay calificaciones registradas.");
}



# ¿Qué responsabilidades pueden separarse?


Las responsabilidades que pueden separarse son:

Agregar estudiantes.

Mostrar la lista de estudiantes.

Calcular el promedio.

Buscar la calificación más alta.

Separar estas tareas mejora el programa porque hace que el código sea más organizado
,fácil de entender y más sencillo de mantener.


### 2️⃣ Variables Locales vs Globales


# ¿Qué variables deben ser globales (static)?


Las variables que deben ser globales son:


estudiantes

calificaciones

Estas se usan en varios métodos del programa.



# ¿Cuáles deben ser locales?


Las variables locales son aquellas que solo se utilizan dentro de un método, por ejemplo:

promedio

suma

nombre

opcion


# ¿Por qué?


Porque estas variables almacenan datos temporales y solo son necesarias durante la ejecución de un método específico.


# Alcance (scope)

Las variables globales pueden utilizarse en todos los métodos de la clase, mientras que las variables locales solo pueden usarse dentro del método donde fueron declaradas.


# Tiempo de vida de la variable

Las variables globales existen durante toda la ejecución del programa.
Las variables locales solo existen mientras se ejecuta el método donde fueron creadas.


# Riesgos de modificar datos globales accidentalmente

Modificar variables globales puede afectar a todo el programa, ya que varios métodos dependen de ellas. Esto puede provocar errores difíciles de detectar.


### 🔐 Validaciones y Manejo de Excepciones

# ¿Qué errores podrían ocurrir?

El programa podía fallar si el usuario ingresaba letras cuando se esperaba un número, por ejemplo al ingresar la opción del menú o la calificación del estudiante.


# ¿Qué validaciones se implementaron?

Se implementaron las siguientes validaciones:

Uso de try-catch para evitar que el programa se cierre si el usuario ingresa texto en lugar de números.

Validación de las entradas del menú.


# ¿Por qué son importantes?


Las validaciones son importantes porque evitan que el programa se detenga por errores del usuario, mejoran la confiabilidad del sistema y permiten una mejor experiencia al usuario.


### 🧩 Parte 4 – Preguntas de Reflexión

## 1️⃣ ¿Qué ventajas tiene dividir el código en métodos?

Dividir el código en métodos ofrece varias ventajas:

# Organización:
 el programa está mejor estructurado y ordenado.

# Reutilización: 
los métodos pueden usarse varias veces sin repetir código.

# Mantenimiento: 
es más fácil corregir errores en una parte específica del programa.

# Claridad: 
cada método cumple una sola función, lo que facilita su comprensión.


## 2️⃣ ¿Por qué no es recomendable usar muchas variables globales?


No es recomendable usar muchas variables globales porque:

Errores inesperados: cualquier método puede modificar su valor sin control.

Dificultad para depurar: es difícil saber qué método causó el problema.

Dependencia entre métodos: los métodos se vuelven dependientes entre sí.


## 3️⃣ ¿Cómo mejora la modularización la legibilidad del código?

La modularización mejora la legibilidad porque el programa se divide en partes pequeñas y claras.
Cada método tiene un nombre que indica su función, lo que permite entender rápidamente qué hace cada parte del programa.
