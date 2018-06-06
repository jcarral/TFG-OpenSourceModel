# Contributing

A continuación, se describe la forma de contribuir al proyecto.

## Tabla de contenidos

1. [Prerrequisitos](#prerequisitos)
2. [¿Cómo empezar?](#cómo-empezar)
3. [Propuesta de mejora](#propuesta-de-mejora)
4. [Traducción](#traducción)
5. [Añadir un ejemplo](#añadir-un-ejemplo)
6. [Versionado](#versionado)
7. [Etiquetas](#etiquetas)
8. [Contacto](#contacto)

## Prerrequisitos

* Cualquier propuesta de mejora, notificación de error o sugerencia de cambio se debe realizar a través de los canales de comunicación establecidos.
Para este proyecto se utilizan los _issues_ de GitHub.
* Se debe seguir el [código de conducta](codeofconduct), cualquier petición que incumpla este código se rechazará inmediatamente.
* El idioma principal de la documentación es el castellano. Por defecto, todos los documentos que no tengan el código del idioma al final del nombre, estarán en castellano.

## ¿Cómo empezar?

1. Crea un _fork_ del repositorio original.
2. Crea un _branch_ con un nombre descriptivo.
4. Realizar los cambios.
5. Haz _commit_ de los cambios.
    - Para los commits utiliza uno de los siguientes prefijos en el mensaje.
    ```
    [DOCS]
    [BUG]
	[EXAMPLE]
    ```
6. Realiza un _pull request_
    - En este punto debes asegurarte de que la rama master está actualizada con el repositorio original.
    - Haz _PR_ desde tu rama a la rama master del proyecto original.
7. Manten actualizada tu _PR_
8. Fusionar el _PR_ (Solo responsables)
9. Actualizar la versión. (Solo responsables)
10. Lanzar una versión. (Solo responsables)

## Propuesta de mejora

1. Comprobar que no es una propuesta de mejora ya realizada.
2. Abrir un nuevo _issue_ utilizando la plantilla para mejoras que se proporciona.
3. Responder a las siguientes preguntas:
    - ¿ Qué debe hacer la mejora ?
    - ¿ Por que debería implementarse ?
    - ¿ Cómo debería hacerse ?
4. Añade cualquier tipo de material que ayude a entender la propuesta. (Imagenes o enlaces a recursos).

## Añadir un ejemplo

Si después de realizar tu trabajo de fin de grado siguiendo un desarrollo _open source_ quieres añadir tu proyecto como ejemplo para que futuros estudiantes puedan consultarlo, debes realizar los siguientes cambios:

1. Crea una carpeta en `examples` con el nombre `tfg-{NOMBRE_USUARIO-GITHUB}`.
2. En la carpeta que has creado crea un fichero README.md siguiendo la [plantilla para los ejemplos](./templates/EXAMPLES-ES.md).
3. Añade en ese directorio todo el material adicional que creas útil. Memoria, imagenes, ...
4. En el fichero [README.md](./examples/README.md) del directorio `examples` añade a la lista de proyectos el tuyo siguiendo la estructura propuesta.
5. Abre un pull request con los cambios realizados.

## Versionado

En este proyecto se sigue el módelo de versiones [semver](https://semver.org/).

## Etiquetas

Cuando se abre una nueva _issue_ se le añaden una serie de etiquetas en función del contenido. En la siguiente tabla se pueden ver todas junto a su descripción.

| Nombre | Descripción |
| ------ | ------------|
| 🐛 bug | Notificación de error |
| ❌ duplicate | Issue repetida |
| 🙋🏼‍♀️ feature | Nueva funcionalidad |
| 👶🏼 good first issue | Ejemplo de una buena _issue_ |
| 🙏🏼 help wanted | Petición de ayuda |
| ⚠️ invalid | _Issue_ incorrecta |
| 🧐 question | Pregunta sobre el proyecto |


## Contacto

* [Joseba Carral](https://github.com/jcarral) - jcarraldc@gmail.com
