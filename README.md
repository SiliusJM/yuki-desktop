# Yuki Desktop 🌸

Asistente personal de escritorio con IA para **Windows 11 (x64)**. Yuki está diseñado para combinar chat, proveedores de IA configurables, personalidad, herramientas, integraciones y una experiencia visual con personajes.

> **Distribución preliminar.** La descarga pública disponible es **v0.1.0-pre.1**. No es una versión estable ni incluye todas las capacidades desarrolladas.

## Descargar

Ve a **[Releases](https://github.com/SiliusJM/yuki-desktop/releases)** y descarga el instalador de la versión que desees probar. La publicación actual contiene `Yuki.Setup.0.1.0.exe`.

**Seguridad:** verifica que el archivo proviene de esta página oficial. El instalador preliminar no está firmado digitalmente; Windows puede mostrar advertencias. No desactives Windows Defender ni SmartScreen para instalarlo.

## Instalar paso a paso

1. Usa Windows 11 x64.
2. Descarga el instalador de la sección **Releases**.
3. Comprueba el nombre y la versión de la publicación; verifica el SHA-256 cuando esté publicado.
4. Ejecútalo con la instalación por usuario, sin modificar los permisos de seguridad del sistema.
5. Abre Yuki desde el menú Inicio.
6. Si aparece un error, conserva el mensaje para reportarlo sin incluir credenciales ni datos personales.

## Configuración inicial

1. **IA y chat:** abre Configuración, selecciona un proveedor/modelo disponible e introduce sus credenciales únicamente en los campos previstos. Los proveedores externos pueden requerir conexión y una cuenta propia.
2. **Personaje:** elige las opciones de apariencia y personalidad disponibles en esa versión. Los modelos y archivos personales no se distribuyen automáticamente.
3. **Herramientas e integraciones:** habilita solamente las que necesites y revisa sus permisos. Algunos servicios requieren autorización adicional.
4. **Voz y RVC:** **no están listos para uso completo en la descarga pública v0.1.0-pre.1**. No descargues archivos `.pth` o `.index` de procedencia dudosa ni uses voces sin autorización.

## Qué está disponible y qué sigue en prueba

| Función | Estado de la descarga pública v0.1.0-pre.1 |
| --- | --- |
| Instalación por usuario y apertura de la aplicación | Aceptación básica Windows completada |
| Chat, proveedores, herramientas y configuración | Algunas capacidades dependen de la versión, proveedor y configuración |
| Avatar/VRM y lip-sync | Disponibilidad y aceptación de usuario final pendientes |
| Pocket/Pipecat y RVC | **No incluidos como funciones listas para esta versión** |
| Actualización entre versiones | No aceptada para esta versión pública |
| Icono original de Yuki | Limitación conocida en la versión preliminar |
| Firma del instalador | Sin firma digital |

Existe un candidato más reciente sometido a pruebas de Windows, pero **no se ha publicado aquí como versión estable**. No confundas las pruebas internas de versiones posteriores con las funciones de esta descarga.

## Desinstalación

Abre **Configuración de Windows → Aplicaciones → Aplicaciones instaladas → Yuki → Desinstalar**. Antes de reinstalar o cambiar de versión, guarda una copia de seguridad de los datos que consideres importantes.

## Privacidad y seguridad

- No publiques API keys, contraseñas, tokens, sesiones, archivos de configuración privados ni modelos personales.
- Yuki puede requerir acceso a servicios externos según las integraciones que actives.
- Los modelos de voz y avatares de terceros pueden tener licencias y restricciones propias.
- Este repositorio es exclusivamente el espacio público de documentación y distribución. **No contiene datos personales, archivos de desarrollo privados ni rutas locales del autor.**

## Problemas y comentarios

Usa **[Issues](https://github.com/SiliusJM/yuki-desktop/issues)** e indica versión de Yuki, versión de Windows y el comportamiento observado. Elimina datos personales de capturas y registros.

## Estado del proyecto

La siguiente versión se publicará cuando complete las verificaciones de seguridad, configuración, audio/voz, RVC, avatar y distribución correspondientes. Las funciones no aceptadas no se anuncian como estables.
