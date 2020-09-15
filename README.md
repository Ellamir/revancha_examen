# revancha_examen
Intento de realizar el examen de TD con Vuetify y VueX :D

## Caso “Classicmodels Orders”

### Contexto del Problema
“Classicmodels” es una empresa dedicada a la fabricación y comercialización de modelos a escala de distintos tipos de vehículos motorizados tales como automóviles, motocicletas, trenes y aviones, entre otros. Sus modelos son de alto realismo y de gran calidad, razón por la cual ha logrado posicionarse en el mercado de los coleccionistas a nivel mundial.
La empresa se creó en los años sesentas como una empresa familiar, y debido a la buena calidad de sus modelos, fue rápidamente creciendo. Actualmente, cuenta con oficinas en las principales capitales del mundo, tales como New York, Boston, San Francisco, Paris, Tokyo, Sydeny, y London.
El crecimiento de la empresa no ha estado exento de dificultades, de hecho, el principal reclamo es el atraso en los pedidos debido a que no se lleva un buen control de las existencias y las órdenes. Al respecto, el CEO de la organización ha solicitado al CTO que impulse un proyecto de mejora de los sistemas ya datan de los años 90s y no se le han hecho grandes mejoras.
El CTO está muy entusiasmado con el proyecto y rápidamente ha formado un equipo de proyectos de primera línea del cual usted forma parte como desarrollador front-end. El equipo de proyectos también lo conforma un Jefe de Proyectos, un Diseñador UX/UI, un Diseñador Web, un Analista Funcional, Desarrolladores Backend y Mobile, y un Arquitecto de Software.

### Objetivo del Proyecto, Alcance y Avance a la fecha
El proyecto busca, dentro de otras cosas, ordenar el sistema de administración de órdenes que cursan los vendedores de las distintas oficinas alrededor del mundo. A continuación, se listan los requisitos del sistema:
Requisitos Funcionales del Sistema:
- [ ] El sistema debe controlar el acceso de los usuarios a la plataforma
- [ ] El sistema debe contar con un dashboard que permita tener una visión general de los procesos relacionados con el cumplimiento de las ordenes
- [ ] El sistema debe permitir la consulta de las órdenes que se encuentran en los distintos estados en las distintas oficinas
- [ ] El sistema debe permitir ver la información de detalle de cada orden, así como su estado de completitud de cada producto

### Definiciones y lineamientos arquitectónicos:
El arquitecto, para satisfacer las necesidades del proyecto, ha definido la utilización de una arquitectura basado en componentes Front-End y Back-end. Para esto, ha definido los siguientes lineamientos:
- [ ] El sistema debe ser implementado utilizando la tecnología de Single Page Application con el framework Vue, Vue-Router y Vuex
- [ ] El sistema debe ser implementado utilizando tecnología REST para el consumo de información de APIs
- [ ] El sistema debe adaptarse a dispositivos de tipo desktop y teléfono
- [ ] Utilizar framework bootstrap o similar para el manejo de estilos
- [ ] Se debe utilizar un preprocesador SASS para el manejo de estilos y alguna metodología para el nombramiento de clases.
- [ ] Se requiere implementar la lógica que permita mostrar una página de error 404 (no encontrada) cuando se acceda a una ruta o recurso inexistente.

### Requerimientos a implementar
El jefe de proyectos, quien lleva un control meticuloso de las actividades del proyecto, le ha solicitado a Usted que realice las siguientes tareas:
- [ ] Implementar página de Login de Usuario.
- [ ] Implementar página Home con Dashboard.
- [ ] Implementar página con Monitor de Ordenes.
- [ ] Implementar página con Detalle de Orden

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
ntar página con Detalle de Orden