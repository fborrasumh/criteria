# CriterIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22171873.svg)](https://doi.org/10.5281/zenodo.22171873)

**Aplicación:** https://fborrasumh.github.io/criteria/

Ayuda al estudiantado universitario a usar la inteligencia artificial en sus trabajos **sin jugársela**. Muestra qué permite cada tarea, deja constancia de lo que se hace, comprueba que las referencias existen y genera la **declaración de uso de IA** que va en el trabajo. Funciona entera sin clave de IA y los datos no salen del navegador. Aplicación de un solo fichero (`index.html`), sin servidor.

## Novedades de la versión 2.0

- Recorrido guiado con el estilo de Forja: tu trabajo, nivel, bitácora, referencias, declaración y entrenamiento. Incluye un ejemplo completo que no se guarda.
- **Control de coherencia**: avisa al anotar un uso que supera el nivel permitido, lo marca en la bitácora y lo recuerda antes de declarar. También avisa de las entradas sin verificar a partir del nivel 2 y de la bibliografía buscada con IA sin comprobar.
- **Declaración en español, portugués e inglés**, en tres extensiones y cuatro ubicaciones. Menciona la verificación de referencias cuando se ha hecho. Se exporta a Word con el anexo de la bitácora, a Markdown o para copiar. Con clave, la IA pule la redacción sin añadir hechos.
- **Cita de cada herramienta** en APA 7, Vancouver o Harvard, con modelo, versión y tipo (modelo de lenguaje, traductor automático o asistente de escritura).
- **Referencias verificadas en Crossref y OpenAlex**, con detección de retractaciones.
- **Enlace para el profesorado**: el docente fija el nivel de su tarea y comparte un enlace que abre la app con ese nivel marcado, junto al texto para el enunciado o la guía docente.
- **Correo al profesor** ya redactado para cuando el enunciado no dice qué nivel se aplica.
- Los datos guardados con la versión 1 se conservan.

## Los cinco niveles

| Nivel | Uso | En resumen |
|---|---|---|
| 0 | Sin IA | La tarea mide algo que la IA haría por ti. |
| 1 | IA para explorar | Antes de escribir; nada de lo que produzca acaba en el texto. |
| 2 | IA para asistir | Ayuda a redactar y revisar; las ideas y la estructura son tuyas. |
| 3 | IA para colaborar | Trabajo conjunto que se dirige, se critica y se reescribe. |
| 4 | IA integral | El uso es el objeto de la tarea; se evalúa el criterio al supervisarla. |

Quien decide el nivel es el profesorado, no esta app.

## Privacidad

Los datos se guardan en `localStorage` del navegador (`criteria_state`). Las referencias se consultan en Crossref y OpenAlex. Solo si se pone una clave de OpenAI, el texto de la declaración viaja a `api.openai.com` para pulirlo.

## Cómo citar

Borrás Rocher, F. (2026). *CriterIA* (versión 2.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.22171873

El DOI anterior es el de concepto: apunta siempre a la última versión. El DOI de cada versión concreta está en [Zenodo](https://doi.org/10.5281/zenodo.22171873). GitHub ofrece la cita en formato APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
