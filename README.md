# Taller 8 - DOO e implementación de soluciones UML y Java, basados en Polimorfismo - GRUPAL

## Elaboración de ejercicios sobre Polimorfismo a través de Diagramas UML
## Elaboración de ejercicios mediante código haciendo uso del concepto de Polimorfismo en Programación Orientada a Objetos

* Leer detenidamente cada problemática propuesta.
* Usar el programa **DIA-UML** _(Open source)_ para generar la representación de su solución _(modelado)_, vía diagramas de clases.
* Para cada diagrama/solución _(modelado de su solución)_, genere/agregue 2 archivos _(fuente e img: \*.dia y \*.png \*.jpeg, etc)_. No olvide titular a cada clase, con el nombre representativo del análisis/solución. Para el nombre de cada archivo use el formato: _Problema-NroProbl_NombClase_. Ejemplo **Problema-1_Trabajador**. Todos estos archivos agréguelos en el subDirectorio: **Modelos_UML**
* En el subDirectorio **Solucion_Codigo** cree un único proyecto NetBeans - _Java Aplication_ (o con el IDE de su preferencia) y en él, agregue todas las clases necesarias para la solución de cada problema _(no use paquetes)_. Y para facilitar la revisión, utilice para la clase base el formato _Problema-NroProbl_NombClaseBase_, y para la clase de prueba/ejecutor use _Problema-NroProbl_NombClaseEjecutor_ (Ésta última es la clase de prueba que genera/instancia con objetos cada entidad/clase y verifica su funcionalidad). 
* Respete la arquitectura **MVC**, es decir, no implemente entradas/salidas desde/hacia teclado-consola directamente en la clase base. Los datos de entrada y resultados deben ser ingresados/mostrados desde/hacia teclado-consola, en la clase de prueba/ejecutor.
* Para retornar los datos del objeto, usar el método _**toString()**_, vía cadena con formato legible. 
___

## Problema 1 - Juego de roles

En un juego de rol, se desea implementar un sistema de combate en el que participen diferentes tipos de **personajes**: **guerreros**, **magos** y **arqueros**. Cada personaje tiene atributos y habilidades únicas, así como diferentes métodos de _ataque_ y _defensa_.

El objetivo del juego es enfrentar a los personajes en batallas y determinar el ganador en función de sus habilidades, estrategias y atributos. Los **guerreros** se destacan por su fuerza y habilidades cuerpo a cuerpo, los **magos** por sus hechizos y poderes mágicos, y los **arqueros** por su precisión y habilidades a distancia.

El sistema debe permitir crear nuevos personajes de cada tipo, asignarles atributos iniciales, como _puntos de vida_ y _nivel de experiencia_, y permitirles _subir de nivel_ a medida que ganan batallas. Además, se debe implementar un algoritmo de combate que evalúe las habilidades de cada personaje y determine el resultado de la batalla.

Utilizando programación orientada a objetos, herencia y polimorfismo, implementa el sistema de combate y las clases necesarias para representar a los diferentes tipos de personajes. Asegúrate de que cada tipo de personaje tenga sus propias habilidades y métodos de ataque y defensa, y que puedan interactuar entre sí en las batallas.

> [!Note]
> Para solucionar lo anterior se debe generar lo siguiente:
> 
> - Un diagrama exclusivo que involucren las funcionalidades principales del juego.
> - Una solución en lenguaje de programación Java. Usar Polimorfismo en la solución.
> - Clase de prueba/ejecutor, que demuestre la funcionalidad del juego.


## Problema 2 - Restaurant

En un restaurant se tiene diferentes tipos de **menú** para ofrecer a los clientes. Una cuenta por pagar está compuesta por características como: _nombre del cliente, listado de todos las cartas(menú) solicitados por el cliente, valor a cancelar total, subtotal, Iva._

Los tipos de menú del restaurant son:

**Menú a la carta**

- nombre del plato
- valor del menú
- valor inicial del menú
- valor de porción de guarnición
- valor de bebida
- porcentaje adicional por servicio en relación del valor inicial del menú

**Menú del día**

- nombre del plato
- valor del menú
- valor inicial del menú
- valor de postre
- valor de bebida

**Menú de niños**

- nombre del plato
- valor del menú
- valor inicial del menú
- valor de porción de helado
- valor de porción de pastel

**Menú económico**

- nombre del plato
- valor del menú
- valor inicial del menú
- porcentaje de descuento, en referencia al valor inicial del menú

