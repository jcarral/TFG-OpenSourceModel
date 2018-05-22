# Modelo de datos

En esta sección, se debe explicar cual es el modelo de datos utilizado para el desarrollo de la aplicación.

## 1. EHU

En este nodo se almacenan todos los datos obtenidos de la página web de la universidad.

```
ehu
|- subjects
|- teachers
|- grades
|- search
|- calendars
```


## 2. Users
En el nodo usuarios se almacena toda la información del perfil del usuario. Este nodo se genera automaticamente cuando el estudiante crea su cuenta ya que se ejecuta una de las funciones gracias al servicio `Auth triggers`.

```
users
|- id1
|- id2
|   |- data
|   |- role
|   |- subjects
|   |- teachers
|- ...
```

Un usuario está compuesto por un objeto con sus datos públicos, otros dos con las subscripciones de profesores o asignaturas y por un atributo con el rol.
