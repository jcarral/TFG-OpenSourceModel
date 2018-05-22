# API

En este documento, se deben documentar todas las funcionalidades de la herramienta si fuera necesario.

Si es demasiado extenso, se deben enlazar los documentos con los apartados con los detalles.

## Instalación

Se puede utilizar un gestor de paquetes como [npm](https://www.npmjs.com/) o [yarn](https://yarnpkg.com/en/), la versión zip también está disponible.

```
npm i --save ehu-scraping
```
```
yarn add ehu-scraping
```

## Uso

Una vez instalada la librería hay que importarla en el proyecto.
```javascript
import {University, Grade } from 'ehu-scraping';
const { University } = require('ehu-scraping');
```

Luego, basta con utilizar las funciones de los objetos que se han importado. Para más información visitar la documentación extendida.

```javascript
// Lista de grados del campus de Bizkaia
const listaDeGrados = University.getGradesList({campus: 'BI'});

//Asignaturas de la carrera de informatica de la FISS
const gradoInformatica = new Grade('GINFOR20');
const asignaturasInfor = gradoInformatica.getSubjects();
```

## Lista de funciones

La lista de funciones disponibles es la siguiente, para más información acceder a la información detallada.

- [University](ScrapingUniversity#university)
	- [static getGradesList([data])](ScrapingUniversity#static-getdegreeslistdata--promise)
	- [static getCampus()](ScrapingUniversity#static-getcampus--object)
	- [static getGradesUrl()](ScrapingUniversity#static-getdegreesurl--string)
- [Grade](ScrapingGrade.md#degree)
	- [getSummary()](ScrapingGrade#getsummary--promise)
	- [getSubjects([course])](ScrapingGrade#getsubjectscourse--promise)
	- [getTeachers()](ScrapingGrade#getteachers--promise)
	- [getURL()](ScrapingGrade#static-geturl--string)
	- [static getName(code)](ScrapingGrade#static-getnamecode--string)
	- [static getCode(codeName)](ScrapingGrade#static-getcodename--string)
	- [code](ScrapingGrade#code--string)
	- [school](ScrapingGrade#school--string)
- [Subject](ScrapingSubject#subject)
	- [getSummary()](ScrapingSubject#getsummary--promise)
	- [getDetail()](ScrapingSubject#getdetail--promise)
	- [getSchedule()](ScrapingSubject#getschedule--promise)
	- [subject](ScrapingSubject#subject--string)
	- [school](ScrapingSubject#school--string)
	- [degree](ScrapingSubject#degree--string)
	- [course](ScrapingSubject#course--string)
- [Teacher](ScrapingTeacher#teacher)
	- [getTutorships()](ScrapingTeacher#gettutorships--promise)
	- [id](ScrapingTeacher#id--string)
	- [degree](ScrapingTeacher#degree--string)
