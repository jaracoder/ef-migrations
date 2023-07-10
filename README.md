# Repositorio de Migraciones de Entity Framework

Este repositorio contiene las migraciones de Entity Framework (EF) para el proyecto. Proporciona un enfoque organizado para gestionar los cambios en el esquema de la base de datos utilizando EF Core.

## Agregar una Migración

Para agregar una nueva migración, utiliza el siguiente comando:

```bash
dotnet ef migrations add MigrationDescription --startup-project ../JARACoder -v
```
+ `dotnet ef migrations add`: Este comando se utiliza para crear una nueva migración.
+ `MigrationDescription`: El nombre de la migración. Puedes personalizarlo según tus necesidades.
+ `--startup-project ../JARACoder`: Especifica el proyecto de inicio donde se encuentra el DbContext.
+ `-v`: Habilita la salida detallada para obtener información detallada durante el proceso de migración.

## Aplicar Migraciones

Para aplicar las migraciones y actualizar la base de datos, utiliza el siguiente comando:

```bash
dotnet ef database update --startup-project ../JARACoder -v
```

+ dotnet ef database update: Este comando aplica las migraciones pendientes en la base de datos.
+ --startup-project ../JARACoder: Especifica el proyecto de inicio donde se encuentra el DbContext.
+ -v: Habilita la salida detallada para obtener información detallada durante el proceso de actualización.
