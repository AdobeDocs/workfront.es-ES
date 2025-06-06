---
title: Actividad de la versión de Adobe Workfront Planning para 2023
description: Actualmente, las funcionalidades de Adobe Workfront Planning están disponibles para determinados clientes de Workfront. Lea este artículo con frecuencia para obtener más información sobre las funciones lanzadas recientemente para las funciones de planificación.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 8a3830e8-0d9a-4ede-a1b6-b80dd4686bc6
source-git-commit: 46faf723ea7a8e9dfa02c0f2bed1f5f450976fc8
workflow-type: tm+mt
source-wordcount: '2900'
ht-degree: 96%

---


# Actividad de la versión de Adobe Workfront Planning para 2023

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

Este artículo enumera las funciones que se lanzaron durante la fase inicial de Workfront Planning en 2023, antes del lanzamiento general de disponibilidad el 28 de agosto de 2024.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Cronología de la versión de Workfront Planning

<!-- this section is also duplicated in the 2024 release notes article-->

La siguiente tabla muestra la cronología de la versión de Workfront Planning:

| Hora | Versión |
|--------------------|-----------------------------------------|
| De agosto a diciembre de 2023 | Versión beta de Workfront Planning* |
| Enero-agosto de 2024 | Versión anticipada de Workfront Planning* |
| jueves, 28 de agosto de 2024 | Disponibilidad general de Workfront Planning |

*Las fases beta y de lanzamiento anticipado estaban disponibles para un grupo limitado de clientes.

## Semana del 25 de diciembre de 2023

### Buscar en la vista de línea de tiempo

Previsualización y producción: 27 de diciembre de 2023

Ahora puede buscar una palabra clave para encontrar rápidamente un registro en la vista de línea de tiempo. Puede utilizar palabras clave y caracteres especiales de cualquier campo visible en la pantalla para buscar un registro. Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Semana del 18 de diciembre de 2023

### Añadir comentarios a los registros desde la página del registro

Vista previa y producción para todos los clientes: 18 de diciembre de 2023

>[!NOTE]
>
>Las siguientes funciones estarán disponibles en el entorno de producción con la versión de enero de 2024:
>
>* Búsqueda de comentarios
>
>* Copia y pegado de imágenes
>
>* Función arrastrar y soltar imágenes
>
>Para obtener más información, consulte [Información general sobre la versión del primer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

Ahora puede colaborar con otros en registros individuales, añadiendo comentarios o respondiendo a otros mientras ve la página de un registro.

La experiencia de comentarios para las capacidades de planificación coincide con la nueva experiencia de comentarios para los objetos de Workfront.

Para obtener más información, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).

### Conector de Workfront Planning para Adobe Workfront Fusion

Producción: 21 de diciembre de 2023

>[!IMPORTANT]
>
>Su organización debe adquirir Adobe Workfront Fusion para poder crear conexiones con las funciones de Adobe Workfront Planning.
>
>Para obtener más información, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

Ahora puede utilizar Adobe Workfront Fusion para conectarse a las funciones de planificación. Con la nueva conexión Fusion, puede hacer lo siguiente:

* Crear, leer, actualizar y eliminar registros

* Obtener una lista de registros por tipo de registro

* Eliminar u obtener una lista de tipos de registros

* Búsqueda de registros

* Realizar una llamada de API

* Activar un escenario cuando se realiza un cambio en las capacidades de planificación

Para obtener más información, consulte [Módulos de Adobe Workfront Planning](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules).

## Semana del 11 de diciembre de 2023

### Actualizar el campo principal en una vista de tabla de un tipo de registro

Previsualización y producción: 14 de diciembre de 2023

Ahora puede elegir el campo que desea mostrar en la primera columna de una vista de tabla. Este campo ahora se denomina campo principal.

Antes de esta mejora, el campo Nombre de un registro siempre se mostraba en la primera columna de la vista de tabla y no se podía colocar en otra posición.

Con esta mejora, observe lo siguiente:

* De forma predeterminada, la columna o el campo Nombre sigue siendo la primera columna de una tabla.

* Puede elegir cualquier campo de los siguientes tipos para que sea un campo principal y reemplazar el campo Nombre en la primera columna:

   * Texto de línea única

   * Número

   * Fórmula

