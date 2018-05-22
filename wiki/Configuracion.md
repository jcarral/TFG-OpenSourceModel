# Configuración

En este apartado se debe documentar el proceso para configurar el proyecto, si requiere de alguna configuración adicional a la de la instalación.

## Variables de entorno

```
// .dotenv
DB_HOST=localhost
DB_USER=root
DB_PASS=s1mpl3
```

## Configuración firebase

Para añadir las credenciales de firebase hay que hacerlo en el fichero `app/config/credentials.js`, sustituir el objeto credentials por el que te da firebase.

```javascript
const credentials = {

};
```
