# camilo_zavala_HERPM13051_s7

## Description

Este repositorio contiene el código para una aplicación Android desarrollada en Kotlin. La aplicación incluye funcionalidades básicas como una pantalla de inicio de sesión y una pantalla de registro.

## Project Structure

- **app**: Contiene el código fuente principal de la aplicación Android.
    - **src/main**: Código fuente de la aplicación.
        - **java/com/example/app**: Paquete principal de la aplicación.
            - **LoginActivity.kt**: Maneja la lógica de la pantalla de inicio de sesión.
            - **RegisterActivity.kt**: Maneja la lógica de la pantalla de registro.
            - **MainActivity.kt**: Pantalla principal después del inicio de sesión.
        - **res/layout**: Archivos de diseño XML.
            - **activity_login.xml**: Diseño de la pantalla de inicio de sesión.
            - **activity_register.xml**: Diseño de la pantalla de registro.
            - **activity_main.xml**: Diseño de la pantalla principal.
    - **res/values**: Archivos de valores XML.
        - **strings.xml**: Cadenas de texto usadas en la aplicación.
        - **colors.xml**: Colores usados en la aplicación.
        - **styles.xml**: Estilos y temas de la aplicación.
- **gradle/wrapper**: Archivos del wrapper de Gradle.
- **.idea**: Archivos de configuración del IDE.

## Functionalities

1. **User Authentication**: Maneja el registro y el inicio de sesión de usuarios.
2. **User Interface**: Incluye pantallas de inicio de sesión y registro con validación de datos.
3. **Main Activity**: Pantalla principal que muestra información básica del usuario autenticado.

## Getting Started

1. **Clone the repository**:
   ```sh
   git clone https://github.com/C1ZC/camilo_zavala_HERPM13051_s7.git
    ```
## Iniciar el proyecto en Android Studio

1. **Abrir el proyecto en Android Studio**:
    - Navega a `Archivo > Abrir` y selecciona el repositorio clonado.

2. **Construir el proyecto**:
    - Haz clic en el menú `Construir` y selecciona `Crear Proyecto`.

3. **Ejecutar la aplicación**:
    - Haz clic en el botón `Ejecutar` o navega a `Ejecutar > Ejecutar 'app'`.

## Dependencias

- **Gradle**: Herramienta de automatización de compilaciones.
- **Kotlin**: Lenguaje de programación para desarrollo Android.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

____________________________________________________________________________________________________


# Desarrollo de la actividad

Eres un desarrollador de aplicaciones móviles para la empresa ABC ESTUDIOS, la cual está interesada en crear una aplicación móvil en Android para ayudar a los estudiantes a gestionar sus días (agenda virtual), por lo cual se han fijado los siguientes requerimientos para dicha aplicación:

1. El nombre del proyecto debe ser su nombre_apellido_seccioncurso.
2. La aplicación debe ser desarrollada en lenguaje Kotlin (aplicativo en lenguaje Java no será considerado).
3. Los días feriados deben ser obtenidos desde la siguiente API:
   `https://apis.digital.gob.cl/fl/feriados/2024`
   (para obtener los días feriados de otro año solo se cambia el último valor de la URL, por ejemplo, para los días feriados del año 2024 sería `https://apis.digital.gob.cl/fl/feriados/2024`). Para invocar a la API debes utilizar hilos y/o AsyncTask.
4. Los datos obtenidos desde la API tienen que ser desplegados en forma de lista (debes deserializar la respuesta de la API para obtener los elementos por separado).
5. La aplicación debe iniciar con una pantalla de bienvenida (SplashScreen).
6. Al ingresar a la aplicación, esta debe contar con un login (usuario y contraseña). La pantalla que despliega los datos de los días feriados debe mostrar el mensaje “Bienvenido: <USUARIO>”, el cual tiene que ser obtenido desde las preferencias de usuario.
7. Luego de cerrada la aplicación, si el usuario ya se encuentra logueado, no debe solicitar credenciales de usuario y clave al abrirla nuevamente.
8. La aplicación debe contar con un botón que permita cerrar la sesión.