> [!Note]
> Para solucionar lo anterior se debe generar lo siguiente:
> 
> - Un diagrama exclusivo que involucren las clases de tipo Menú (usar polimorfismo)
> - Una solución en lenguaje de programación Java. Usar Polimorfismo en la solución.
> Hacer uso del método **_toString()_** para presentar toda la información posible del objeto (nombre del cliente, subtotal, iva, listado de todos los menú, valor a cancelar a total.


## Problema 3 - Juego de fútbol "Estadísticas"

Se desea realizar una aplicación que permita a un periodista deportivo llevar las estadísticas de los jugadores de un equipo de fútbol para poder valorar su actuación en el partido.

Cada jugador se identifica por su nombre, número de dorsal
y Rut

Los jugadores se dividen en **tres categorías**:

1. **Atacantes**
2. **Defensores**
3. **Porteros**

Para todos los jugadores se desea contabilizar el número de goles marcados, además en el caso de los jugadores de campo se contabilizan los pases realizados con éxito y el número de balones recuperados. En el caso de los porteros se contabilizan las atajadas realizadas.

### Valoración del jugador

**Cálculo base para todos los jugadores:**

- `valor_goles = goles * 30`

**Valor adicional según tipo de jugador:**

1. **Atacantes**
   - `valor += recuperaciones * 3`

2. **Defensores**
   - `valor += recuperaciones * 4`

3. **Porteros**
   - `valor += atajadas * 5`

> [!Note]
> Se debe aplicar polimorfismo mediante la aplicación de herencia, encapsulamiento de atributos y comportamientos comunes, y especializar comportamiento según el tipo de jugador. 

## Problema 4 - Sistema de monitoreo de impactos del cambio climático en Ecuador

Una red de monitoreo ambiental tiene como objetivo registrar, analizar y reportar los impactos del cambio climático en diferentes regiones. En cada ubicación se instalan dispositivos capaces de medir distintos indicadores climáticos como temperatura, precipitación, calidad del aire, y humedad del suelo. Dependiendo de la región (costa, sierra y oriente), los dispositivos pueden variar en capacidades y protocolos de recolección.

Los datos recolectados deben almacenarse y analizarse periódicamente. Además, ciertas ubicaciones requieren generar reportes personalizados que destaquen riesgos ambientales como sequías, deslizamientos o contaminación del aire. Algunos dispositivos pueden comportarse de forma especializada para detectar únicamente ciertos tipos de indicadores dependiendo de la región (costa, sierra y oriente). 

### Requisitos funcionales:

- Representar diferentes tipos de dispositivos y sus especializaciones, para la costa, sierra y oriente. 
- Implementar métodos polimórficos que permitan procesar los datos según los tipos de dispositivos y sus especializaciones, para la costa, sierra y oriente.
- Generar reportes dinámicos en función del tipo de riesgo ambiental detectado según la región

> [!Note]
> Plantee una solución polimórfica dada una jerarquía de clases con ventajas de herencia. Y para la generación de reportería, use los toString() base. 

## Problema 5 - Plataforma de apoyo a emprendimientos en Loja

Una organización local ha creado una plataforma digital para registrar y promover emprendimientos de la ciudad de Loja. Los emprendimientos pueden clasificarse por tipo (tecnológico, artesanal, agrícola, gastronómico, etc.), y cada uno presenta información detallada sobre su misión, productos o servicios, y datos de contacto.
Algunos emprendimientos requieren acompañamiento técnico por parte de mentores especializados, quienes brindan asesoría en áreas como marketing, contabilidad o desarrollo de software. Además, los emprendimientos pueden participar en ferias locales, donde presentan sus productos y compiten por reconocimientos. Existen emprendimientos que evolucionan a lo largo del tiempo y extienden sus líneas de productos o abren nuevas sedes.

### Requisitos funcionales:

- Diferenciar los distintos tipos de emprendimientos mediante herencia.
- Asociar uno o más mentores a los emprendimientos que lo requieran.
- Implementar comportamientos polimórficos en función del tipo de feria o actividad en la que participan.
- Permitir registrar productos o servicios que ofrece cada emprendimiento.
- Simular la evolución de un emprendimiento con el tiempo (crecimiento, diversificación, expansión).

> [!Note]
> Plantee una solución polimórfica dada una jerarquía de clases con ventajas de herencia. Para la visualización de resultados use los toString() base. 

## Problema 6 - Simulador de Conflictos Bélicos Mundiales 2025 - Versión 2.0

Con el objetivo de dar continuidad al “Simulador de Conflictos Bélicos Mundiales 2025” desarrollado por usted en el primer bimestre, la **ONU** le solicita desarrollar la **versión 2.0** de este simulador en el lenguaje de alto nivel orientado a objetos **Java**, considerando sus **cuatro pilares fundamentales**: **abstracción, encapsulamiento, herencia y polimorfismo**, cumpliendo con los siguientes lineamientos:

## Requisitos Funcionales

- Cada **nación** debe ser representada con:
- Nombre de la nación
- Número de habitantes
- Cantidad de recursos económicos disponibles
- Nivel de poder militar (valor entre 1 y 100)
- Estado de conflicto (si está en conflicto o no)
- Otros datos complementarios que se consideren necesarios

- Implementar métodos y/o constructores para procesar esta información conforme a los requerimientos.

### Naciones Desarrolladas

- Se debe indicar si la nación dispone de **tecnología avanzada**.
- Implementar un **cálculo del impacto**, que considera un **bono de tecnología** para el incremento de su poder militar.
- Si el bono supera el límite permitido, se debe asignar directamente el valor de **100** como poder militar máximo.

### Naciones en Vías de Desarrollo

- Se debe registrar su **nivel de recursos limitados** (recursos económicos y poder militar por cada N habitantes).
- Implementar el **cálculo del impacto**, que **reduce el impacto** del conflicto en función de sus recursos limitados.
- Se permite libertad para definir un **modelo matemático o estadístico personalizado** para este cálculo.

### Naciones Aliadas

- Tanto para naciones desarrolladas como en vías de desarrollo, pueden contar con **naciones aliadas**.
- Las alianzas afectan directamente el **nivel de impacto**, incrementándolo o reduciéndolo, pero **solo si existen aliados disponibles**.

### Simulación de Conflictos

- El programa debe permitir **declarar conflictos** entre dos naciones seleccionadas mediante un **proceso aleatorio**.
- Utilizar **polimorfismo** para implementar el **cálculo de impacto** y determinar las consecuencias del conflicto.

### Consecuencias del Conflicto

- Reducción del **5% de población** por cada diferencia en los niveles de poder militar.
- Reducción del **10% de recursos** de la nación derrotada.
- Si las naciones tienen el **mismo nivel de poder militar**, ambas pierden el **5% de recursos**.

> [!Note]
>  Reporte Final
>  - Al finalizar la simulación, debe generarse un **reporte general** que contenga:
>  - Estado actual de cada nación (población, recursos, estado de conflicto, etc.)
>  - **Total de conflictos** simulados entre N naciones.