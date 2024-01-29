# Ecommerce app

## Vision general del proyecto

Este proyecto es un ecommerce desarrollado para dispositivos mobiles esta desarrollado en stack asociado a JavaScript. Las tecnologías requeridas para esta ocasión incluyen:

1. **JavaScript:** Lenguaje de programacion.
2. **NodeJS:** Motor de ejecución para JavaScript en el servidor.
3. **Express:** Framework para crear aplicaciones web con NodeJS.
4. **React:**  Para construir la interfaz de usuario (frontend) de la app.
5. **Firebase:** Base de datos NoSQL escalable.
6. **Socket.IO:** Permite realizar comunicaciones entre cliente y servidor en tiempo real.
7. **Expo:** Para simplificar su código React Native

## Inicio rápido

Para ejecutar este proyecto, necesitas tener instalado lo siguiente:

1. [Node.js v16.x.x o superior](https://nodejs.org/en/download/) (se recomienda la versión LTS).
2. Un editor de código de tu elección (por ejemplo, Visual Studio Code aka VSCode).

Además, para el hosting de imágenes, necesitarás una cuenta de Cloudinary para obtener las credenciales.

## Instalaciones necesarias

### Instalación de Node

-   Sigue las instrucciones del asistente, presionando "Siguiente" en cada pantalla.
    -   Directorio de instalación: Por defecto, es en el disco (C:) de Windows y su equivalente /root/ para Linux. Asegúrate de tener suficiente espacio para la instalación.
    -   Agregar Node al PATH (Win OS): Importante para ejecutar procesos de Node.

![Instalación de Node](https://i.stack.imgur.com/SsGIl.png)

## Instrucciones de uso

### Base de datos
# Configuración de la Base de Datos Firebase

Este documento proporciona instrucciones detalladas sobre cómo configurar la base de datos de tu proyecto utilizando Firebase.

## Paso 1: Crear un Proyecto en Firebase

1. Accede a [Firebase Console](https://console.firebase.google.com/).
2. Haz clic en el botón "Agregar proyecto".
3. Sigue las instrucciones para configurar tu nuevo proyecto.

## Paso 2: Configurar la Base de Datos

1. En el panel de tu proyecto en Firebase Console, selecciona "Database" en el menú lateral.
2. Haz clic en "Crear base de datos".
3. Elige entre "Firestore" (base de datos NoSQL) o "Realtime Database" (base de datos en tiempo real). Selecciona el que mejor se adapte a tus necesidades.

## Paso 3: Establecer Reglas de Seguridad

1. En la pestaña "Reglas" de la sección Database, establece las reglas de seguridad para tu base de datos. Asegúrate de entender y configurar las reglas según las necesidades de tu aplicación.


## Paso 4: Configurar las Credenciales

1. En la configuración de tu proyecto, haz clic en el icono de engranaje y selecciona "Configuración del proyecto".
2. En la pestaña "Cuentas del servicio", agrega una nueva clave JSON para tu aplicación. Guarda el archivo JSON generado de manera segura.

## Paso 5: Integrar Firebase en tu Aplicación

1. Instala la biblioteca Firebase en tu proyecto. Para JavaScript, puedes usar:
                npm install firebase

2. Incializamos Firebase con las credenciales proporcionadas:
 - apiKey:"",
 - authDomain:"",
 - proyectId: "",
 - storageBucket:"",
 - messagingSenderId,
 - appId: ""

### Descarga y configuración del proyecto

-   Abre una consola CMD o equivalente en el directorio deseado y ejecuta el comando `git clone` para tener una copia local del proyecto:
    ```bash
    git clone https://github.com/MaximoPavesi/my-ecommerce-app
    ```
-   En la misma consola, ejecuta `cd my-ecommerce-app` para acceder a la carpeta que contiene el proyecto, recientemente creada.
-   Para instalar las dependencias necesarias y especificadas en el archivo `package.json`, ejecuta el comando `npm install` o su equivalente `npm i`.

### Archivo `.env`

-   Este archivo no se encuentra en la copia creada recientemente porque está entre las excepciones a subir a Github, especificado en el archivo `.gitignore`. Este archivo contiene información sensible respecto a Variables de Entorno. Estas variables se configuran de acuerdo con la información del usuario, conexiones a APIs externas mediante credenciales u otros. Para este proyecto, es necesario crear un archivo `.env` en la raíz del proyecto y debe contener las siguientes claves:
    ```dotenv
    PORT=4000
    base_url=/* La URL base de datos de Firebase */
    api_key=/* Key api de Firebase*/
    base_auth_url/* La URL de auth de Firebase*/
    maps_api_key = /* La key de google Cloud*/
    ```

## Ejecución del Proyecto

Con las instalaciones necesarias realizadas y con el archivo `.env` configurado, abrir dos consolas y ejecutar un comando de los que se detalla a continuación en cada una:
-   Ejecutar el comando `npm expo start` para ejecutar el proyecto en modo desarrollo.


¡Disfruta! ✨