# Contribuir a Versat Labs

[English](CONTRIBUTING.md) | [Português](CONTRIBUTING.pt.md) | [Español](CONTRIBUTING.es.md)

Quienes desarrollan, diseñan arquitectura, hacen diseño o contribuyen de otras formas pueden ayudar a planificar o implementar una issue existente, proponer una nueva o mejorar la calidad. Elige el repositorio y lee su README, AGENTS.md y pautas disponibles. El CONTRIBUTING.md propio del repositorio tiene prioridad sobre estos valores predeterminados de la organización.

## Comenzar una contribución

Abre **Issues → New issue** en el repositorio destino y usa el formulario disponible de bug, funcionalidad o mantenimiento. Describe problema, contexto y resultado esperado; incluye reproducción para bugs. Puedes contribuir con una issue bien definida sin implementarla. Antes de trabajar en archivos, sigue preparación, especificaciones y validación del repositorio. En el PR, vincula la issue, explica el cambio e informa comprobaciones reales y validaciones no disponibles.

## Instalar el plugin Versat AI Harness

El plugin `versat-ai-harness` proporciona Skills reutilizables y orientación para planificar, implementar y validar contribuciones con Codex. Sigue la ruta de instalación correspondiente a tu cuenta. Los nombres de los menús siguientes se muestran en inglés.

### Miembros del workspace de Versat

1. En Codex, selecciona el workspace de Versat y abre **Settings > Plugins > Browse Directory > Versat**.
2. Abre **Versat-ai-harness** y selecciona **Install**.

La administración del workspace gestiona la distribución. Si el plugin no aparece o la instalación no está disponible, contacta con el administrador del workspace.

### Colaboradores externos

Si tu cuenta de Codex no forma parte del workspace de Versat:

1. Abre **Settings > Plugins > Add > Add Marketplace**.
2. En **Source**, introduce la URL del repositorio del Harness: [https://github.com/versat-labs/versat-ai-harness](https://github.com/versat-labs/versat-ai-harness).
3. Confirma que deseas añadir el marketplace. En el marketplace **Versat Plugins** añadido, busca `versat-ai-harness` y selecciona **Install**. Añadir el marketplace e instalar el plugin son pasos separados.

**Actualiza manualmente con cada nueva versión.** Lee las instrucciones de la versión y comprueba la compatibilidad con tu proyecto, actualiza el marketplace añadido y actualiza el plugin instalado mediante los controles disponibles en tu versión de Codex. Confirma la versión instalada en un chat nuevo antes de continuar; actualizar solo el catálogo no confirma la actualización del plugin. Si la versión seleccionada no está disponible o la actualización falla, contacta con los mantenedores del Harness antes de continuar con esa versión.

El repositorio del Harness es público. El acceso al repositorio en el que deseas contribuir es independiente de la instalación del plugin.

## Empezar a usar el plugin

1. Clona o abre el repositorio destino como proyecto en Codex. Lee su README, AGENTS.md y las pautas de contribución.
2. Inicia un chat nuevo después de instalar o actualizar el plugin y pide a Codex que compruebe la preparación:

   ```text
   Confirma la carpeta actual del proyecto, la versión instalada de versat-ai-harness y dónde encontraste su Skill versat-sdd y los recursos canónicos correspondientes. Informa de cualquier prerrequisito que falte antes de modificar archivos.
   ```

3. Una vez confirmada la preparación, usa una issue real para solicitar el plan inicial. Sustituye los campos siguientes:

   ```text
   Usa $versat-sdd para planificar el cambio <change-name> de la issue <issue-url>: <describe el problema y el resultado esperado>. Crea solo Proposal y Requirements; no implementes. Detente para la revisión del Gate 1.
   ```

Espera los archivos `specs/changes/<change-name>/proposal.md` y `requirements.md`, escritos en inglés. Revísalos antes de aprobar la siguiente etapa. Design y Tasks siguen sus respectivos gates de aprobación; la implementación requiere una solicitud explícita después de la revisión de Tasks. Si faltan la Skill o sus recursos, resuelve la instalación con el administrador del workspace o los mantenedores del Harness antes de continuar.

## Guías del Harness

Estos enlaces apuntan a la documentación mantenida del Harness en `main`; sigue la documentación correspondiente a la versión instalada cuando trabajes en un proyecto versionado. También puedes proponer una issue mediante la vía pública de contribución sin instalar el plugin.

- [Primer uso](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/quickstart.es.md)
- [Preparar el entorno](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/workspace-setup.es.md)
- [SDD y aprobaciones](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/sdd-with-codex.es.md)
- [Entrega mediante GitHub](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/github-delivery.es.md)
- [Validación](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/validation-and-evaluations.es.md)
- [Política canónica de idiomas (inglés)](https://github.com/versat-labs/versat-ai-harness/blob/main/standards/core/language.md)

## Derechos y procedencia

Antes de proponer código, texto o recursos, identifique su origen, los permisos aplicables y los avisos exigidos. Si no puede acreditar el permiso para contribuir una ilustración, omítala y consulte al responsable del repositorio; una issue o revisión técnica no aporta derechos ausentes. Siga los términos efectivos del repositorio de destino. El permiso para usar una herramienta interna de desarrollo es distinto de la licencia del proyecto de destino, e instalar esa herramienta no es un requisito para la contribución pública descrita arriba. Esta guía no introduce CLA, DCO ni cesión de derechos.

## Informes de seguridad

Para bugs comunes, usa Bug report. Para sospechas de vulnerabilidad en repositorios públicos, usa Private Vulnerability Reporting de GitHub cuando esté habilitado. En los privados, envía email a los CODEOWNERS pertinentes por los canales internos existentes de Versat. No divulgues detalles de vulnerabilidades en issues comunes. Consulta [reportes de seguridad](SECURITY.es.md) para encaminamiento y recuperación cuando el canal no esté disponible.
