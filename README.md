Sistema de Monitoreo de Estanque de Agua y Control de Bomba
Descripción del Proyecto
Este proyecto consiste en una aplicación móvil nativa desarrollada en Kotlin para Android, diseñada para la supervisión en tiempo real del nivel de agua en estanques y la gestión automatizada de sistemas de bombeo. Su objetivo principal es prevenir la falla por trabajo en seco (dry running) mediante el corte automático del flujo eléctrico hacia la bomba cuando los niveles de agua se encuentran bajo el umbral de seguridad.

Arquitectura y Componentes Técnicos
1. Seguridad y Autenticación
EncryptedSharedPreferences: Implementado para garantizar el almacenamiento seguro de credenciales de usuario y tokens de sesión a nivel local.

ISO 27400: El diseño de la aplicación contempla pautas de seguridad para dispositivos IoT, protegiendo la confidencialidad de los datos de acceso.

2. Comunicación Inalámbrica y Manejo de Concurrencia
Protocolo de Comunicación: Soporte para comunicación inalámbrica local mediante Bluetooth (RFCOMM) o conexión en red local Wi-Fi.

Corrutinas de Kotlin: Gestión asíncrona de las conexiones en segundo plano para evitar el bloqueo del hilo principal de la interfaz de usuario (UI).

3. Interfaz de Usuario (UI)
Material Design: Cumplimiento con las guías de diseño moderno de Android para ofrecer una interfaz limpia, legible y responsiva.

Monitoreo en Tiempo Real: Panel de control con desplazamiento vertical que muestra el porcentaje o nivel del estanque, estado de la bomba (activa/inactiva) y controles de anulación manual.

Requisitos del Sistema y Entorno
Lenguaje de Programación: Kotlin

Entorno de Desarrollo (IDE): Android Studio (versión recomendada: Ladybug o superior)

Instrucciones de Compilación y Despliegue
1. Clonar el Repositorio
Bash
git clone https://github.com/enxoyt10-coder/MonitoreoEstanqueIoT.git
2. Abrir en Android Studio
Inicie Android Studio.

Seleccione la opción Open y busque la carpeta donde clonó el proyecto.

Guarde unos minutos mientras Gradle sincroniza las dependencias e índices del proyecto.

3. Ejecución en Dispositivo
Active las Opciones de Desarrollador y la Depuración por USB en su dispositivo Android.

Conecte el dispositivo mediante cable USB a la computadora.

En la barra superior de Android Studio, seleccione su dispositivo en el desplegable.

Presione el botón Run 'app' (o use la combinación de teclas Shift + F10).

Licencia y Contexto Académico
Proyecto desarrollado para la asignatura TI3042 en el área de Tecnologías de la Información y Comunicación - INACAP.

¿Cómo agregarlo a tu proyecto?
En Android Studio, busca el archivo README.md en el panel de la izquierda (si no existe, haz clic derecho en la raíz del proyecto > New > File y nómbralo README.md).

Pega este texto, guarda los cambios y ejecuta en la Terminal:

Bash
git add README.md
git commit -m "Documentación inicial del proyecto"
git push origin master
SDK Mínimo: Android 7.0 (API Nivel 24)

SDK Objetivo: Android 14 (API Nivel 34)
