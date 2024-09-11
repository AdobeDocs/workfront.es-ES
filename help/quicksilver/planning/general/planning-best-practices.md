---
title: Prácticas recomendadas de planificación de Adobe Workfront
description: Como líder de operaciones de marketing, puede utilizar Adobe Workfront Planning para organizar el trabajo en todo el ciclo de vida de marketing para todos sus equipos. Estas son algunas prácticas recomendadas que recomendamos al comenzar con Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ae10d35c61bf40c9e6f0422bd670b9733ad62aae
workflow-type: tm+mt
source-wordcount: '3225'
ht-degree: 0%

---


<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Prácticas recomendadas de Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Como líder de operaciones de marketing, puede utilizar Adobe Workfront Planning para organizar el trabajo en todo el ciclo de vida de marketing para todos sus equipos.

Este artículo documenta algunas preguntas frecuentes y prácticas recomendadas que recomendamos al comenzar con Workfront Planning.

## Prácticas recomendadas de configuración

### Espacios de trabajo

Los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo. Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo.

Las siguientes son algunas de las preguntas más frecuentes sobre la configuración de Workfront Planning.

#### ¿Cómo debo empezar?

* ✅ Cuando inicie sesión en Planning por primera vez, siga nuestro proceso de incorporación en la aplicación que comunique claramente el valor de Planning y le guíe en cómo navegar y utilizar el producto de forma eficaz. Esto garantiza que entienda sus capacidades y cómo comenzar su trabajo con facilidad.
* ✅ Empiece explorando nuestras plantillas de espacio de trabajo predefinidas para conocer ideas de casos de uso similares existentes. Puede utilizar los tipos de registros predefinidos y los campos que se incluyen en una plantilla, o bien puede agregar los suyos propios.
* ✅ Identifique los casos de uso principales que desea resolver con Workfront Planning. Por ejemplo, la mayoría de las organizaciones quieren mejorar la visibilidad de las actividades estratégicas, lo que puede incluir la creación de un mejor &quot;Calendario de campaña&quot;. Por lo tanto, para ese caso de uso, le recomendamos empezar respondiendo a algunas preguntas:

   * ¿Quién lo pide?
   * ¿Cómo llaman a las cosas que quieren poner en el calendario?
¿Campañas? ¿Tácticas? ¿Iniciativas? ¿Actividades? ¿Eventos?
   * ¿Qué tipo de preguntas quieren responder con este calendario?
   * ¿Hay campañas superpuestas para la misma audiencia?
   * ¿Cuál es nuestro presupuesto para esa campaña, táctica, actividad o evento?

  Las respuestas a estas preguntas dictarían lo que debe crear dentro de Workfront Planning.

  Además, tenga en cuenta que puede haber otros planificadores que actualmente no sean usuarios de Workfront. Estos planificadores pueden operar desde hojas de cálculo de Excel, documentos de Word, PowerPoints, etc. Piense en cómo podrían acceder a su información en Workfront Planning.

* ✅ Para aprovechar al máximo Workfront Planning, considere la posibilidad de reemplazar el uso de Portfolio y programas en el flujo de trabajo de Workfront por otra estructura de nivel superior en Workfront Planning.

  Hoy en día, los clientes de Workfront representan su trabajo estratégico a través de portafolios y programas, en algunos casos como proyectos de diferentes tipos. Con la introducción de Planning, todo este trabajo estratégico debe gestionarse a través de tipos de registros personalizados en Workfront Planning, mientras que Workfront se centrará en la fase de ejecución del trabajo representado como proyectos y tareas.


#### ¿Cuándo se debe crear un espacio de trabajo nuevo y cuándo se debe modificar uno existente?

* ✅ Diseño para el volumen más bajo de espacios de trabajo de nivel de organización. Puede crear espacios de trabajo para unidades de organización operativas específicas, de modo que coincidan con el modo exclusivo en que funciona cada unidad.

  Tener la información en una sola Workspace para garantizar que las relaciones entre todos los datos se puedan administrar fácilmente.

  Por ejemplo, intente crear un único espacio de trabajo para todo el departamento de marketing.

  Es aceptable crear un nuevo espacio de trabajo para un equipo que tenga una estructura operativa completamente diferente:

  Por ejemplo, un área de trabajo de **Desarrollo de producto** debe ser distinta de un área de trabajo de **Marketing**.