* El campo principal de una vista de tabla siempre está inmovilizado y no se puede mover, a menos que establezca otro campo como campo principal.

* Puede cambiar el campo principal de un encabezado de columna no principal.

* Todas las vistas de tabla de un tipo de registro tienen el mismo campo principal que seleccione.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

### Conexión de registros de funcionalidad de planificación a Adobe Experience Manager Assets

Versión de vista previa: 14 de diciembre de 2023

Versión de producción: 21 de diciembre de 2023

>[!IMPORTANT]
>
>La instancia de Workfront de su organización debe incorporarse a Adobe Business Platform o Adobe Admin Console para poder conectar los registros de funcionalidades de Adobe Workfront Planning a Adobe Experience Manager Assets.
>
>Si tiene preguntas sobre la incorporación a Adobe Admin Console, consulte las [Preguntas frecuentes sobre la experiencia unificada de Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Ahora puede establecer una conexión entre los tipos de registro de funcionalidades de Adobe Workfront Planning y Adobe Experience Manager Assets.

Después de establecer la conexión, esta actualización incluye la siguiente funcionalidad:

* Puede vincular recursos y carpetas de Experience Manager a un registro de funcionalidad de planificación desde un repositorio específico de Experience Manager Assets al que tengan acceso. En este proceso, puede conectar los campos de recursos a los campos de funcionalidad de planificación.

* Los usuarios de la funcionalidad de planificación pueden ver el nombre de los recursos conectados, así como los valores de los campos conectados, en las funcionalidades de la planificación.

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Planning after you establish the connection. Connected assets are visible in the table and timeline views of this new record type.  
-->

* Puede hacer clic en el nombre de recurso en la vista de tabla del registro de funcionalidad de planificación desde el campo de registro conectado y ver una ventana emergente con la miniatura del recurso y varios campos clave. En la ventana emergente, puede navegar hasta el visor de recursos en Experience Manager y ver todos los detalles sobre él.

Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

## Semana del 4 de diciembre de 2023

### Copiar y pegar información de un campo a otro en la vista de tabla de funcionalidad de planificación para los campos de tipo Personas y de registro vinculado

Vista previa y producción: 5 de diciembre de 2023

Ahora puede copiar y pegar información de un campo a otro del mismo tipo en una vista de tabla de tipo de registro. Esta funcionalidad ahora se admite para los siguientes tipos de campos:

* Personas
* Campos de registro vinculados

Tenga en cuenta lo siguiente:

* Copiar y pegar valores de campo de un campo a otro es posible con los campos que muestran varios valores.

* No puede copiar información de otro origen que no sea un campo de funcionalidad de planificación del mismo tipo que el campo en el que pega la información.

* No se pueden copiar y pegar valores de campo para los campos que se muestran en el área Detalles de un registro.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Para obtener información sobre los campos vinculados, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

## Semana del 27 de noviembre de 2023

### Copiar y pegar información de un campo a otro en la vista de tabla de funcionalidad de planificación

Vista previa y producción: 28 de noviembre de 2023

Ahora puede copiar y pegar información de un campo a otro del mismo tipo en una vista de tabla de tipo de registro de funcionalidad de planificación.

Tenga en cuenta lo siguiente:

* No puede copiar información de otro origen que no sea un campo de funcionalidad de planificación del mismo tipo que el campo en el que pega la información.

* No se pueden copiar y pegar valores de campo para los campos que se muestran en el área Detalles de un registro.

* No puede copiar y pegar valores de campo para los siguientes tipos de campo:

   * Personas

   * Campos del sistema

   * Campos vinculados creados como resultado de la conexión de registros

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Semana del 6 de noviembre de 2023

### Agrupación para la vista de tabla

Previsualización y producción: 7 de noviembre de 2023

Ahora puede agrupar registros en la vista de tabla de una página de tipo de registro. Puede agrupar por tres campos únicos en la interfaz de funcionalidad de planificación<!--checking into this for now: and by four fields when using the API-->.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Semana del 30 de octubre de 2023

### Nuevos tipos de campos para campos de usuario y fecha para capturar quién creó o modificó por última vez un registro o en qué fecha

Previsualización y producción: 30 de octubre de 2023

Hemos introducido los siguientes tipos de campos para los registros de funcionalidades de Adobe Workfront Planning:

* Creado por

* Fecha de creación

* Última modificación realizada por

* Fecha de la última modificación

Los valores de campo de los campos creados a partir de estos tipos de campo son de solo lectura y capturan el nombre del usuario que creó o modificó por última vez un registro, o la fecha en la que se creó o modificó por última vez el registro.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

### Navegar a objetos de Workfront desde un registro de funciones de planificación

Vista previa y producción: 31 de octubre de 2023

Ahora puede abrir las páginas de objetos de Workfront desde las siguientes áreas de Workfront Planning:

* La vista de tabla del registro de objetos de Workfront vinculados de solo lectura

* La página de registro de objetos de Workfront de solo lectura

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

### Se ha mejorado la navegación en la vista de tabla

Vista previa y producción: 2 de noviembre de 2023

Hemos mejorado la navegación en la vista de tabla de una página de tipo de registro.

A continuación se indican algunas de las mejoras:

* Utilice la tecla Tab del teclado para desplazarse por las columnas y filas de la tabla

* Añada un nuevo registro desde cualquier posición de columna. Antes de esta mejora, solo podía añadir un registro desde la primera columna.

* Utilice la combinación de teclado Mayús + Intro para añadir un nuevo registro (o fila) en la tabla.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Semana del 16 de octubre de 2023

### Nuevo tipo de campo Personas

Vista previa y producción: 16 de octubre de 2023

Ahora puede añadir un campo de tipo Personas a los tipos de registro de funcionalidades de planificación. Puede utilizar campos de tipo Personas para asociar usuarios existentes con un registro. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

### Texto enriquecido: formato para campos de párrafo

Vista previa y producción: 16 de octubre de 2023

Se han añadido controles de formato de texto enriquecido para los campos de tipo párrafo. Puede dar formato a los campos de párrafo mediante Texto enriquecido en la vista Tabla de un tipo de registro o en la página de registro. Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).


