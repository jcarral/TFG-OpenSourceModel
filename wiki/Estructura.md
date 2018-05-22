# Estructura

En este documento se debe detallar cual es la estructura de la aplicación, los directorios que contiene y cual es el fin de cada uno.

```
app
|- admin
|   |- screens
|- assests
|- auth
|   |- screens
|- calendar
|   |- screens
|- components
|- config
|- grade
|   |- screens
|- lib
|- locale
|   |- languages
|- search
|   |- screens
|- settings
|   |- screens
|- subject
|   |- screens
|- teacher
|   |- screens
|- user
|   |- screens
```

* **admin:** Este módulo es el controla el comportamiento de las vistas del administrador. La página principal, el calendario y la lista de fechas.

* **assets:** Directorio donde se almacena el contenido como imágenes o estilos.

* **auth:** Módulo que gestiona todo lo relacionado con la autenticación del usuario. Desde las ventanas de registro e inicio de sesión hasta el _SplashScreen_.

* **calendar:** Apartado donde se gestiona todo lo relacionado con los calendarios, desde cargar las fechas hasta visualizarlos para el usuario.

* **components:** Sección donde se almacenan todos los componentes reutilizables.

* **config:** Directorio donde se guardan los ficheros responsables de la configuración de la aplicación.