* ⛔ No cree espacios de trabajo únicos para cada equipo o proceso dentro de una organización.

  La organización de marketing debe esforzarse por mantener un solo espacio de trabajo para mantener la visibilidad y permitir que los datos se acumulen en el nivel de planificación global.

  Evite crear espacios de trabajo similares o duplicados para equipos que siguen procesos similares (por ejemplo, Marketing EMEA frente a Marketing APAC), especialmente donde estos equipos pueden trabajar que se acerquen a campañas estratégicas comunes.

#### ¿Cómo debo usar las secciones de Workspace?

* ✅ Cree y etiquete secciones para ayudar a los usuarios a comprender cómo organiza el ciclo de vida operativo.

  Por ejemplo, podría crear una sección llamada **Registros principales** en la que ubicaría sus campañas, tácticas y entregables en su área de trabajo.
* ✅ Agrupar los tipos de registros &quot;me gusta&quot;.

  Por ejemplo, podría crear una sección llamada **Geografías** que contenga tipos de registros como: Región, País y Ciudad.

### Tipos de registro

Los tipos de registro son los componentes básicos de un Workspace de Workfront Planning. Puede definir cómo se interconectan los tipos de registros.


#### ¿Cómo se deben definir los tipos de registros en el espacio de trabajo?

* ✅ Dedique algún tiempo a identificar qué información necesita rastrear (qué tipos de registros necesito) y cómo debe conectarse esta información. Hable con las partes interesadas que utilizarán el espacio de trabajo para tener en cuenta todas sus necesidades. También puede crear secciones personalizadas con diferentes tipos de registros para presentar la información de una manera muy consumible.


* ⛔ No duplique los tipos de registros para un período diferente (por ejemplo, no cree tipos de registros separados para **Campañas 2024** y **Campañas 2025**).

  La creación de diferentes tipos de registros interrumpe el flujo de datos, siempre que desee comparar datos de varios años. Las vistas de hoy son por tipo de registro, por lo que en cuanto termine el año, la vista de ese tipo de registro ya no mostrará los elementos futuros. La práctica recomendada es tener un tipo de registro para el tipo de trabajo y segmentar los datos mediante filtros o archivarlos, si es necesario.

#### ¿Cuándo se debe utilizar un campo de selección único o múltiple en lugar de un tipo de registro vinculado?

* ✅ Agregar un nuevo tipo de registro si el objeto se va a utilizar en conexión con varios tipos de registros más

  Por ejemplo, una campaña puede tener una conexión con varias audiencias de Target y una táctica puede tener una conexión con una sola audiencia de Target. Por lo tanto, Campaign, Tactic y Audience deben ser tipos de registro en lugar de campos de selección múltiple.

* ✅ Agregue un nuevo tipo de registro si el objeto necesita almacenar valores de metadatos adicionales que puedan ser útiles en las búsquedas

  Por ejemplo, un tipo de registro de canal como **Correo electrónico** puede almacenar una lista de entregables de soporte, ya sea como metadatos nativos o como conexión a un tipo de registro independiente **Entregables**.
* ⛔ No agregue un nuevo tipo de registro si los datos que está almacenando sólo son relevantes para un único tipo de registro.

  Por ejemplo, un tipo de registro **Campaign** puede tener un campo de selección único denominado **Tamaño de campaña**, que solo es relevante cuando se asocia directamente con una campaña específica.

#### ¿Cómo debo etiquetar mis tipos de registros?

* ✅ Cree y etiquete tipos de registros que representen una sola construcción o un solo sustantivo, como **Campañas**.
* ⛔ No cree un tipo de registro que se represente mejor como vista.

  Por ejemplo, **Calendario** es una mala opción para un tipo de registro, porque no es el tipo de registro en sí, sino una vista de registros.

### Administración de campos

Los campos son atributos de tipos de registro y se muestran como columnas en la vista de tabla. Puede crear campos personalizados para los tipos de registro y, a continuación, asociar los campos a los registros de Workfront Planning para mejorar la información de los registros.


#### ¿Qué campo se recomienda definir como campo principal?


* ✅ Utilice valores de campo principal únicos para que sea más fácil encontrar y &quot;seleccionar&quot; esos registros al realizar conexiones. 

  Al realizar una conexión, los usuarios buscarán por los valores del campo Principal y, si no son únicos, los usuarios no sabrán cuál elegir. 
* ⛔ Evite utilizar valores no únicos como campo principal porque puede crear confusión para los usuarios que deben buscar en el campo principal al utilizar el menú selector de conexiones. 

#### ¿Cómo debo usar las fórmulas?

