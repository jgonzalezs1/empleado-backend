# empleado-backend

Para ejecutar este API se debe de contar con las siguientes bibliotecas de clases

-TalentoHumanoAPI
-TalentoHumanoData

En TalentoHumanoAPI se encuentran las carpetas Controllers y Services
En TalentoHumanoData se encuentran las carpetas Migrations, Models y Repositories

Estructura del Proyecto

TalentoHumanoAPI

Controllers: EmpleadoController.cs
Services:
-Impl: IEmpleadoService.cs
EmpleadoService.cs

TalentoHumanoData

Migrations
-DbContext: TalentoHumanoContext.cs
Models
-Empleado.cs
Repositories
-Impl: IEmpleadoRepository.cs
EmpleadoRepository.cs

Pasos para ejecutar TalentoHumanoAPI

1.- Se inicia desde el API, debe de tener el Swagger instalado
2.- Se ejecuta el DbContext para crear una Base de Datos con tablas migradas, a través de appsettings.json donde se obtiene el String "DevConnection"
3.- Se debe de incluir en Startup. cs lo siguiente
-Swagger
-Repository
-Service
-DbContext
-Cors
Esto permite que al momento de ejecutar el API nos devuelva datos de un CRUD de una tabla migrada de EF
4.- Ejecutar desde los puertos http://localhost:5000 o http://localhost:5001
5.- Probar los CRUDs ejecutados desde el servidor
6.- Verificar la data actualizada en SQL Server

Happy coding
Jose Gonzalez
