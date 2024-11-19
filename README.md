# 202DWESProyectoTema4

## Tema 4: Técnicas de Acceso a Datos en PHP

Este proyecto es una implementación práctica de las técnicas de acceso a datos en PHP, correspondiente al Tema 4 del módulo **Desarrollo Web en Entorno Servidor (DWES)**. Está diseñado para explorar conceptos como la conexión a bases de datos, consultas, manejo de excepciones, y mejores prácticas en el uso de PDO.

---

## **Índice**
1. [Descripción](#descripción)
2. [Requisitos](#requisitos)
3. [Instalación](#instalación)
4. [Estructura del Proyecto](#estructura-del-proyecto)
5. [Funcionalidades Principales](#funcionalidades-principales)
6. [Autor](#autor)

---

## **Descripción**

El proyecto implementa las siguientes funcionalidades:
- Conexión a bases de datos utilizando **PDO** (PHP Data Objects).
- Realización de operaciones CRUD (Crear, Leer, Actualizar, Eliminar) con bases de datos.
- Manejo de errores y excepciones para garantizar robustez.
- Aplicación de consultas parametrizadas para evitar inyecciones SQL.
- Uso de configuraciones externas para credenciales de conexión.

---

## **Requisitos**

Antes de ejecutar el proyecto, asegúrate de contar con los siguientes requisitos:

- **Servidor web** con soporte para PHP (por ejemplo, Apache con XAMPP o WAMP).
- **PHP 7.4 o superior**.
- **Base de datos MySQL/MariaDB**.
- Navegador web actualizado para probar la interfaz (si corresponde).
- Herramienta para ejecutar consultas SQL, como phpMyAdmin o MySQL Workbench.

---

## **Instalación**

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/usuario/202DWESProyectoTema4.git
   cd 202DWESProyectoTema4

   Subir estos archivos al servidor web

2. **Configurar la base de datos:**

Importa el archivo ___.sql incluido en el proyecto para crear las tablas necesarias.
Configura las credenciales de acceso en el archivo config/config.php:
```php
define('DB_HOST', 'localhost');
define('DB_NAME', 'nombre_base_datos');
define('DB_USER', 'usuario');
define('DB_PASS', 'contraseña');
```

3. **
Si utilizas servidor web en la nube, coloca el proyecto en la carpeta htdocs y accede mediante https://202DWESProyectoTema4.victorgargon.informatica.ieslossauces.es/

---

## **Estructura de directorios**
´´´bash
202DWESProyectoTema4/
├── config/
│   ├── config.php          # Configuración de base de datos
├── database/
│   ├── database.sql        # Script para crear y poblar la base de datos
├── public/
│   ├── index.php           # Página principal del proyecto
├── src/
│   ├── Connection.php      # Clase para la conexión a la base de datos
│   ├── CrudOperations.php  # Funciones CRUD encapsuladas
├── tests/
│   ├── test_connection.php # Prueba de conexión a la base de datos
├── README.md               # Documentación del proyecto

´´´

## **Funciones principales**

1. Conexión a la base de datos:

* Uso de PDO con configuración externa.
* Manejo de excepciones al conectar.
2. Operaciones CRUD:
* Crear: Añadir nuevos registros a la base de datos.
* Leer: Mostrar registros con filtrado dinámico.
* Actualizar: Editar información existente.
* Eliminar: Eliminar registros específicos.
  3. Seguridad:
  * Consultas parametrizadas para prevenir inyecciones SQL.
  * Validación básica de entradas.
 
  ## **Autor**
- Nombre: Víctor García
- Fecha de última actualización: 18/11/2024