* ✅ Utilice tipos de campo Fórmula para reducir la entrada manual. Cuando se introduce información basada en datos que ya están en la vista de tabla, es posible que se ahorre algún esfuerzo calculando esa información automáticamente mediante fórmulas.

#### ¿Cómo debo empezar a conectar los datos en mi espacio de trabajo?

* ✅ La creación de conexiones es una de las funciones más potentes de Workfront Planning. Puede conectar tipos de registros entre sí o con tipos de objetos de otras aplicaciones, como Adobe Workfront (conexión a proyectos, Portfolio, programas, compañías y grupos) y con Adobe Experience Manager Assets (conexión a recursos y carpetas).

  La conexión de tipos de objetos y registros proporciona una descripción general completa de cómo está conectado todo en su compañía.

  Por ejemplo, tiene un tipo de registro **Campaign**, y un tipo de registro **Tactics**, y puede crear una conexión entre estos dos tipos de registro para ver qué **Tactics** están asociadas a una **Campaign** específica.

  Después de definir la conexión, todas las personas del área de trabajo pueden empezar a agregar valores para **Campañas** haciendo doble clic en el campo de conexión, donde verán una lista de todas las **Tácticas** disponibles. Esto le permite encontrar rápidamente qué tácticas deben asociarse con sus campañas.

#### ¿Cómo se deben utilizar los campos de búsqueda?

* ✅ Después de establecer la conexión entre registros o tipos de objeto, puede conectar registros individuales entre sí y mostrar campos de los registros vinculados o tipos de objeto en un registro de Workfront Planning. Reducirá el número de lugares en los que tiene que actualizar la misma información y se asegurará de que coincidan perfectamente.

  Por ejemplo, una vez que tenga una conexión entre un tipo de registro **Campaign** y un tipo de registro **Tactics**, verá la información del campo principal, pero cuando agregue campos de búsqueda, podrá obtener información adicional de ese tipo de registro, como la **fecha de lanzamiento** para ese **Tactic**. Los datos de estos campos de búsqueda se rellenan automáticamente después de agregar los registros.

#### ¿Qué tipo de campo se recomienda para las direcciones URL? 

* ✅ Utilice un campo de texto de una sola línea para agregar datos de URL a un registro.

### Vistas

#### ¿Cómo puedo decidir qué debe ser una vista en lugar de un tipo de registro?

* ✅Para las cosas que representan una sola construcción o sustantivo (como **Campañas**), no cree un tipo de registro. 

* ⛔ No cree un tipo de registro que se represente mejor como vista.

  Por ejemplo, **Calendario** es una mala opción para un tipo de registro, porque no es el tipo de registro en sí, sino una vista de registros. 

#### ¿Debería ocultar o eliminar los campos que no son relevantes para mí?

* ✅ Oculte la columna en lugar de eliminarla cuando esta información pueda ser relevante para una persona diferente que utilice el mismo tipo de registro. Si elimina el campo en una vista de tabla específica, este campo también se eliminará en el resto de las vistas de este registro, así como en cualquier otro lugar desde el que esté vinculado este tipo de registro.

#### ¿Cómo debo usar los filtros y las agrupaciones en las vistas de tabla y cronología?

* ✅ Utilice vistas con filtros y agrupaciones para mostrar una instantánea de lo que necesita ver. Puede filtrar y agrupar los datos para tener una forma más legible de comprender lo que se ha planificado. Puede agrupar los registros por campos de metadatos.

  Por ejemplo, puede tener una vista de la cronología del tipo de registro **Campaign**, que puede agrupar por **Audiencias de destino** y filtrarla por **Fecha** para mostrar solo el año actual.

#### ¿Por qué no veo todos los registros en mi vista de cronología?

* ✅ Recuerde definir 2 campos de fecha para los registros. Solo puede crear una vista de escala de tiempo si tiene al menos dos campos de fecha asociados a un tipo de registro. Es posible que algunos registros no se muestren en la vista de escala de tiempo cuando las fechas de inicio o finalización no tienen valores y cuando la fecha de inicio es posterior a la fecha de finalización.

#### ¿Cómo debo usar la configuración de la vista de cronología?

