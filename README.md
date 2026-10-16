# RetailMax Analytics

## Qué se versiona

Se versionan scripts, notebooks exportados, configuraciones sin secretos, definiciones de pipelines, infraestructura Terraform, migraciones SQL y documentación.

## Qué no se versiona y por qué

- Datos reales y modelos grandes: evita aumentar el repositorio y exponer información sensible.
- Contraseñas, tokens y credenciales: se gestionan mediante un gestor de secretos.
- Entornos virtuales, cachés y archivos temporales: pueden regenerarse.
- Estado y planes de Terraform: pueden contener información sensible.

## Versionado de la procedencia de datos

Cada ejecución debe registrar la fuente, fecha de extracción, versión o snapshot del dataset, transformaciones aplicadas, versión del esquema, reglas MDM, parámetros y versión del modelo.
Git guarda las definiciones y referencias sin datos sensibles, mientras que el almacenamiento externo conserva las versiones de datos y modelos.
