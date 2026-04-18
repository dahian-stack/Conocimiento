# Conocimiento

# Descripción general
Mediapro es un sistema de gestion para la industria audiovisual que permite administrar producciones, personal técnico y creativo, equipos, loscalizaciones, procesos de rodaje y postproduccion.
El sistema facilita la organización de la informacion y optimiza los procesos mediante el uso de procedimientos almacenados y vistas.

# Instrucciones de uso
1. Abrir HeidiSQL o cualquier otro gestor de base de datos compatible con MYSQL.
2. Seleccionar la base de datos donde se ejecutarán los scripts.
3. Ejecutar el archivo Scrip - AudiovisualMediapro.txt, el cual contiene los procedimientos almecenados y vistas del sistema.
4. Verificar la creación de los procedimientos y vistas mediante consultas como:
   
   SHOW PROCEDURE STATUS
   
   SHOW FULL TABLES WHERE Table_type = 'VIEW'

# Estructura de módulos implementados
El sistema MediaPro se organiza en los siguientes módulos:

 1. Módulo de Producción
    
    Encargado de gestionar la información de las producciones audiovisuales y sus clientes.
    
    * Tablas: Cliente, Produccion

3. Módulo de Peronal
   
Gestiona el personal técnico y creativo asignado a cada producción.

* Tablas: Personal, Produccion_Personal

3. Módulo de Rodaje
   
Planifica y organiza los días de grabación, incluyendo escenas, actores y recursos.

* Tablas: Plan_Rodaje, Plan_Rodaje_Escena, Plan_Rodaje_Actor, Plan_Rodaje_Equipo

4. Módulo de Escenas y Actores
   
Administra las escenas, personajes y actores que participan en la producción.

* Tablas: Escena, Actor, Personaje, Escena_Actor

5. Módulo de Equipos Técnicos
   
Gestiona los equipos utilizados en las producciones y su mantenimiento.

* Tablas: Equipo_Tecnico, Mantenimiento, Produccion_Equipo

 6. Módulo de Material Grabado
    
Registra el material audiovisual generado durante el rodaje.

* Tablas: Material_Grabado, Audio

 7. Módulo de Postproducción
    
Controla los procesos de edición, versiones y aprobación del material.

* Tablas: Postproduccion, Material_Postproduccion, Versiones, Aprobacion

8. Módulo de Distribución
   
Gestiona la distribución y promoción de las producciones audiovisuales.

* Tablas: Distribucion, Material_Promocional

9. Módulo de Automatización
   
Implementa funcionalidades avanzadas mediante procedimientos almacenados y vistas.

* Stored Procedures
* Views
