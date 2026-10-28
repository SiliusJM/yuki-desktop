# Yuki Desktop 🌸

**Yuki Desktop** es un asistente personal con inteligencia artificial para Windows 11, con chat, proveedores de IA configurables, integraciones, herramientas y personalización de personajes.

> **Estado: vista previa de desarrollo.** Este repositorio es el punto de distribución de Yuki Desktop, separado del [repositorio de desarrollo](https://github.com/SiliusJM/waifu-assistant). **Todavía no hay una descarga publicada aquí.**

## Estado actual

La versión candidata **0.1.0** ha superado en una cuenta de Windows de pruebas: instalación por usuario, apertura de la aplicación, reinstalación de la misma versión y desinstalación (4/4). Estos resultados **no equivalen a una versión estable ni a una distribución pública aprobada**.

| Área | Estado de la versión candidata |
| --- | --- |
| Instalación y apertura de la interfaz | Probadas en cuenta Windows de pruebas |
| Chat y proveedores de IA | Implementados en el proyecto; verificar funciones disponibles en esta compilación |
| Personalización de personajes e integraciones | Desarrolladas en el proyecto; disponibilidad depende de la compilación y configuración |
| Voz Pocket/Pipecat | **No incluida funcionalmente en el instalador actual** |
| RVC | Experimental; **no disponible en el instalador** |
| Rosa de Yuki en la barra de tareas | **Error conocido**: puede mostrarse el icono de Electron |
| Actualización entre versiones | No probada |
| Conservación de datos tras desinstalación | No probada |
| Firma digital | El instalador candidato no está firmado |

## Descarga

Cuando haya una versión aprobada, estará disponible en [Releases](https://github.com/SiliusJM/yuki-desktop/releases).

**No hay un instalador publicado todavía.** Evita usar instaladores de procedencia desconocida o desactivar las protecciones de Windows.

## Requisitos

- Windows 11 de 64 bits.
- Conexión a Internet para los proveedores de IA en la nube.
- Cuenta y credenciales propias del proveedor elegido, si corresponde.

## Guía de configuración

### 1. Instalar

1. Descarga el instalador desde una publicación oficial de **Releases**, cuando esté disponible.
2. Comprueba el nombre, versión y SHA-256 indicados en las notas de esa versión.
3. Ejecuta el instalador por usuario y sigue las instrucciones.
4. Abre Yuki desde el menú Inicio.

**Importante:** si Windows advierte que el ejecutable no tiene firma digital, verifica primero su origen. No desactives Defender o SmartScreen para continuar.

### 2. Configurar la IA

1. Abre **Configuración** en Yuki.
2. Selecciona un proveedor compatible y el modelo deseado.
3. Introduce las credenciales por los controles de configuración de la aplicación.
4. Comprueba el chat con un mensaje breve.

Nunca compartas claves API, contraseñas ni tokens en Issues o capturas públicas.

### 3. Personalizar el personaje

En Configuración, selecciona el personaje y las opciones de apariencia disponibles. Algunas rutas de avatar o VRM requieren archivos externos proporcionados por el usuario.

### 4. Configurar herramientas e integraciones

Activa únicamente las herramientas que necesites y revisa sus permisos. Los servicios externos pueden requerir autenticación adicional.

### 5. Voz y RVC

La versión candidata de instalación **no incluye los runtimes y componentes necesarios para proporcionar las rutas de voz de desarrollo**. Pocket/Pipecat y RVC no deben considerarse funciones listas para el usuario final en este paquete.

## Desinstalación

Desde **Windows → Configuración → Aplicaciones instaladas**, busca Yuki y elige **Desinstalar**.

La configuración del instalador pretende conservar los datos del usuario, pero **todavía no se ha validado físicamente la conservación tras desinstalar**. Haz una copia de seguridad de los datos importantes antes de cambios de versión.

## Problemas conocidos y limitaciones

- El icono mostrado en la barra de tareas puede ser el de Electron, no la rosa de Yuki.
- No hay soporte de voz empaquetada ni RVC listo para distribución.
- No se ha comprobado una actualización entre dos versiones distintas.
- El instalador candidato no está firmado.
- Siguen pendientes revisiones de seguridad y compatibilidad antes de cualquier lanzamiento estable.

## Código fuente y desarrollo

El desarrollo técnico, el historial de implementación y la documentación interna están en [SiliusJM/waifu-assistant](https://github.com/SiliusJM/waifu-assistant).

Este repositorio se reserva para documentación destinada a usuarios y futuras descargas verificadas. **No se incluyen modelos, credenciales ni runtimes experimentales.**
