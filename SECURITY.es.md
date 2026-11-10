# Reportes de seguridad

[English](SECURITY.md) | [Português](SECURITY.pt.md) | [Español](SECURITY.es.md)

Sigue las instrucciones de seguridad propias del repositorio destinatario cuando existan. Los bugs funcionales comunes corresponden al formulario de issue **Bug report**. No divulgues sospechas de vulnerabilidades en issues, discusiones ni pull requests públicos.

Los CODEOWNERS pertinentes son responsables de supervisar, clasificar y coordinar la resolución de reportes de seguridad de sus componentes, tanto mediante PVR en repositorios públicos como por email interno en los privados. Los mantenedores configuran los permisos y notificaciones necesarios; la asignación en CODEOWNERS no configura por sí sola la recepción en GitHub.

## Repositorios públicos

Usa **Security and quality → Report a vulnerability** en el repositorio público afectado cuando Private Vulnerability Reporting esté habilitado. Envía versión afectada, resumen, reproducción segura e impacto mediante ese formulario privado. Los reportes pueden escribirse en inglés, portugués o español. No incluyas secretos, datos de clientes ni adjuntos sensibles innecesarios.

La organización proporciona un formulario predeterminado `.github/VULNERABILITY_REPORT.yml`; el formulario propio del repositorio tiene prioridad. Una plantilla no habilita la función ni acredita que responsables la supervisen. Si la opción privada está ausente o no está disponible, solicita instrucciones privadas a un mantenedor sin revelar la vulnerabilidad. No sustituyas esa ruta por un issue común con detalles de seguridad.

## Repositorios privados

Envía email a los **CODEOWNERS** pertinentes mediante los canales internos existentes de Versat. Identifica a los responsables de las rutas afectadas en el archivo CODEOWNERS y obtén sus emails del directorio interno o de un contacto interno establecido. No deduzcas emails desde nombres de usuario de GitHub ni publiques contactos internos.

Si falta CODEOWNERS, la responsabilidad no está clara o no tienes acceso a contactos internos, solicita instrucciones privadas al mantenedor o a tu contacto existente en Versat sin revelar detalles sensibles. Un issue en un repositorio privado no sustituye esta ruta: su público puede exceder a los destinatarios previstos.

## Recepción y alcance

Esta política no concede acceso a repositorios privados ni permiso para realizar pruebas. No promete plazo de respuesta ni monitoreo continuo. Los mantenedores deben establecer destinatarios permitidos, notificaciones y recepción real antes de afirmar que la ruta está verificada. Conserva privados los detalles durante la coordinación de la corrección.
