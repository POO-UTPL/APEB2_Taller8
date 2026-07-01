# Propuesta de Prompt para el Taller 8

## Programación Orientada a Objetos

**Carrera:** Ciencias de la Computación  
**Universidad:** Universidad Técnica Particular de Loja (UTPL)  
**Taller:** Taller 8  
**Tema central:** Herencia, polimorfismo, clases abstractas, métodos abstractos, UML y Java

---

## Objetivo del documento

Este documento presenta un prompt estructurado para revisar, generar y retroalimentar soluciones del **Taller 8** de la asignatura **Programación Orientada a Objetos**, considerando el modelado UML en archivos `.PNG` o `.DIA` y la implementación en código `.JAVA`.

El propósito es facilitar una revisión formativa y técnica de las soluciones de los estudiantes, tomando como base los contenidos estudiados sobre abstracción, encapsulamiento, herencia, polimorfismo, clases abstractas, métodos abstractos, relaciones UML, estructuras de datos y buenas prácticas de programación orientada a objetos.

---

# Prompt sugerido para el Taller 8

```text
Considerando el Taller 8: README.md adjunto, de la asignatura “PROGRAMACIÓN ORIENTADA A OBJETOS”, segundo ciclo, carrera de CIENCIAS DE LA COMPUTACIÓN de la UNIVERSIDAD TÉCNICA PARTICULAR DE LOJA: revisa, genera y retroalimenta las soluciones en modelado .PNG y código .JAVA adjuntas.

--------------------------------
Instrucciones adicionales
--------------------------------

1. Enunciado de referencia del taller/ejercicios:
   - Disponible en: https://github.com/POO-UTPL/APEB2_Taller8
   - Si no hay acceso al repositorio, utiliza el archivo README.md adjunto.

2. Subida de imágenes:
   - Se adjunta 1 imagen UML por ejercicio.
   - El formato puede ser .PNG o .DIA.

3. Generación TXT del UML:
   - A partir de cada imagen adjunta, extrae:
     - clases,
     - atributos,
     - métodos,
     - relaciones,
     - jerarquías de herencia,
     - clases abstractas,
     - métodos abstractos.

   - Genera el diagrama en formato Mermaid para ser exportado a StarUML.

   - Usa el siguiente formato:

classDiagram
class NombreClase1{
  <<abstract>>
  -tipo1 nombre_Atributo1
  +tipo2 nombre_Atributo2
  #tipo2 nombre_Atributo3
  +nombre_Metodo_Funcion1*(tipo1 nombre_Atributo) tipoRetorno
  -nombre_Metodo_Funcion2() tipoRetorno
}

class NombreClase2{
  -tipo1 nombre_Atributo1
  +tipo2 nombre_Atributo2
  #tipo2 nombre_Atributo3
  +nombre_Metodo_Funcion1(tipo1 nombre_Atributo) tipoRetorno
  -nombre_Metodo_Funcion2() tipoRetorno
}

NombreClase1 <|-- NombreClase2

   - Define los métodos abstractos con un asterisco (*) al final del nombre del método.
   - Define las clases abstractas con <<abstract>>, tal como se muestra en el ejemplo.
   - No incluyas texto adicional ni explicación dentro del bloque Mermaid.
   - Entrega únicamente el diagrama en formato Mermaid.

4. Generación de soluciones ideales:

   4.1. Diagrama de clases ideal

   Genera una versión corregida y optimizada del “Diagrama de clases”, aplicando criterios de:

   - eficiencia,
   - calidad,
   - abstracción,
   - encapsulamiento,
   - herencia,
   - polimorfismo,
   - clases abstractas,
   - métodos abstractos,
   - patrones de diseño,
   - principios SOLID,
   - buenas prácticas de Programación Orientada a Objetos.

   4.2. Código Java ideal

   Genera una versión corregida y optimizada del código `.java`, aplicando criterios de:

   - eficiencia,
   - calidad,
   - abstracción,
   - encapsulamiento,
   - herencia,
   - polimorfismo,
   - clases abstractas,
   - métodos abstractos,
   - patrones de diseño,
   - principios SOLID,
   - buenas prácticas de Programación Orientada a Objetos,
   - patrón arquitectónico MVC,
   - entradas y salidas de datos únicamente en el método `main()`,
   - uso correcto de sentencias de control selectivas,
   - uso correcto de sentencias de control repetitivas,
   - uso de arreglos estáticos,
   - uso de estructuras dinámicas como `ArrayList` y colecciones de objetos.

5. Contenidos estudiados para este taller:

   Unidad 1: Conceptos Principales de Programación Orientada a Objetos
   - Introducción al Paradigma de Programación Orientada a Objetos.
   - Introducción al Lenguaje Unificado de Modelado.
   - Pilares fundamentales de Programación Orientada a Objetos:
     - abstracción,
     - polimorfismo,
     - herencia,
     - encapsulación.
   - Clases y objetos.
   - Notación UML para clases y objetos.

   Unidad 2: Estructura y creación de programas en Programación Orientada a Objetos
   - Declaración de clases en lenguajes de alto nivel.
   - Manipulación de métodos en Programación Orientada a Objetos.
   - Creación y manipulación de objetos en lenguajes de alto nivel.
   - Uso de métodos establecer y obtener.
   - Manejo y sobrecarga de constructores.
   - Relación entre clases:
     - asociación,
     - agregación,
     - composición.

   Unidad 3: Manejo de Estructuras
   - Estructura de control en Programación Orientada a Objetos:
     - condicionales,
     - repetitivas.
   - Estructuras de datos en Programación Orientada a Objetos:
     - manejo de estructuras estáticas,
     - arreglos de objetos,
     - manejo de estructuras dinámicas,
     - ArrayList,
     - colecciones de objetos,
     - serialización de objetos.

   Unidad 4: Manejo de Herencia
   - Implementación de herencia en lenguaje de alto nivel.
   - Relación entre clases:
     - asociación,
     - agregación,
     - composición,
     - herencia.
   - Nombre, simbología, rol, navegabilidad y multiplicidad en UML.
   - Conceptos generales:
     - superclases,
     - subclases,
     - niveles de acceso.
   - Jerarquía de herencia en diagramas UML.
   - Invocación de constructores.
   - Implementación de herencia en lenguaje de alto nivel.

   Unidad 5: Implementación de Polimorfismo
   - Conceptos generales:
     - clases abstractas,
     - métodos abstractos.
   - Diseño de diagramas UML bajo el polimorfismo.
   - Implementación de polimorfismo en lenguaje de alto nivel.
   - Creación y uso de interfaces en lenguajes de alto nivel.

6. Retroalimentación y evaluación:

   - Compara el “Diagrama de clases” del estudiante con la “Solución ideal generada”.
   - Señala en máximo 1 línea las diferencias y mejoras principales para cumplir totalmente el enunciado del problema.
   - Compara el archivo `.java` del estudiante con la “Codificación ideal generada”.
   - Señala en máximo 1 línea las diferencias y mejoras principales para cumplir totalmente el enunciado del problema.
   - Genera un único informe con:
     - calificación cualitativa,
     - puntaje por criterio,
     - puntaje total,
     - retroalimentación breve y puntual.
```

