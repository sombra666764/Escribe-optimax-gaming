# Guía de Implementación: OptiMax Gaming Edition

Esta guía detalla cómo importar y compilar el proyecto en Android Studio.

## Requisitos Previos:
1.  **Android Studio Hedgehog (2023.1.1)** o superior.
2.  **JDK 17** (incluido con Android Studio).
3.  **Dispositivo de prueba o emulador** con Android 9 (API 28) o superior.

## Pasos para Importar:
1.  Abre Android Studio.
2.  Selecciona **File > New > Import Project...**
3.  Navega hasta la carpeta `OptiMaxGamingEdition` y selecciónala.
4.  Espera a que Gradle sincronice el proyecto.

## Estructura de Módulos:
*   **DNSManager.kt**: Gestiona la configuración de DNS privado para optimizar el ping en juegos.
*   **StorageCleaner.kt**: Implementa la lógica de escaneo y limpieza de archivos temporales.
*   **ProcessManager.kt**: Proporciona accesos directos a la configuración del sistema para gestionar procesos y animaciones.
*   **MainActivity.kt**: Interfaz de usuario construida con Jetpack Compose en Modo Oscuro.

## Notas sobre Permisos:
Para que todas las funciones operen correctamente, el usuario deberá otorgar manualmente los siguientes permisos cuando la app los solicite:
*   **Acceso a todos los archivos (MANAGE_EXTERNAL_STORAGE)**: Necesario para la limpieza profunda en Android 11+.
*   **Modificar ajustes del sistema (WRITE_SETTINGS)**: Necesario para cambiar el DNS privado automáticamente.
*   **Acceso de uso (PACKAGE_USAGE_STATS)**: Necesario para el gestor de procesos avanzado.

---
*OptiMax Gaming Edition - Potencia Pura para tu Android*
