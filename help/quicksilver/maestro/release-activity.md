---
title: Actividad de versión de Adobe Maestro
description: Utilizar Maestro para crear objetos, campos y espacios de trabajo personalizados.
hidefromtoc: true
hide: true
source-git-commit: 6e219089f68db651f5eb8369e3c6df83b6cd823b
workflow-type: tm+mt
source-wordcount: '1432'
ht-degree: 0%

---


# Actividad de versión de Adobe Maestro

>[!IMPORTANT]
>
>En la actualidad, Adobe Maestro forma parte de un programa beta cerrado que está abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro/maestro-overview.md).

Este artículo enumera las funciones que se han publicado tras el lanzamiento del programa beta cerrado de Maestro, el 22 de mayo de 2023.

Las funciones lanzadas se enumeran en el orden de su lanzamiento, con las más recientes primero. Los clientes que participan en el programa beta cerrado de Maestro pueden acceder a todas las funciones en sus entornos de Previsualización y Producción.

>[!IMPORTANT]
>
>La documentación a la que se hace referencia en las secciones siguientes estará disponible un tiempo después de que las funciones se publiquen en el entorno de producción.

En esta sección se enumeran las funciones y revisiones que se han publicado tras el lanzamiento del programa beta cerrado de Maestro el 22 de mayo de 2023.

Las funciones se lanzan semanalmente y se enumeran en el orden de lanzamiento, empezando por las más recientes. Los clientes que participan en el programa beta cerrado de Maestro pueden acceder a todas las funciones en sus entornos de Previsualización y Producción.

## Semana del 4 de septiembre de 2023

### Conectar registros de Maestro con empresas y grupos de Workfront

Vista previa y producción: 5 de septiembre de 2023

Ahora puede conectar un registro de Maestro con empresas y grupos de Workfront. Primero debe crear una conexión entre un tipo de registro de Maestro y los tipos de objetos de empresas y grupos de Workfront. A continuación, puede conectar un único registro Maestro del tipo de registro seleccionado a empresas y grupos individuales de Workfront.

Tenga en cuenta lo siguiente:

* Debe crear una conexión entre los tipos de registros de Maestro y los tipos de objetos Compañía y Grupo de Workfront para cada Espacio de trabajo.

* No puede conectar tipos de registros de taxonomía con tipos de objetos de Workfront.

* Puede conectar varios registros de Maestro a la misma compañía o grupo de Workfront y varias compañías o grupos al mismo registro de Maestro.

* No puede editar compañías o grupos en Maestro. Todos los cambios de compañía o de grupo realizados en Workfront se pueden ver en Maestro al revisar los registros vinculados de Maestro.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registros](../maestro/architecture-and-fields/connect-record-types.md)
   * [Conectar registros](../maestro/records/connect-records.md)

### Compatibilidad con URL para campos de texto de una sola línea

Previsualización y producción: 7 de septiembre de 2023

Para obtener una mejor visibilidad al trabajar con vínculos en la vista de tabla, se ha agregado compatibilidad con direcciones URL en campos de texto de una sola línea. El uso de direcciones URL a otros sitios web o unidades externas al actualizar un campo de texto de una sola línea, ahora las identifica como vínculos y le permite hacer clic en ellas desde la tabla. Antes de esta mejora, los vínculos se mostraban como texto.

## Semana del 28 de agosto de 2023

### Menú de visibilidad de campos para la barra de herramientas Vista de tabla

Previsualización y producción: 31 de agosto de 2023

Para mostrar la información correcta en un conjunto determinado de registros, especialmente si tiene intención de compartir la vista con otras personas que deben ver algunos campos de un tipo de registro, pero no todos, ahora puede seleccionar qué campos (o columnas) mostrar y cuáles ocultar en la vista Tabla.

Puede ocultar o mostrar campos individuales de cada encabezado de las columnas de campo, o bien puede administrar todos los campos del tipo de registro desde una configuración de la barra de herramientas de la vista de tabla.

Para obtener más información, consulte [Administrar la vista de tabla](../maestro/views/manage-the-table-view.md).

## Semana del 21 de agosto de 2023

### Conectar registros de Maestro a programas y portafolios

Previsualización y producción: 24 de agosto de 2023

Ahora puede conectar un registro de Maestro con programas y portafolios de Workfront. Debe crear una conexión entre un tipo de registro Maestro y un programa o portafolio que cree un campo conectado. A continuación, puede conectar cualquier registro de Maestro de todos los demás tipos de registro del mismo área de trabajo a programas y portafolios específicos, lo que crea un tipo de registro de sólo lectura de programa de Workfront o de Portfolio de Workfront en el mismo área de trabajo. Tenga en cuenta lo siguiente:

* Los tipos de registros del conector de Workfront son únicos para cada espacio de trabajo.
* Puede conectar varios registros de Maestro al mismo programa o portafolio de Workfront y varios programas y portafolios al mismo registro de Maestro.
* No puede editar programas y portafolios en Maestro. Todos los cambios de programas y portafolios realizados en Workfront se pueden ver en Maestro al revisar los registros vinculados.

### Nueva funcionalidad de ordenación para la vista de tabla

Previsualización y producción: 24 de agosto de 2023

Ahora puede ordenar registros en la vista de tabla de una página de tipo de registro.
Ya están disponibles las siguientes funciones:

