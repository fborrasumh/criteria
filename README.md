# CriterIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22171873.svg)](https://doi.org/10.5281/zenodo.22171873)

**Aplicación:** https://fborrasumh.github.io/criteria/

Ayuda al estudiantado universitario a usar la inteligencia artificial en sus trabajos **con criterio**: muestra qué permite cada tarea, deja constancia de lo que se hace, comprueba que las referencias existen y genera la **declaración de uso de IA** que va en el trabajo. Funciona entera sin clave de IA. Aplicación de un solo fichero (`index.html`), sin servidor.

**Idiomas de la interfaz:** español (por defecto), inglés y portugués; selector en la barra superior o `?lang=en` / `?lang=pt` en la URL. La declaración puede ir en un idioma distinto del de la interfaz.

## Novedades de la versión 3.0

- Reconstruida con el sistema Forja: interfaz completa en **español, inglés y portugués** (pasos, niveles, casos de práctica, avisos y ejemplo).
- **Pulir la redacción con OpenAI, Google Gemini o Anthropic Claude** (antes solo OpenAI), con desplegable de los modelos de la propia clave, aviso previo con la muestra de lo que se envía y datos personales enmascarados. **El código comprueba la versión pulida**: avisa si añade cifras o herramientas, si quita alguna herramienta usada, si pierde la cabecera o la tabla de usos, y permite volver a la versión base.
- **Referencias más honestas:** un fallo de conexión ya no se presenta como «no existe», sino como «sin comprobar».
- **Word generado en el propio navegador**, sin librerías externas ni red.
- Datos en IndexedDB, con exportación e importación en JSON. Los datos de las versiones 1 y 2 se recuperan solos.
- El ejemplo se guarda aparte y nunca se mezcla con el trabajo propio.
- Bitácora exportable también a CSV; herramienta libre («Otra herramienta…»).

## Qué hace

1. **Tu trabajo:** nombre, asignatura, tipo de trabajo, idioma de la declaración (es/en/pt) y estilo de cita (APA 7, Vancouver, Harvard).
2. **Nivel de uso:** cinco niveles, de 0 (sin IA) a 4 (IA integral), con lo que se puede, lo que no y lo que hay que guardar. Correo al profesor ya redactado para cuando el enunciado no dice nada.
3. **Bitácora:** herramienta, versión, uso, petición y qué se hizo con la respuesta. Avisa al anotar un uso que supera el nivel de la tarea y lo marca en la tabla. Exporta el anexo (.md) y CSV.
4. **Referencias:** comprueba cada referencia en **Crossref** (si el DOI existe y si apunta al trabajo citado; búsqueda bibliográfica si no hay DOI) y en **OpenAlex** (retractaciones). Informe descargable.
5. **Declaración:** se redacta a partir del nivel, la bitácora y las referencias, en tres extensiones y cuatro ubicaciones; incluye la **cita de cada herramienta**. Control de coherencia antes de declarar. Word, Markdown o copiar.
6. **Entrenar:** 14 situaciones reales con explicación, sin IA.
7. **Enlace para el profesorado:** el docente fija el nivel de su tarea y comparte un enlace que abre la app con ese nivel marcado, junto al texto para el enunciado o la guía docente.

## Cómo se usa la IA

Es opcional y solo sirve para **pulir la redacción** de la declaración, con la clave de cada persona (OpenAI, Google Gemini o Anthropic Claude). La IA propone; el código compara la versión pulida con la base (cifras, herramientas, cabecera y tabla) y avisa de cualquier diferencia de contenido.

## Privacidad

- Se guarda solo en el navegador (IndexedDB): el trabajo, la bitácora, las referencias, la declaración y, si se pone, la clave de IA.
- Las referencias que se comprueban se envían a Crossref y OpenAlex (bases públicas, sin clave).
- Solo si se pulsa «Pulir» y se confirma en el aviso previo, el texto de la declaración va al proveedor de IA elegido, con correos, DNI/NIE, teléfonos y el nombre del estudiante enmascarados.
- El JSON exportado no contiene claves.

## Límites

- CriterIA **no decide** qué está permitido: lo decide el profesorado y la normativa de cada universidad. Los niveles son una guía.
- Un libro, una tesis o unas actas pueden no estar en Crossref y ser reales; una referencia que existe puede no decir lo que se cita. Hay que abrirlas y leerlas.
- La comprobación de la versión pulida detecta cifras y herramientas añadidas o quitadas, no cambios sutiles de matiz: la declaración hay que leerla antes de usarla.
- La app no detecta si un texto está escrito con IA ni sustituye a la normativa de integridad académica.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche).

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

Borrás Rocher, F. (2026). *CriterIA* (versión 3.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.22171873

El DOI anterior es el de concepto: apunta siempre a la última versión. El DOI de cada versión concreta está en [Zenodo](https://doi.org/10.5281/zenodo.22171873). GitHub ofrece la cita en APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