### Registro y agrupación de códigos de color para la vista Linea de tiempo

Previsualización y producción: 19 de octubre de 2023

Ahora puede codificar con colores las barras de registro y las agrupaciones en la vista Línea de tiempo.

Las siguientes son opciones para los colores que puede elegir mostrar para las barras de registros y agrupaciones en la vista Línea de tiempo:

* Las agrupaciones pueden coincidir con los colores siguientes:

   * Gris (valor predeterminado)

   * El color del campo por el que se agrupa

* Las barras pueden coincidir con los colores siguientes:

   * El color del tipo de registro

   * El color del campo que seleccione

   * El color de la agrupación

   * Sin color (predeterminado)

Al hacer coincidir colores con un campo determinado, solo puede seleccionar campos con opciones codificadas por colores.

Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Semana del 9 de octubre de 2023

### Buscar en la vista de tabla

Previsualización y producción: 9 de octubre de 2023

Ahora puede buscar una palabra clave para encontrar rápidamente un registro en la vista de tabla. Puede utilizar palabras clave y caracteres especiales de cualquier campo visible en la pantalla para buscar un registro. Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Semana del 18 de septiembre de 2023

### Reordenar filas

Previsualización y producción: 20 de septiembre de 2023

Ahora puede reordenar una o varias filas (o registros) en la vista Tabla de una página de tipo de registro. Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Semana del 4 de septiembre de 2023

### Conexión de registros de capacidades de planificación con empresas y grupos de Workfront

Previsualización y producción: 5 de septiembre de 2023

Ahora puede conectar un registro de capacidad de planificación con empresas y grupos de Workfront. Primero debe crear una conexión entre un tipo de registro de capacidad de planificación y los tipos de metas de empresas y grupos de Workfront. A continuación, puede conectar un único registro de capacidad de planificación del tipo de registro seleccionado a empresas y grupos de Workfront individuales.

Tenga en cuenta lo siguiente:

* Debe crear una conexión entre los tipos de registro de capacidades de planificación y los tipos de objeto Compañía y Grupo de Workfront para cada espacio de trabajo.

* No puede conectar tipos de registros de taxonomía con tipos de objetos de Workfront.

* Puede conectar varios registros de capacidad de planificación a la misma compañía o grupo de Workfront, y varias compañías o grupos al mismo registro de capacidad de planificación.

