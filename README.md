<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

### Descripción del Proyecto
Este es CMS construido con Laravel, tiene una funcionalidad completa con roles de usuarios.

### Para qué lo uso este proyecto
- Marco Laravel 10
- Viento de cola para el frente y el administrador
- Políticas de Laravel
- Puertas de Laravel
- Correo Laravel
- Laravel Colas (Boletín semanal de construcción)
- Regla de validación personalizada
- Comentarios, Aplicados (relación polimórfica)
- Relaciones aplicadas (uno a muchos y muchos a muchos) entre modelos
- Recuento de vistas de publicaciones usando cookies
- Falsificador y sembrador de bases de datos
- jQuery
- URL de slug amigables con SEO
  
### Funcionalidad del proyecto
#### Panel de administrador
- Editar información general del blog,
- Crear/Actualizar/Eliminar (Categorías, Publicaciones, Etiquetas y Páginas Personalizadas)
- Administrar roles

### Panel de escritores
- Crear, actualizar y eliminar sus propias publicaciones
- Crear, actualizar y eliminar etiquetas.

### Roles
                    
Role Name  | Role_ID
------------- | -------------
Admin  | 1
Writer | 2 
User | 3
                

### Gate Function
Hay un inicio de sesión de filtro de puerta cuando el usuario inicia sesión en el panel de administración, si el usuario es administrador, tendrá funciones completas para administrar el blog y si es un escritor, tendrá pocas funciones.

### Api Routes
                    
Method  | End_Point | Description
------------- | ------------- | -------------
GET | api/categories | Show All Categories
GET | api/categories/{id} | Show All Posts inside Specific Category
GET | api/posts | Show All Posts
GET | api/posts/{id} | Show Specific Post

## Requerimientos
- PHP >= 8.1
- MySQL u otro servidor de base de datos
- Composer
- NodeJS

### Cómo instalar
1. Clonar el proyecto
2. Vaya al directorio raíz del proyecto y ejecute `composer install` y `npm install`
3. Crear `.env` archivar y copiar contenido de `.env.example`
4. Correr `php artisan key:generate` desde terminal
5. Cambiar la información de la base de datos en `.env`
6. Ejecutar migraciones ejecutando `php artisan migrate` , Entonces corre  `php artisan db:seed` si quieres usar registros de base de datos falsos
7. Correr `php artisan storage:link` desde terminal para mostrar las imagenes cargadas
8. Comience el proyecto ejecutando el sitio publico `php artisan serve`
9. Comience el proyecto ejecutando el sitio administrador `npm run dev`
10. Ahora tienes el cms corriendo.

