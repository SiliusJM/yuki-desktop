# Yuki Desktop — Archivo público de estado (3 de noviembre de 2026)

**Estado del desarrollo: PAUSADO / ARCHIVADO. No es una versión final ni estable.**

Este documento informa del resultado real de las pruebas físicas del candidato H19 y conserva las tareas pendientes. El código de desarrollo se conserva en un repositorio **privado**, separado de este repositorio público. La documentación pública no incluye dicho historial, credenciales, modelos privados ni archivos personales.

## Resultado del último candidato instalado (Windows 11)

| Función | Estado |
| --- | --- |
| Chat escrito: enviar y recibir respuestas | **PASS** |
| Micrófono: convertir una intervención en mensaje del chat | **FAIL** — queda en «Detener micrófono», sin enviar el turno |
| Inicio de respuestas habladas | **FAIL** — demora excesiva |
| Audio TTS: silbido agudo | **KNOWN FAIL** |
| Cambio físico de dispositivos de audio | **NO VALIDADO COMPLETAMENTE** |
| Animación OBS, vista previa RVC y respuesta física del avatar | **NO VALIDADAS COMPLETAMENTE** |

Una suite de código registró **1.937 PASS, 0 FAIL y 3 SKIP**; esto **no equivale** a aceptación física. Los problemas anteriores siguen abiertos.

## Distribución H19: BLOQUEADA

No hay un instalador H19 autónomo para descargar desde aquí. El EXE depende de un archivo ZIP de voz offline de **4.636.926.717 bytes**, cuya presencia y suma SHA-256 verifica el instalador antes de continuar. Un asset individual de GitHub Releases no admite ese tamaño. Tampoco están completamente verificadas las condiciones de redistribución de todos los runtimes y modelos de terceros. El ejecutable está sin firmar.

**No se deben descargar archivos EXE o ZIP de fuentes no verificadas ni presentar H19 como versión estable.** La publicación binaria requiere resolver hospedaje, derechos de redistribución, integridad de artefactos e instrucciones de instalación.

## Archivo de pendientes

Consulta el [registro YF-01 a YF-41](YUKI_H19_KNOWN_ISSUES.md). YF-28 sigue **BLOCKED / UNVERIFIED / NOT IMPLEMENTED** y YF-39 **FUTURE / DEFERRED**. Las anotaciones de verificaciones técnicas históricas no sustituyen los resultados de uso real.

## Reanudación posterior

El desarrollo permanecerá pausado hasta una decisión futura. Para retomarlo, se utilizará el archivo fuente privado verificado y los recursos personales que el propietario haya respaldado por separado. No se requiere ninguna nueva prueba de voz para cerrar este archivo público.

**Esta publicación contiene documentación, no una nueva versión binaria ni cambios de aplicación.**
