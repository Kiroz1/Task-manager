# Task Manager (Spring Boot)

Aplicación web sencilla para la **gestión de tareas** desarrollada con Java y Spring Boot.
El proyecto implementa operaciones básicas para administrar tareas y sirve como **base para un sistema de administración de tareas más completo**.

## Descripción

Este proyecto permite registrar y organizar tareas mediante una interfaz web simple.
Las tareas pueden crearse, visualizarse, actualizar su estado y eliminarse.

El objetivo del proyecto es demostrar el uso de una arquitectura básica con Spring Boot utilizando el patrón:

Controller → Service → Repository

## Tecnologías utilizadas

* Java
* Spring Boot
* Spring MVC
* Spring Data JPA
* Thymeleaf
* H2 Database
* HTML y CSS

## Funcionalidades

* Crear tareas
* Visualizar tareas
* Cambiar el estado de una tarea
* Eliminar tareas
* Filtrar tareas por estado

## Estados de las tareas

Cada tarea puede encontrarse en uno de los siguientes estados:

* PENDIENTE
* EN_PROGRESO
* TERMINADO

## Estructura del proyecto

```
src
 └─ main
     ├─ java
     │   └─ controller
     │   └─ service
     │   └─ repository
     │   └─ model
     │
     └─ resources
         ├─ templates
         └─ static
```

### Capas

**Controller**

Gestiona las peticiones HTTP y la comunicación con las vistas.

**Service**

Contiene la lógica de negocio de la aplicación.

**Repository**

Gestiona el acceso a datos utilizando Spring Data JPA.

**Model**

Define las entidades del sistema.

## Entidad principal

Task

Campos principales:

* id
* titulo
* descripcion
* estado
* fechaLimite

## Base de datos

El proyecto utiliza **H2 Database**, una base de datos en memoria utilizada comúnmente para desarrollo y pruebas.

## Ejecución del proyecto

1. Clonar el repositorio

```
git clone https://github.com/usuario/task-manager.git
```

2. Entrar al proyecto

```
cd task-manager
```

3. Ejecutar la aplicación

```
mvn spring-boot:run
```

4. Abrir en el navegador

```
http://localhost:8080/tasks
```

## Objetivo del proyecto

Este proyecto sirve como **base para el desarrollo de sistemas de administración de tareas**, implementando una estructura simple con Spring Boot y demostrando la integración entre backend, base de datos y vistas web.
