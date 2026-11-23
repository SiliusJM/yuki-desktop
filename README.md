# Yuki Desktop 🌸

Asistente personal de escritorio con IA para **Windows 11 (x64)**. Yuki está diseñado para combinar conversación, proveedores configurables, personalidad, herramientas e integraciones.

## Descargar la versión actual

**Versión pública más reciente: [v0.2.0-stable.4 — Windows 11](https://github.com/SiliusJM/yuki-desktop/releases/tag/v0.2.0-stable.4).**

La instalación del EXE y el primer arranque se aceptaron en una cuenta de pruebas aislada de Windows (YukiTest). **Esto no constituye aceptación funcional completa** de voz, micrófono, RVC, avatar ni actualizaciones automáticas.

### Archivos necesarios

Descarga desde los **Assets** de ese Release:

- [Instalador Windows — `Yuki.Setup.0.2.0-stable.4.exe`](https://github.com/SiliusJM/yuki-desktop/releases/download/v0.2.0-stable.4/Yuki.Setup.0.2.0-stable.4.exe)
- `Yuki.Offline.Voice.0.2.0-stable.4.zip.part001`, `.part002` y `.part003` (las tres partes)
- [`Reconstruct-Offline-Voice.ps1`](https://github.com/SiliusJM/yuki-desktop/releases/download/v0.2.0-stable.4/Reconstruct-Offline-Voice.ps1)
- [`INSTALLATION-ES.md`](https://github.com/SiliusJM/yuki-desktop/releases/download/v0.2.0-stable.4/INSTALLATION-ES.md) (instrucciones detalladas)
- [`SHA256SUMS.txt`](https://github.com/SiliusJM/yuki-desktop/releases/download/v0.2.0-stable.4/SHA256SUMS.txt) (sumas de integridad)
- [`LICENSES-VOICE-ES.txt`](https://github.com/SiliusJM/yuki-desktop/releases/download/v0.2.0-stable.4/LICENSES-VOICE-ES.txt) (licencias y atribuciones)

**Importante:** el instalador exige el ZIP offline **completo**, no las partes por separado. Sigue `INSTALLATION-ES.md` para reconstruirlo con el helper, verificar su SHA-256 y dejarlo junto al EXE con su nombre original. **No ejecutes el instalador hasta completar esos pasos.** El helper acepta los nombres de descarga de GitHub, que sustituyen espacios por puntos.

SHA-256 del EXE: `A8EA0A6D79BEFBED18B45805C0180B44C385B6DA65D8A8B56EBC65CFE01186A8`

SHA-256 del ZIP reconstruido: `EE8F436E6507C20A6EAACC4D35EE56AA6DB5595599900696A329355D59BF9A41`

No descargues paquetes o modelos desde fuentes no verificadas. El instalador **no está firmado digitalmente**; Windows puede mostrar advertencias de SmartScreen. No desactives Defender ni SmartScreen para instalarlo.

## Configuración inicial

1. Abre Yuki y selecciona un proveedor/modelo en **IA y modelos**. Los servicios externos pueden requerir una cuenta y credenciales propias.
2. Configura las integraciones y sus permisos según necesites.
3. Consulta **Más ajustes → Soporte y diagnósticos** para ver el estado local. Un estado local saludable no prueba por sí solo que un proveedor remoto funcione.
4. Mantén las credenciales y modelos personales fuera de reportes públicos.

## Alcance comprobado y limitaciones

| Área | Estado para v0.2.0-stable.4 |
| --- | --- |
| Instalación Windows por usuario | **PASS** en cuenta de pruebas aislada |
| Arranque, pantalla inicial y diagnósticos | **PASS** de apertura/navegación básica |
| Chat con proveedores externos | Requiere configuración; no cubierto por esta aceptación |
| Voz offline, Pocket TTS, Moonshine, Smart Turn, VAD y RVC | Runtime/modelos incluidos según notas; **funcionamiento integral no aceptado** |
| Actualización incremental automática | **No verificada** |
| Casilla «Abrir notas de versión» del instalador | Se reportó que no abrió la página esperada; pendiente de diagnóstico |
| Firma digital | Instalador sin firma |

No se incluyen modelos privados de voz RVC (`.pth`/`.index`), ni se autoriza redistribuir voces de terceros sin sus derechos correspondientes. Consulta los avisos adjuntos.

## Otras versiones e incidencias

El [Release preliminar v0.1.0-pre.1](https://github.com/SiliusJM/yuki-desktop/releases/tag/v0.1.0-pre.1) continúa disponible como archivo histórico; no representa la versión recomendada actual.

Reporta defectos en [GitHub Issues](https://github.com/SiliusJM/yuki-desktop/issues), indicando la versión, Windows y pasos de reproducción, **sin claves API, tokens, capturas sensibles, registros personales o credenciales**.

El [PR #1](https://github.com/SiliusJM/yuki-desktop/pull/1) conserva un **archivo histórico H19 de incidencias YF-01 a YF-41**. Sus estados corresponden a un candidato anterior y **no describen necesariamente la versión publicada**. No se consideran 41 problemas actuales verificados automáticamente.

## Desinstalación

Usa **Configuración de Windows → Aplicaciones → Aplicaciones instaladas → Yuki → Desinstalar**. Antes de actualizar o desinstalar, respalda los datos importantes.

## Sobre este repositorio

Este repositorio público contiene documentación y archivos de distribución. No debe alojar credenciales, datos personales, modelos privados ni artefactos internos del desarrollo.