* Ordenación en el nivel de tabla, donde puede ordenar por varios campos al mismo tiempo.
* Ordenación en el nivel de columna o de campo, donde puede ordenar por un campo individual a la vez.

### Mejoras en la vista de la cronología: nueva apariencia para las agrupaciones y el conmutador de vista Compacto/ Estándar

Previsualización y producción: 24 de agosto de 2023

Hemos introducido las siguientes mejoras en la vista de cronología:

* Ahora puede mostrar la vista de la cronología en los modos siguientes:

   * Estándar: muestra los registros en líneas independientes.
   * Compacto: muestra los registros cuyas fechas no se cruzan en la misma línea.

* Hemos cambiado el aspecto de las líneas de agrupación en la vista de la cronología para que se muestren encima de la cronología de los registros que contienen. Antes de esta mejora, las líneas de agrupación se mostraban en toda la longitud de la cronología.

## Semana del 14 de agosto de 2023

### Reordenar columnas en la vista de tabla

Ahora puede reordenar columnas en la vista de tabla de Maestro. Tenga en cuenta lo siguiente al reordenar las columnas:

* El campo Nombre es siempre el primer campo de la vista de tabla de una página de tipo de registro

* No se puede mover el campo Nombre a otra posición

* El campo Nombre está inmovilizado y no forma parte del desplazamiento horizontal.

### Desplazamiento horizontal para vista de escala de tiempo

Ahora puede desplazarse horizontalmente en la vista de la cronología de un tipo de registro.

## Semana del 7 de agosto de 2023

### Importar tipos de registros desde un archivo de Excel

Previsualización y producción: 10 de agosto de 2023

Ahora puede importar un archivo de Excel para crear tipos de registros en un espacio de trabajo. Las hojas del archivo se convierten en los tipos de registro, y las columnas del archivo se convierten en sus respectivos campos.

### Experiencia mejorada para conectar tipos de registros y proyectos

Previsualización y producción: 10 de agosto de 2023

Hemos mejorado la forma de conectar los tipos de registros, incluida la conexión a proyectos de Workfront. Como parte de esta mejora, hemos realizado los siguientes cambios al agregar un campo para un tipo de registro desde la vista de tabla:

* Se ha eliminado el campo Relationship-type de la pestaña &quot;New field&quot;.

* Añada una pestaña &quot;Nueva conexión&quot; donde puede seleccionar directamente el tipo de registro u objeto al que desea conectarse, lo que elimina la necesidad de un campo de tipo Relación.

## Semana del 10 de julio de 2023

### Actualizar el aspecto de un tipo de registro

Previsualización y producción: 13 de julio de 2023

Ahora puede seleccionar un icono personalizado para un tipo de registro y un color personalizado para el icono de tipo de registro.

### Nuevo tipo de campo Casilla

Previsualización y producción: 13 de julio de 2023

Ahora puede agregar un tipo de campo Casilla de verificación a los tipos de registro Maestro. Puede utilizar el tipo de campo Casilla de verificación para agregar una sola opción de casilla de verificación a un registro. Puede utilizar este campo para indicar un atributo o estado específico para ese registro en particular. Por ejemplo, puede utilizarlo como indicador para rastrear la finalización, la aprobación o cualquier otro atributo binario de cada registro.

## Semana del 26 de junio de 2023

### Activación rápida del menú contextual en una tabla

Previsualización y producción: 28 de junio de 2023

Hemos habilitado la capacidad de activar el menú contextual haciendo clic con el botón derecho en cualquier lugar de una fila de registro, cuando se visualizan los registros en la vista de tabla o en un tipo de registro. Ahora puede ver, eliminar o copiar rápidamente un vínculo a la página Detalles del registro al acceder al menú contextual desde cualquier lugar de la vista de tabla de un tipo de registro. Antes de esta mejora, el menú contextual solo era accesible desde el menú Más en la columna Nombre de un registro.

## Semana del 19 de junio de 2023

### Los nombres de los campos de registro son únicos

Hemos introducido el requisito de que los nombres de campo de un tipo de registro Maestro deben tener nombres únicos. Los campos que pertenecen a diferentes tipos de registro no tienen por qué tener nombres únicos.

## Semana del 5 de junio de 2023

### Conectar registros de Maestro con proyectos de Workfront

Previsualización y producción: 5 de junio de 2023

Ahora puede conectar un registro de Maestro con proyectos de Workfront. Debe crear un tipo de registro de conector Maestro para establecer la conexión entre registros de Maestro y proyectos de Workfront. A continuación, puede conectar cualquier registro de Maestro de todos los demás tipos de registro al registro del conector mediante el campo Relación. Tenga en cuenta lo siguiente:

* Debe tener un tipo de registro de conector para Workfront para cada espacio de trabajo.
* Puede conectar varios registros de Maestro al mismo proyecto de Workfront y varios proyectos al mismo registro de Maestro.
* No puede editar proyectos en Maestro. Todos los cambios de proyecto realizados en Workfront se pueden ver en Maestro al revisar los registros vinculados.

## Semana del 29 de mayo de 2023

### Requisito de dos fechas para crear una vista Cronología

Previsualización y producción: 31 de mayo de 2023

Debe tener al menos dos campos de fecha asociados a un tipo de registro para crear una vista Línea de tiempo.