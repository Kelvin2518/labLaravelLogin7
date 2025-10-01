cat << 'EOF' > README.md
# 📌 CMDB System  
## Sistema de Gestión de Activos y Configuración  

Este proyecto es la culminación del curso **Desarrollo VII (PHP)**, impartido por la **Profesora Irina Fong** en la **Universidad Tecnológica de Panamá**.  

El laboratorio consiste en la implementación de un módulo de inicio de sesión (**login**) en el framework **Laravel**, siguiendo la arquitectura de diseño **Modelo-Vista-Controlador (MVC)**.  

###  Arquitectura MVC
- **Modelos** → Se encargan de la interacción con la base de datos para manejar la lógica de negocio.  
- **Vistas** → Definen la interfaz de usuario, como las páginas HTML.  
- **Controladores** → Actúan como intermediarios, procesando las solicitudes de los usuarios y devolviendo las respuestas adecuadas.  
- **Rutas** → Definen las URLs que se utilizan para acceder a las diferentes partes de la aplicación.  

---

## 1️. Prerrequisitos e Instalación  

Antes de ejecutar este proyecto, asegúrate de contar con los siguientes componentes:  

- **Servidor Web**: Apache o Nginx  
- **PHP**: Versión 8.1 o superior  
- **Base de Datos**: MySQL o MariaDB  
- **Composer**: Para la gestión de dependencias de PHP  
- **Editor de Código**: Visual Studio Code (recomendado)  
- **Entorno Local**: XAMPP, WampServer o Laragon  

###  Configuración del proyecto  
Ejecuta los siguientes comandos:  

# Clonar el repositorio
git clone https://github.com/Kelvin2518/labLaravelLogin7.git

# Instalar dependencias PHP
composer install

# Instalar paquete de autenticación
composer require laravel/ui 

# Generar el andamiaje de autenticación
php artisan ui bootstrap --auth 

# Instalar dependencias de NPM y compilar
npm install && npm run dev

2️. Base de Datos

El proyecto utiliza un archivo .env para la configuración de la conexión.
La base de datos definida es: lablaravellogin7.

📂 Migraciones

Para crear las tablas necesarias para el login de Laravel (incluyendo users y sessions) se usaron migraciones:
php artisan migrate:fresh

3️. Dificultades y Soluciones

a. Error de conexión a la base de datos

b. Problema: Laravel no encontraba la BD.

c. Solución: Corregir el nombre en .env a lablaravellogin7.

QueryException y Table already exists


a. Problema: La tabla sessions no existía y la tabla users ya existía.

b. Solución: Ejecutar

c. php artisan migrate:fresh


Esto eliminó todas las tablas y las recreó correctamente.


a. Problemas con Git y subida a GitHub

b. Problema: Errores al subir el proyecto (conflicto entre ramas main y master).

c. Solución: Uso de línea de comandos:

git add .
git commit -m "Primer commit"
git push origin master

4️. Puntos de Referencia


a. Laravel Official Documentation

b. Laravel UI Documentation

c. Styde.net - Tutoriales de Laravel


👨‍💻 Información del Desarrollador
Este laboratorio ha sido desarrollado por el estudiante de la Universidad Tecnológica de Panamá:


Nombre: Kelvin Fernández

Correo: kelvin.fernandez@utp.ac.pa

Curso: ING WEB

Instructor: Ing. Irina Fong

Fecha de Ejecución

1 de octubre de 2025
