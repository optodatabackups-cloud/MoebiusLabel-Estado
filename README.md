# MoebiusLabel-Estado

Repositorio de datos, no de código. Lo usa el sistema de licencias de **Moebius LabelPrint**:

- `estado.json` — lista de licencias emitidas (cliente, PC, vencimiento, si está revocada). Lo edita
  el panel de "Ópticas" de `GeneradorLicenciasOptodata` y lo lee el programa cliente al abrir, para
  saber si su licencia sigue siendo válida.
- **Issues** de este repo — cada apertura del programa cliente crea/actualiza un issue con el título
  igual al código de la PC, y el cuerpo con la versión instalada y la fecha. Es solo un buzón de
  "aviso de versión"; el panel de Ópticas los lee para mostrar qué versión tiene cada óptica.

Es público a propósito: el programa cliente necesita leer `estado.json` sin credenciales para poder
funcionar sin depender de una cuenta. No tiene código fuente ni instaladores — eso vive en
[MoebiusLabel-Releases](https://github.com/optodatabackups-cloud/MoebiusLabel-Releases).