---

# Formato Mermaid de referencia

> Este formato se debe utilizar para representar diagramas de clases con herencia, clases abstractas y métodos abstractos.

```mermaid
classDiagram
class NombreClase1{
  <<abstract>>
  -tipo1 nombre_Atributo1
  +tipo2 nombre_Atributo2
  #tipo2 nombre_Atributo3
  +nombre_Metodo_Funcion1*(tipo1 nombre_Atributo) tipoRetorno
  -nombre_Metodo_Funcion2() tipoRetorno
}

class NombreClase2{
  -tipo1 nombre_Atributo1
  +tipo2 nombre_Atributo2
  #tipo2 nombre_Atributo3
  +nombre_Metodo_Funcion1(tipo1 nombre_Atributo) tipoRetorno
  -nombre_Metodo_Funcion2() tipoRetorno
}

NombreClase1 <|-- NombreClase2
```

---

# Convenciones para el modelado Mermaid

## Visibilidad de atributos y métodos

| Símbolo | Significado |
|---|---|
| `+` | Público |
| `-` | Privado |
| `#` | Protegido |

## Clases abstractas

Las clases abstractas deben representarse usando:

```mermaid
classDiagram
class NombreClase{
  <<abstract>>
}
```

## Métodos abstractos

Los métodos abstractos deben marcarse con un asterisco `*` al final del nombre del método:

```mermaid
classDiagram
class Figura{
  <<abstract>>
  +calcularArea*() double
}
```

## Herencia

La relación de herencia debe representarse con:

```mermaid
classDiagram
ClasePadre <|-- ClaseHija
```

## Dependencia o uso

La relación de uso o dependencia debe representarse con:

```mermaid
classDiagram
ClaseEjecutora ..> ClaseBase : usa
```

## Agregación

La agregación puede representarse con:

```mermaid
classDiagram
ClaseContenedora o-- ClaseParte : agrega
```

## Composición

La composición puede representarse con:

```mermaid
classDiagram
ClaseTodo *-- ClaseParte : compone
```

---

# Estructura esperada del informe final

El informe final generado debe usar la siguiente estructura:

```md
# Informe de Revisión del Taller 8

## 1. Diagrama Mermaid extraído

```mermaid
classDiagram
```

## 2. Diagrama ideal propuesto

```mermaid
classDiagram
```

## 3. Retroalimentación del modelado

Texto breve de máximo una línea.

## 4. Retroalimentación de la implementación Java

Texto breve de máximo una línea.

## 5. Calificación

| Criterio | Nivel | Puntaje |
|---|---|---:|
| Modelado |  |  |
| Implementación |  |  |
| Resultados / Funcionalidad |  |  |
| Validación IA |  |  |
| **Total** |  | **/10** |

## 6. Retroalimentación general

Texto breve, claro y constructivo.
```

---

# Recomendación de uso

Este prompt debe utilizarse como apoyo para la retroalimentación formativa del Taller 8. Su finalidad es validar diagramas UML, revisar implementaciones Java y fortalecer el aprendizaje progresivo de Programación Orientada a Objetos mediante el uso responsable de herramientas de Inteligencia Artificial Generativa.

