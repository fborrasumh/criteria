# CriterIA

**Usar IA en tus trabajos con criterio.** Alfabetización en inteligencia artificial
generativa para estudiantes universitarios. Aplicación web de un único fichero HTML.

👉 https://fborrasumh.github.io/criteria/

## Por qué

El catálogo tenía material de alfabetización en IA para el profesorado (100 Conceptos,
25 Conceptos), pero nada equivalente para el alumnado. Y lo que un estudiante necesita
no es un glosario: es saber **qué le permite cada profesor**, **cómo comprobar que lo que
le devuelve el modelo es cierto** y **cómo declararlo** sin jugarse la asignatura.

## Funciona sin clave de API

Los niveles de uso, la verificación de referencias contra Crossref, la bitácora, la
declaración y el entrenamiento no necesitan clave de OpenAI ni cuenta de nada. La clave
es opcional y solo pule la redacción de la declaración.

## Qué hace

| Pestaña | Función |
|---|---|
| **Qué puedo usar** | Cinco niveles de uso, del 0 (sin IA) al 4 (la IA es el objeto de la tarea). Para cada uno: qué puedes hacer, qué no, y qué evidencia guardar. |
| **Verificar referencias** | Pega la bibliografía que te ha dado un modelo y comprueba contra Crossref, en directo, si cada trabajo existe. Distingue tres casos: existe y coincide, **el DOI existe pero apunta a otro trabajo** (el fallo más típico de las citas inventadas) y no se localiza. |
| **Bitácora** | Registro de qué le pediste a la IA y qué hiciste con la respuesta. Exportable como anexo. |
| **Declaración** | Genera el párrafo de declaración de uso a partir del nivel elegido y de la bitácora, en tres formatos. |
| **Entrenar** | Catorce situaciones reales de clase con explicación razonada. Sin conexión a ninguna IA. |

## Los cinco niveles

| | Nivel | Qué significa |
|---|---|---|
| 0 | Sin IA | La tarea mide algo que la IA haría por ti. |
| 1 | IA para explorar | Antes de escribir. Nada suyo llega al texto. |
| 2 | IA para asistir | Ayuda en la redacción; las ideas y la estructura son tuyas. |
| 3 | IA para colaborar | Trabajo conjunto. Se evalúa también cómo lo has dirigido. |
| 4 | IA integral | El uso es el objeto de la tarea; lo evaluado es tu criterio. |

Quien fija el nivel es el profesor, no la aplicación.

## Para el profesorado

Se puede usar de tres maneras: como lectura previa a la primera entrega de la asignatura,
como material de una sesión sobre integridad académica, o indicando en el enunciado
el nivel de uso que se aplica a cada tarea (`Nivel 2 de CriterIA`) para que el alumnado
sepa exactamente a qué atenerse.

## Uso responsable

La app promueve declarar el uso, no ocultarlo. No genera texto para entregar, no evade
detectores y no sustituye ninguna tarea evaluable.

## Fuentes de datos

- [Crossref](https://www.crossref.org) — verificación de referencias.
- [OpenAI API](https://platform.openai.com) — opcional, solo para pulir la declaración.

## Licencia

MIT — Fernando Borrás Rocher, Universidad Miguel Hernández de Elche.