* No se pueden editar compañías o grupos en las funciones de planificación. Todos los cambios de empresa o grupo realizados en Workfront se pueden ver en las funciones de planificación al revisar las funciones de planificación y los registros vinculados.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)

### Compatibilidad con URL para campos de texto de una sola línea

Previsualización y producción: 7 de septiembre de 2023

Para obtener una mejor visibilidad al trabajar con vínculos en la vista de tabla, se ha añadido compatibilidad con direcciones URL en campos de texto de una sola línea. El uso de direcciones URL en otros sitios web o unidades externas al actualizar un campo de texto de una sola línea, ahora las identifica como vínculos y le permite hacer clic en ellas desde la tabla. Antes de esta mejora, los vínculos se mostraban como texto.

## Semana del 28 de agosto de 2023

### Menú de visibilidad de campos para la barra de herramientas Vista de tabla

Previsualización y producción: 31 de agosto de 2023

Para mostrar la información correcta en un conjunto determinado de registros, especialmente si tiene intención de compartir la vista con otras personas que deben ver algunos campos de un tipo de registro, pero no todos, ahora puede seleccionar qué campos (o columnas) mostrar y cuáles ocultar en la vista Tabla.

Puede ocultar o mostrar campos individuales de cada encabezado de las columnas de campo, o bien puede administrar todos los campos del tipo de registro desde una configuración de la barra de herramientas de la vista de tabla.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Semana del 21 de agosto de 2023

### Conexión de registros de funciones de Adobe Workfront Planning a programas y portafolios

Previsualización y producción: 24 de agosto de 2023

Ahora puede conectar un registro de funciones de planificación con programas y portafolios de Workfront. Debe crear una conexión entre un tipo de registro de funciones de planificación y un programa o portafolio que cree un campo conectado. A continuación, puede conectar cualquier registro de funciones de planificación de todos los demás tipos de registro del mismo espacio de trabajo a programas y portafolios específicos, lo que crea un tipo de registro de solo lectura de portafolios de Workfront o Programa Workfront en el mismo espacio de trabajo. Tenga en cuenta lo siguiente:

* Los tipos de registros de conector de Workfront son únicos en cada espacio de trabajo.
* Puede conectar varios registros de funcionalidades de planificación al mismo programa o portafolio de Workfront, y varios programas y portafolios al mismo registro de funcionalidades de planificación.
* No puede editar programas y portafolios en las funcionalidades de planificación. Todos los cambios de programas y portafolios realizados en Workfront se pueden ver en las funcionalidades de planificación al revisar los registros vinculados.

### Nueva funcionalidad de ordenación para la vista de tabla

Previsualización y producción: 24 de agosto de 2023

Ahora puede ordenar registros en la vista de tabla de una página de tipo de registro.
Ya están disponibles las siguientes funcionalidades:

* Ordenación a nivel de tabla, donde puede ordenar por varios campos al mismo tiempo.
* Ordenación a nivel de columna o de campo, donde puede ordenar por un campo individual a la vez.

### Mejoras en la vista de la línea de tiempo: nuevo aspecto para las agrupaciones y el conmutador de vista Compacto/Estándar

Previsualización y producción: 24 de agosto de 2023

Hemos introducido las siguientes mejoras en la vista de línea de tiempo:

* Ahora puede visualizar la vista de línea de tiempo en los modos siguientes:

   * Estándar: muestra los registros en líneas independientes.
   * Compacto: muestra los registros cuyas fechas no se cruzan en la misma línea.

* Hemos cambiado el aspecto de las líneas de agrupación en la vista de la línea de tiempo para que se muestren encima de la línea de tiempo de los registros que contienen. Antes de esta mejora, las líneas de agrupación se mostraban en toda la longitud de la línea de tiempo

## Semana del 14 de agosto de 2023

### Reordenación de columnas en la vista de tabla

Ahora puede reordenar las columnas en la vista de tabla. Tenga en cuenta lo siguiente al reordenar las columnas:

* El campo Nombre es siempre el primer campo de la vista de tabla de una página de tipo de registro

* No puede mover el campo Nombre a otra posición

* El campo Nombre está inmovilizado y no forma parte del desplazamiento horizontal

