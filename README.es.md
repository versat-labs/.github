# Versat Labs · Valores predeterminados de la organización

[English](README.md) | [Português](README.pt.md) | [Español](README.es.md)

El inglés es la fuente canónica de este README. Las traducciones al portugués y al español se mantienen junto con ella, siguiendo la convención de idiomas de Versat AI Harness para la documentación dirigida a la comunidad.

## Objetivo

Versat Labs mantiene `versat-labs/.github` para centralizar el perfil público de la organización, las pautas de contribución predeterminadas y las plantillas de issues. Sigue la convención de GitHub para el repositorio especial `.github`, lo que permite que los repositorios de la organización compartan recursos coherentes para las contribuciones.

Este repositorio contiene metadatos de la organización y documentación. No tiene una aplicación ejecutable, un proceso de compilación ni una suite de pruebas automatizadas.

## Cómo utiliza GitHub este repositorio

- GitHub muestra `profile/README.md` en el perfil público de la organización. Consulta la [documentación sobre el perfil de la organización](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile).
- `CONTRIBUTING.md` proporciona las pautas predeterminadas cuando un repositorio no tiene su propia guía de contribución.
- La carpeta `.github/ISSUE_TEMPLATE/` proporciona los formularios de issues predeterminados. Las plantillas válidas o la configuración de plantillas propias de un repositorio sustituyen toda la carpeta predeterminada.
- GitHub hace referencia a estos recursos sin copiarlos a los repositorios que los utilizan. Consulta la [documentación sobre archivos predeterminados de la comunidad](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

`AGENTS.md` y `.gitignore` se aplican a este repositorio; GitHub no los distribuye como valores predeterminados de la organización.

## Guía de archivos

| Archivo | Finalidad |
| --- | --- |
| [README.md](README.md) | Descripción general canónica en inglés de este repositorio, sus archivos y el flujo de mantenimiento. |
| [README.pt.md](README.pt.md) | Traducción de esta descripción general al portugués. |
| [README.es.md](README.es.md) | Traducción de esta descripción general al español. |
| [profile/README.md](profile/README.md) | Perfil público de la organización: misión, visión, áreas de trabajo, formas de contribuir y recursos útiles de Versat Labs. |
| [CONTRIBUTING.md](CONTRIBUTING.es.md) | Entrada para contribuir y enlaces a las guías mantenidas en el Harness. |
| [AGENTS.md](AGENTS.md) | Instrucciones para agentes que trabajan en este repositorio, incluidos el alcance, las convenciones de edición y los requisitos de validación. |
| [.gitignore](.gitignore) | Excluye del control de versiones los archivos del entorno local, la configuración de editores, los logs y los artefactos generados; permite `.env.example`. Estos patrones no implican que existan herramientas de compilación en este repositorio. |
| [.github/ISSUE_TEMPLATE/bug_report.yaml](.github/ISSUE_TEMPLATE/bug_report.yaml) | Formulario para informar de errores. Requiere una descripción, los pasos para reproducir el error y el comportamiento esperado; también incluye campos para capturas de pantalla, detalles de los dispositivos y contexto adicional. Utiliza el prefijo de título `fix: ` y el tipo de issue `Bug`. |
| [.github/ISSUE_TEMPLATE/chore.yaml](.github/ISSUE_TEMPLATE/chore.yaml) | Formulario de mantenimiento. Requiere una descripción, el alcance y los criterios de finalización. Utiliza el prefijo de título `chore: ` y el tipo de issue `Task`. |
| [.github/ISSUE_TEMPLATE/feature_request.yaml](.github/ISSUE_TEMPLATE/feature_request.yaml) | Formulario para solicitar funcionalidades. Requiere el problema, el trabajo que se busca realizar y los perfiles de usuario y comprador, con contexto adicional opcional. Utiliza el prefijo de título `feat: ` y el tipo de issue `Feature`. |

Los tres formularios declaran `versat-labs/1` en el metadato `projects`.

## Cómo utilizar los recursos de contribución

Abre el repositorio al que deseas contribuir, lee sus pautas de contribución y selecciona **Issues → New issue**. Cuando se apliquen los valores predeterminados de la organización, elige el formulario de error, funcionalidad o mantenimiento, completa los campos obligatorios y envíalo. La issue resultante reúne la información necesaria para comenzar la planificación. Las pautas específicas del repositorio tienen prioridad.

## Mantenimiento de este repositorio

Lee [CONTRIBUTING.md](CONTRIBUTING.es.md) y [AGENTS.md](AGENTS.md) antes de editar. Mantén alineadas las tres versiones del README siempre que cambie su contenido.

Las instrucciones detalladas de desarrollo se mantienen en la [guía SDD del Harness](https://github.com/versat-labs/versat-ai-harness/blob/27735687a37e896cd6b0c95cd9d2d848ee166d90/docs/user-docs/guides/sdd-with-codex.es.md) (requiere acceso privado). Sigue el AGENTS.md de este repositorio para revisión y verificaciones locales. Los colaboradores públicos pueden comenzar por [CONTRIBUTING.es.md](CONTRIBUTING.es.md).

### Validación

Comienza por los requisitos de validación de [AGENTS.md](AGENTS.md):

1. Revisa el diff y ejecuta `git diff --check`.
2. Para Markdown, comprueba los encabezados, el formato, los enlaces y la correspondencia entre traducciones. Previsualiza el contenido público cuando el diseño sea relevante.
3. Para los formularios de issues modificados, analiza el YAML y verifica las claves obligatorias, la unicidad de los IDs de los campos, los indicadores de obligatoriedad, los prefijos de los títulos, los tipos de issue y los metadatos del proyecto. Comprueba el formulario en GitHub cuando el comportamiento no pueda verificarse localmente.
4. Indica en el pull request los cambios, las comprobaciones realizadas y cualquier validación que no se haya podido completar.
