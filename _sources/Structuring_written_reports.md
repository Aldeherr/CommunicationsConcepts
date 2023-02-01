Estructura de reportes escritos
---

- [Estructura de reportes escritos](#estructura-de-reportes-escritos)
  - [Tipos de reportes y Características](#tipos-de-reportes-y-características)
    - [Por información](#por-información)
    - [Por estructura](#por-estructura)
    - [Estructura para un journal](#estructura-para-un-journal)
    - [Estructura de reporte empresarial](#estructura-de-reporte-empresarial)
    - [Audiencia](#audiencia)
  - [Reproducción y referencias](#reproducción-y-referencias)
    - [Ventajas de la reproducibilidad](#ventajas-de-la-reproducibilidad)
    - [Buenas practicas](#buenas-practicas)
  - [Reportes claros y precisos](#reportes-claros-y-precisos)
    - [Frases vacías](#frases-vacías)
    - [Sustantivos concretos](#sustantivos-concretos)
  - [Caso de estudio: reporte sobre riesgo de crédito](#caso-de-estudio-reporte-sobre-riesgo-de-crédito)
    - [Story](#story)
    - [Tech or no tech](#tech-or-no-tech)
    - [Data](#data)
    - [Viz](#viz)
    - [Presentar](#presentar)


### Tipos de reportes y Características

Los reportes escritos también deben contener una estructura siempre y cuando seamos consientes de los datos y personas que recibirán la información.

- [x] Reporte como información

#### Por información
| Informativos                                                                                                                                                                   | Analíticos                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
| Escritos que llevan información actual descriptiva y corta, no poseen una estructura necesariamente e informan principal mente de los hechos actuales y tienen una estructura. | Incluyen distintos análisis entre los escritos como, recomendaciones o relaciones. Pueden variar de acuerdo al tamaño |


#### Por estructura 
- [x] Reporte como estructura


| Reporte Final| Reporte Summary |
| -------- | -------- |
| Incluye muchos detalles sobre el análisis, hallazgos y resultados asi como los visuales. Al ser un reporte largo, podemos utilizarlo para audiencias con gran conocimiento técnico. | Los reportes tipo resumen incluyen solo los insights mas importantes y las recomendaciones, asi como las visualizaciones. Este tipo de reporte es corto con menos de 5 paginas. Son un resumen del reporte final y pueden incluir enlaces del reporte principal. Los reportes summary están orientados a personas con toma de decision y que no necesariamente necesitan conocimiento técnico.       |


#### Estructura para un journal

<p align="center">
<img src="https://www.ijasrjournal.org/wp-content/uploads/2014/04/Research-2015-paper.jpg" width="600">
</p>


No hay una estructura 100% determinada; siempre depende de factores los factores que necesitemos cumplir. Aunque podemos basarnos en la siguiente estructura.

- Introducción
  - Propósito
    - Análisis del producto desde los reviews del website
    - Puntuar predicciones basadas en las opiniones
  - Información de contexto
    - Porque incremento los reviews negativos
  - Preguntas en el análisis
    - Factores que afectan a una mala experiencia de usuario
- Cuerpo
  - Datos
    - Descripción de las tablas
  - Métodos
    - Técnica utilizada (NLP y Random Forest)
  - Análisis
    - Visuales
      - Gráficas con las palabras mas comunes
  - Resultados
    - Descripción y visuales
      - 30 % de las malas puntuaciones están asociadas con la palabra "delay" y "shipping"
- Conclusiones
  - Replanteamos las preguntas del análisis
  - Resumir los resultados mas importantes


#### Estructura de reporte empresarial

- Contexto empresarial
- Regla de [1-3-25]
  - 1 pagina de abstracto
  - 3 paginas de resumen ejecutivo
  - 25 paginas de detalle

#### Audiencia

<p align="center">
<img src="https://53.fs1.hubspotusercontent-na1.net/hub/53/hubfs/know-your-audience-better.jpg?width=595&height=400&name=know-your-audience-better.jpg" width="600">
</p>




Siempre debemos tener en cuenta nuestra audiencia o los receptores de nuestro reporte. *Cada stakeholder* esta interesado en diferentes partes de nuestro reporte, por ello debemos adaptar todas estas cosas.

- Los ejecutivos querrán ver un reporte de rápida lectura con una introducción al problema y su conclusion.
- El equipo técnico solo hará un vistazo en el cuerpo del reporte. Queriendo validar y entender los métodos aplicados de nuestro análisis.

### Reproducción y referencias

La Reproducción y claridad de nuestros resultados es sumamente importante para nuestros resultados y conclusiones.

Por ejemplo, si un amigo pastelero cocina galletas de chocolates. Es muy probable que podamos crear las galletas en nuestra casa siempre y cuando tengamos la receta y los utensilios de cocina.

En el mundo de la data debemos ser capaces de obtener resultados idénticos aun con diferentes enviroments.


#### Ventajas de la reproducibilidad

- Previene la duplicación de esfuerzo
- Construir sobre herramientas pre existentes
- Nos concentra en nuevos retos
- Permite la revision en pares o de forma individual
- Agnóstica en cuanto a herramientas, ya sea en excel, tableau u otra, tendremos los mismos resultados.

#### Buenas practicas

1. Tener un track de como fueron generados los resultados
   1. Documentar correctamente los scripts
   2. Comentar el código
   3. Tener una lista de los paquetes utilizados y `env` utilizados.
   4. Usar programas de control de version.
2. Evitar la manipulación manual de la data.
   1. Importante versionar la data
   2. Guardar la data cruda y crear procesos intermedios
   3. Esto nos permite adaptarnos al problema
3. Tener control de la aleatoriedad (`randomness`)
   1. Establecer random seeds para pipelines de ML
   2. Usar variables para verificar los cambios en el modelo
4. Interpretabilidad
   1. El grado de facilidad de interpretación con que los stakeholders entiendan nuestro modelo
   2. Ayudan a la toma de decisiones
5. Citar bibliografías de forma correcta. 

**Para las citas bibliográficas podemos utilizar gestores de citas bibliográficas**


### Reportes claros y precisos

La escritura en la ciencia de datos debe tener estos cuatros elementos básicos.

- Conciso
- Preciso
- Evita el mal entendimiento y confusion
- Mensajes con sentidos


#### Frases vacías

Debemos evitar hablar con frases vacías.

- Es interesante notar que
- EL hecho de
- Es bien sabido que
- Cabe señalar que

Todos estos puntos conducen simplemente a una posible **distracción** a nuestro público, sin contenido. Por lo tanto debemos eliminar de nuestra presentación estas palabras.


Hecho directo| Frase Vacía | 
---------|----------|
 Las malas puntuaciones están asociadas con la palabra "retraso" y "envío" | Otro punto importante es el hecho de que las puntuaciones negativas están asociadas con las palabras "retraso" y "envío" | 
 

La Buena redacción técnica es concisa y directa. Por ello debemos escribir de forma concreta con pronombres y evitando el sobre uso de pronombres

- Eso
- Aquella
- Esto

#### Sustantivos concretos

El uso de sustantivo aporta una comunicación directa y de mejor comprensión. 

Sin sustantivo | Con sustantivo | 
---------|----------|
 Esto muestra una efectividad del 80% cuando predecimos los abandonos de clientes. | El modelo muestra una efectividad del 80% cuando predecimos los abandonos del cliente |
 
- La voz activa: hace énfasis en el autor
  - Se utiliza en entorno empresarial
- Voz pasiva: cargada y difícil de leer.
  - Se utiliza en un entorno académico

### Caso de estudio: reporte sobre riesgo de crédito

Veamos un paso a paso de como escribir un reporte de riesgo crediticio. Tengamos en cuenta que un riesgo crediticio cuantifica la probabilidad de que un cliente no cumpla con los pagos acordados. El banco **LOANME** desea predecir con anterioridad si un nuevo cliente tiende a fallar en sus letras. Tenemos los datos crudos disponibles y podemos ejecutar un EDA y realizar modelos para entrenamiento y evaluación.

#### Story

- Background: el porcentaje de clientes morosos aumento en los últimos 5 años.
  - Debemos predecir que clientes tienen una alta probabilidad de ser morosos.
- Insight: las personas con periodos de desempleo tienden a ser morosos
- Insight: las personas con ingresos bajos tienden a ser morosos
- Climax: predecir que personas serán morosos con un porcentaje de probabilidad del 95%.
- Next Steps: el ultimo paso consiste en realizar un ensayo controlado.

#### Tech or no tech

Realizar todas las traducciones técnicas a palabras no técnicas.

#### Data

- Audience persona
  - Director del departamento de finanzas
  - Intereses: decision en implementar un sistema automático de denegado.
  - Data apropiada:
    - Relaciones entre desempleados e ingresos y morosos
    - Porcentaje de clientes morosos desde hace seis meses.
- Estadística: Necesitamos algunos números agregados para poder parametrizar
  - Edad Media
  - Ingresos
  - Radio de cambio

#### Viz

- Un Gráfico de tipo boxplot vs condición de morosidad; mostrará la condición de los clientes y sus rangos.

- Un gráfico lineal con el porcentaje de cambio en los clientes morosos durante los próximos meses.


#### Presentar

- Quien? Director de Departamento de Finanzas
- Porque? importante decision a tomar
- Contenido: Hallazgos importantes y recomendaciones
- Canal:  enviar los resultados antes de la reunion