### Desplazamiento horizontal para la vista de línea de tiempo

Ahora puede desplazarse horizontalmente en la vista de la línea de tiempo de un tipo de registro.

## Semana del 7 de agosto de 2023

### Importación de tipos de registros desde un archivo de Excel

Vista previa y producción: 10 de agosto de 2023

Ahora puede importar un archivo de Excel para crear tipos de registros en un espacio de trabajo. Las hojas del archivo se convierten en los tipos de registro, y las columnas del archivo se convierten en sus respectivos campos.

### Experiencia mejorada para conectar tipos de registros y proyectos

Vista previa y producción: 10 de agosto de 2023

Hemos mejorado la forma de conectar los tipos de registros, incluida la conexión a proyectos de Workfront. Como parte de esta mejora, hemos realizado los siguientes cambios al añadir un campo para un tipo de registro desde la vista de tabla:

* Se ha eliminado el campo de tipo Relación de la pestaña &quot;Nuevo campo&quot;.

* Añada una pestaña &quot;Nueva conexión&quot; en la que puede seleccionar directamente el tipo de registro u objeto al que desea conectarse, lo que elimina la necesidad de un campo de tipo Relación.

## Semana del 10 de julio de 2023

### Actualización del aspecto de un tipo de registro

Vista previa y producción: 13 de julio de 2023

Ahora puede seleccionar un icono personalizado para un tipo de registro y un color personalizado para el icono de tipo de registro.

### Nuevo tipo de campo Casilla de verificación

Vista previa y producción: 13 de julio de 2023

Ahora puede añadir un tipo de campo Casilla de verificación a los tipos de registro de funcionalidad de planificación. Puede utilizar un campo de tipo Casilla de verificación para añadir una sola opción de casilla de verificación a un registro. Puede utilizar este campo para indicar un atributo o estado específico para ese registro en particular. Por ejemplo, puede utilizarlo como indicador para realizar un seguimiento de la finalización, la aprobación o cualquier otro atributo binario de cada registro.

## Semana del 26 de junio de 2023

### Activación rápida del menú contextual en una tabla

Vista previa y producción: 28 de junio de 2023

Hemos habilitado la capacidad de activar el menú contextual haciendo clic con el botón derecho en cualquier lugar de una fila de registro, al visualizar los registros en la vista de tabla o en un tipo de registro. Ahora se puede ver, eliminar o copiar rápidamente un vínculo a la página del registro al acceder al menú contextual desde cualquier lugar de la vista de tabla de un tipo de registro. Antes de esta mejora, al menú contextual solo se podía acceder desde el menú Más de la columna Nombre de un registro.

## Semana del 19 de junio de 2023

### Los nombres de los campos de registro son únicos

Ahora hemos introducido el requisito de que los nombres de campo de un tipo de registro de funcionalidades de planificación deben tener nombres únicos. Los campos que pertenecen a diferentes tipos de registro no tienen por qué tener nombres únicos.

## Semana del 5 de junio de 2023

### Conexión de registros de funcionalidades de Adobe Workfront Planning con proyectos de Workfront

Vista previa y producción: 5 de junio de 2023

Ahora puede conectar un registro de funcionalidades de planificación con proyectos de Workfront. Debe crear un tipo de registro de funcionalidades de planificación del conector para establecer la conexión entre los registros de funcionalidades de planificación y los proyectos de Workfront. A continuación, puede conectar cualquier registro de funcionalidades de planificación de los restantes tipos de registro al registro del conector mediante el campo Relación. Tenga en cuenta lo siguiente:

* Debe tener un tipo de registro de conector de Workfront para cada espacio de trabajo.
* Puede conectar varios registros de funcionalidades de planificación al mismo proyecto de Workfront, y varios proyectos al mismo registro de funcionalidades de planificación.
* No se pueden editar proyectos en las funcionalidades de planificación. Todos los cambios de proyectos realizados en Workfront se pueden ver en las funcionalidades de planificación al revisar los registros vinculados.

## Semana del 29 de mayo de 2023

### Requisito de dos fechas para crear una vista Escala de tiempo

Vista previa y producción: 31 de mayo de 2023

Debe tener al menos dos campos de fecha asociados a un tipo de registro para crear una vista Escala de tiempo.