* ✅ Defina la configuración de su vista de la cronología, como el **estilo de barra** y el **color**, para obtener una vista más enriquecedora. Puede personalizar el **estilo de barra** definiendo si desea ver una miniatura con una imagen significativa y agregar más campos para mostrar en la barra (por ejemplo, **Propietario** o **Estado**).

  De forma predeterminada, solo se ve el campo principal. También puede definir el color de la barra por valores de campo (por ejemplo, puede personalizar los colores de las barras haciendo coincidir con el campo Estado ) o por la agrupación aplicada. De forma predeterminada, el color coincide con el color del tipo de registro.

  Sólo los colores de tipo de registro o los campos con opciones asociadas a colores pueden afectar a los colores de las barras de registro de la escala de tiempo.

### Permisos y uso compartido

Utilice la función de uso compartido para otorgar los permisos adecuados a los empleados para acceder a las vistas y espacios de trabajo.

#### ¿Cómo debo administrar los permisos de los espacios de trabajo?

* ✅ Cuando crea un **espacio de trabajo**, solo está disponible para usted. Cualquier otra persona que no sea administrador del sistema no podrá encontrarla. Una vez definido el espacio de trabajo y listo para llevar a su equipo al inicio de la colaboración, debe compartirlo con ellos y definir su nivel de permisos.

  Puede elegir entre los siguientes niveles de permisos:

   * **Administrar**: Las personas pueden editar, eliminar y compartir el área de trabajo.
   * **Contribute**: las personas pueden crear, editar y eliminar registros.
   * **Ver**: Las personas pueden ver registros.

* ✅ Aunque muchos clientes sienten que concederían permisos de **Administrar** a los espacios de trabajo a la mayoría de las personas, no restrinja los permisos de **Administrar** a un grupo selecto de personas de confianza que no eliminarán accidentalmente un tipo de registro ni crearán campos y tipos de registros innecesarios. Pueden editar, compartir e incluso eliminar el espacio de trabajo. Este nivel de permisos les concede acceso administrativo completo a Workspace.

  Se requiere una licencia de usuario estándar para que alguien tenga permisos de administración en un espacio de trabajo.

* ✅ Conceda permisos a los usuarios de **Contribute** si solamente desea que puedan crear, editar y eliminar registros, pero no desea que cambien la estructura y el esquema del área de trabajo. Con los permisos de **Contribute**, no pueden crear tipos de registros ni cambiar los campos en los tipos de registros existentes.

  Se requiere una licencia de usuario estándar para que alguien tenga los permisos de **Contribute** en un espacio de trabajo.

* ✅ Asigne permisos a los usuarios **Ver**, si solamente desea que vean registros.

  >[!NOTE]
  >
  >En este momento, no tenemos permisos específicos para tipos de registros o registros, por lo que significa que todos los registros de cualquiera de los tipos de registros serán visibles si concede a alguien **Ver** acceso al área de trabajo.

#### ¿Cómo debo administrar los permisos de las vistas?

* ✅ Restringe los permisos de **Administrar** a las personas que deseas que puedan editar, eliminar y compartir la vista. Esto significa que pueden cambiar los filtros, los campos de agrupación o alguna configuración de la vista. Estos cambios afectarán a la configuración principal de la vista para todos los demás usuarios que también utilicen la vista.

  Se requiere una licencia de usuario estándar para que alguien tenga permisos de administración en una vista.

* ✅ Dé acceso a los usuarios **View** para que puedan aplicar la vista. Podrán cambiar algunos de los filtros, agrupaciones y ordenación, pero esos cambios serán solo temporales; los cambios no se guardan para todos los demás usuarios que accedan a la vista. Estos cambios no afectarán a la configuración principal de la vista para todos los demás usuarios que también utilicen la vista.  Sus cambios solo son visibles para el usuario que está aplicando la configuración modificada. Después de actualizar la pantalla, los cambios se restablecen al valor predeterminado.

* ✅ Dar a **Todos los usuarios del área de trabajo pueden ver** permisos cuando desee que todos los usuarios que puedan ver el área de trabajo vean los registros y sus campos en esa vista específica. De este modo, no es necesario agregar a nadie manualmente al cuadro de permisos de uso compartido de la vista.

  >[!NOTE]
  >
  >Si no se ha compartido una vista y comparte un vínculo con otras personas, podrán ver los registros en la **Vista de tabla predeterminada**. Si tiene una licencia estándar de Workfront, puede crear su propia vista.


#### ¿En qué se diferencia el uso compartido de **Workspace** del uso compartido de **vistas**?

* **Uso compartido de Workspace** define el acceso de las personas al espacio de trabajo, sus tipos de registros, registros y sus campos.

* **Compartir vistas** define si el usuario puede ver la vista que ha creado y si puede cambiar el filtro, los campos de agrupación o alguna otra configuración de la vista. La visibilidad de los registros mostrados en la vista está controlada por el uso compartido de Workspace y no por el uso compartido de Vista.

#### ¿Cómo afectan los tipos de licencia de Workfront a los permisos de Workfront Planning?

* Para **uso compartido de Workspace**: los usuarios con licencias Light y Contribute solo pueden obtener acceso de Ver a un espacio de trabajo. Para conceder a alguien permiso de Contribute o Administración a un espacio de trabajo, debe tener una licencia estándar.

* **Uso compartido de vistas**: Los usuarios con licencia estándar que tengan permisos de administración en un área de trabajo podrán crear una vista. Los usuarios con licencias Light y Contribute solo pueden utilizar las vistas que los usuarios de Standard han creado y compartido con ellos. De lo contrario, si no se ha compartido nada, los usuarios podrán ver la **Vista de tabla predeterminada**.


#### ¿Qué debo hacer cuando cambia el propietario de un Workspace?

* Workfront establece el creador del espacio de trabajo como propietario, pero en cuanto a la funcionalidad, el propietario tiene los mismos permisos que cualquier usuario con permisos de Administración.
* Si se desactiva el propietario, otros miembros podrán continuar su trabajo en el área de trabajo sin interrupciones.
* Los administradores del sistema tienen acceso a cualquier espacio de trabajo, por lo que si el propietario era la única persona con permisos de gestión, los administradores pueden agregar a otra persona y concederle permisos de gestión para gestionar la gestión del espacio de trabajo.

### Envío de solicitudes en Workfront Planning

Puede crear un formulario de solicitud para cada tipo de registro cuando desee que los usuarios agreguen registros fuera de la página de un tipo de registro. Al enviar el formulario, se agrega un nuevo registro al tipo de registro.

#### ¿Cuándo debería empezar a crear un formulario de solicitud para un tipo de registro?

* ✅ Debe asegurarse de que la estructura de tipo de registro se configura primero agregando los campos necesarios a la tabla. Estos campos describen los registros y se puede acceder a ellos desde el generador de formularios.

  Lo ideal es crear el formulario de solicitud o admisión después de finalizar la estructura de tipo de registro para evitar que falte ningún campo clave.

#### ¿Quién puede crear formularios de solicitud?

* ✅ Cualquier usuario con acceso de Administración al espacio de trabajo puede crear o editar un formulario de solicitud. Asegúrese de que los permisos del usuario estén asignados correctamente para permitir esta funcionalidad.

#### ¿Cómo se crea o edita un formulario de solicitud para un tipo de registro?

* ✅ Cualquier usuario con acceso de Administración al área de trabajo puede seguir los pasos descritos en el artículo [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### ¿Quién puede enviar nuevos registros utilizando el formulario de solicitud?

* ✅ Los permisos de envío dependen de la configuración configurada para cada formulario.

  En el generador de formularios, después de publicar el formulario, puede administrar permisos para controlar quién puede enviar solicitudes.

  Puede elegir entre las tres opciones de uso compartido siguientes:

   * **Cualquier persona con acceso de visualización o superior al área de trabajo:** Permite que todos los usuarios con permisos de visualización o superiores puedan enviar una solicitud para crear un registro.
   * **Cualquier persona con acceso al espacio de trabajo de tipo Contribution o superior**: Restringe los envíos a los usuarios con permisos de Contribute o superior para el espacio de trabajo.
   * **Cualquier persona con el vínculo:** Permite que cualquier persona que tenga el vínculo de formulario envíe una solicitud.
   * **Fecha de caducidad:** Asegúrese de establecer una fecha de caducidad para el vínculo público para mejorar la seguridad.

### Prácticas recomendadas para administrar formularios de solicitud

A continuación se indican algunas recomendaciones para administrar formularios de solicitud:

* Planificar con anticipación: defina claramente qué información se necesita o se requiere de los solicitantes antes de crear el formulario para evitar revisiones excesivas posteriormente.
* Usar etiquetas claras: Asegúrese de que las etiquetas de campo y las descripciones sean claras y comprensibles para todos los usuarios.
* Probar formularios: antes de desplegar nuevos formularios en una audiencia más amplia, pruébelos con el vínculo del formulario y la opción de previsualización de formulario para garantizar que todos los campos y la lógica funcionen según lo esperado.
* Mantener actualizados los formularios: revise periódicamente los formularios y actualícelos para que coincidan con cualquier cambio en la estructura de tipo de registro o en los procesos operativos.

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->