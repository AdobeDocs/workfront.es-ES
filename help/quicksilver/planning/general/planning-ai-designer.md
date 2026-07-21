---
title: Introducción a Adobe Workfront Planning Designer
description: Puede utilizar Adobe Planning Designer con tecnología de IA para configurar sus espacios de trabajo y estructuras de datos con facilidad. Planning Designer admite desde la creación y configuración de espacios de trabajo hasta la definición de campos y fórmulas, la administración de registros, la revisión del historial de cambios y la creación de vistas personalizadas. Ya sea que se utilice directamente o a través del Asistente de IA, Planning Designer proporciona un entorno flexible y potente para crear y mantener información estructurada y conectada.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YZRzcl8ymUo85jplCgKOx-qI83Gqa4CUI6saxfijtec
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e8216d44973c43f14ef615a6f8c4eb1cb05bd935
workflow-type: tm+mt
source-wordcount: 1496
ht-degree: 7%

---

# Introducción a Adobe Workfront Planning Designer

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer está disponible actualmente para todos los clientes con un estado de Beta.
>
>La información de este artículo hace referencia a Adobe Workfront Planning, una funcionalidad adicional de Adobe Workfront.
>
>Para obtener una lista de los requisitos para acceder a Workfront Planning, consulte [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Para obtener información general sobre Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Puede utilizar Adobe Planning Designer con tecnología de IA para configurar sus espacios de trabajo y estructuras de datos con facilidad. Planning Designer admite desde la creación y configuración de espacios de trabajo hasta la definición de campos y fórmulas, la administración de registros, la revisión del historial de cambios y la creación de vistas personalizadas.

Ya sea que se utilice directamente o a través del Asistente de IA, Planning Designer proporciona un entorno flexible y potente para crear y mantener información estructurada y conectada.

Para obtener información sobre Workfront Planning, consulte los siguientes artículos:

* [Índice general de información y artículos para Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Información general de acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Requisitos de acceso <!--edit theses??-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de Workfront o de flujo de trabajo con un paquete de Planning</p>
<p>Cualquier Planning como paquete de producto independiente</p>
   </td> </tr>
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Workfront</p></td> 
   <td><p>Estándar</p> 
   <p>Los administradores de Workfront deben habilitar Planning Designer para su organización</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación</p></td> 
   <td><p>Estándar</p> 
   <p>Los administradores de Workfront deben habilitar Planning Designer para su organización</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilite Planning Designer para su organización

Como administrador del sistema, puede activar Planning Designer Beta para su organización. Después de activar esta configuración, todos los usuarios de la instancia de Workfront podrán ver las capacidades de Planning Designer en el área de Planning.

1. Inicie sesión como administrador de Workfront.
1. Haga clic en el **icono del menú principal** ![Menú principal](assets/main-menu-shell.png) y, a continuación, haga clic en **Configurar**.
1. Vaya a **Sistema** > **Preferencias** > **Preferencias de IA**.
1. Activar **Habilitar IA**.

   >[!NOTE]
   >
   >No es necesario aceptar el contrato de IA para utilizar Planning Designer en la versión beta.

1. Active la configuración **Adherirse a las beta de IA** si no está habilitada.
1. Active la configuración **Planning Designer** si no está habilitada.

   ![Configuración de Planning Designer en Preferencias del sistema](assets/ai-preferences-with-planning-designer-unaccepted-agreement.png).

   >[!TIP]
   >
   >Las opciones **Opt-in to AI Beta** y **Planning Designer** están activadas de forma predeterminada, pero debe aceptar el acuerdo de Beta para poder usar Planning Designer.

1. (Condicional y obligatorio) Si no ha aceptado el Contrato de Beta, haga clic en **Revisar el Contrato de Beta** y lea el contrato; a continuación, haga clic en **Aceptar**.

1. Haga clic en **Guardar**.

   Las funcionalidades de Planning Designer para crear o editar espacios de trabajo ya están disponibles para todos los usuarios de su organización que pueden acceder a Planning.

<!--

## Turn off the Planing Designer for your organization

After your Workfront administrator accepts the AI Assistant agreement, the Planning Designer is turned on for everyone in your organization, by default. 

To turn it off: 

1. Log in to Workfront as a System Administrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn off the **Planning Onboarding** setting.
1. Click **Save**.

    This removes the Planning Designer for all users in the system.

-->

<!--

## Enroll in the Closed Beta program for the Planning Designer

Currently, you can request to participate in the Closed Beta program for the Planning Designer by sending us an email to sargism@adobe.com.

After we receive the email, our Engineering team will turn on the Planning Designer in your Workfront instance. 

>[!IMPORTANT]
>
>Your company must first accept the AI Assistant agreement before the Planning Designer is available in your system. 

-->

## Enviar comentarios sobre Planning Designer

Puede enviar comentarios sobre Planning Designer durante el programa beta.

1. Inicie sesión en Workfront, luego haga clic en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **Planificación**.

   Se abre el área **Planificación**.

1. Haga clic en **Crear con IA**. <!--update this tag name when they change it-->

   Se abre la ventana **Planning Designer**.

1. Haga clic **Enviar comentarios aquí** en la parte inferior de la página.
1. Agregue sus comentarios en el espacio proporcionado y haga clic en **Enviar**.
Los comentarios se envían a los equipos de ingeniería y producto.

## Consideraciones sobre Planning Designer

* No es necesario habilitar el acuerdo de IA para poder acceder a Planning Designer.

* Debe firmar el acuerdo de Beta para acceder a Planning Designer.

<!--
Sargis and Ashot  said these are not required: 

* To use the Planning Designer, you first need to enable AI for your organization. The following must be in place for the AI features to be available to everyone in your organization:

    * Workfront must make the AI features available for your organization.

        For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
    * After Workfront makes the AI features available for your organization, the main Workfront administrator can access it. 

        For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md). 
    * The Workfront administrator must accept the Gen AI agreement, and then turn on AI and the Planning Designer for your organization. 

        For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md). 

-->

* El administrador de Workfront debe activar Planning Designer para su organización. Después de esto, Planning Designer está disponible para todos los usuarios de forma predeterminada.
* Si su organización ha firmado un acuerdo de IA, las acciones realizadas por Planning Designer también las puede realizar el asistente de IA cuando lo utilice en el área de Planning.
* Las acciones que realiza el Asistente de IA en el área de Planning o las que realiza Planning Designer se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront.

  Para obtener más información, consulte los siguientes artículos:

  * [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por el asistente de IA o por Planning Designer en nombre del usuario se rastrean en el panel del historial del registro.

* Las acciones realizadas por el Designer de Planificación son permanentes y podrían ser irreversibles. Por ejemplo, no se puede deshacer la eliminación de un campo. Revise todas las acciones propuestas por Designer antes de aceptarlas.

  >[!IMPORTANT]
  >
  >Al crear, actualizar o eliminar un objeto a través de Planning Designer, el mensaje solicitará confirmación solo para las acciones que son irreversibles. Por ejemplo, la eliminación de un tipo de registro o de un espacio de trabajo es irreversible. No se puede eliminar un registro. Planning Designer solo solicitará confirmación cuando intente eliminar un tipo de registro o espacio de trabajo.

* Cuando se crean espacios de trabajo y tipos de registros utilizando Planning Designer, las vistas y los campos también se crean automáticamente.

## Funcionalidad disponible actualmente para Planning Designer

Puede utilizar Planning Designer o el asistente de IA para realizar cualquiera de las siguientes acciones:

* Creación y configuración de espacios de trabajo

* Editar espacios de trabajo

* Crear tipos de registros, incluida la definición y adición de tipos de registros globales a espacios de trabajo

* Campos de diseño o campos de fórmula

* Crear, eliminar, duplicar y restaurar registros

* Editar, actualizar y anexar un campo en un registro

* Vincular registros a otros registros

* Acceder a historial de cambios de registro

* Creación de vistas personalizadas

* Creación de registros importando un documento

  Por ejemplo, puede cargar una imagen de un organigrama en su empresa y Planning Designer puede crear un espacio de trabajo basado en ella.

  La creación de objetos a partir de un documento importado sólo está disponible en Planning Designer y no en el asistente de IA.

  >[!IMPORTANT]
  >
  >Aunque se admiten los tipos de archivo .XLSX, no se pueden utilizar para la importación de registros a gran escala mediante Planning Designer.
  >Si necesita importar un número considerable de registros en este momento, le recomendamos que lo haga mediante las funciones manuales disponibles en Planning.
  >
  >Para obtener más información, vea [Crear registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Para ver las limitaciones de tipo de archivo, consulte la sección &quot;Obtener sugerencias basadas en un documento que haya cargado&quot; en [Usar el relleno de formulario con tecnología de IA para rellenar una solicitud mediante peticiones de datos o documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Creación o actualización de objetos mediante Planning Designer

Puede crear o actualizar objetos en Workfront Planning mediante Planning Designer o el Asistente de IA, a menos que se especifique lo contrario.

1. Inicie sesión en Workfront, luego haga clic en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **Planificación**.

   Se abre el área **Planificación**. <!--update screen shot when they change the name of the button-->

   ![Crear con el botón IA en la página Espacios de trabajo](assets/design-with-ai-button-on-workspaces-page.png)

1. Haga clic en **Crear con IA** o haga clic en **Crear espacio de trabajo** y, a continuación, utilice la ventana de solicitud de la parte superior para indicar qué tipo de espacio de trabajo desea crear. <!--update this when they change it to Generate with AI-->

   Se abre la ventana **Planning Designer**. <!--remove the Beta tag here when this removes from Beta-->

   ![Ventana de Planning Designer](assets/planning-designer-window.png)

1. En el espacio proporcionado, empiece a escribir las solicitudes del Ayudante de IA y, cuando termine, haga clic en Entrar.

   <!--add screen shot-->

   Por ejemplo, puede escribir mensajes similares a los siguientes:

   * Cree y configure un espacio de trabajo con cinco tipos de registros para administrar campañas

   * Cree campañas de marketing para cada mes del año actual

   * Agregue un campo de campaña para Estado para el área de trabajo Diseño de marketing

   * Eliminar todos los registros de un estado de obsoleto

   * Actualizar todas las campañas de Planning a un estado de Activo

   * Conectar campañas a personas en el espacio de trabajo de diseño de marketing

   * Mostrar el historial de cambios de la campaña &quot;San Valentín&quot;

   * Crear una vista de cronología para las campañas en el área de trabajo Diseño de marketing

   * Crear registros importando un documento. La creación de registros a partir de un documento importado sólo está disponible en Planning Designer y no en el asistente de IA.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Después de recibir una respuesta correcta, siga los vínculos proporcionados en el área de solicitud para crear, actualizar o revisar el objeto de la solicitud.

   Cuando acepte crear los objetos, los cambios se mostrarán a la derecha del área de solicitud.

   Puede ver espacios de trabajo, tipos de registros, campos, vistas y registros en el área de vista previa a la derecha del mensaje.

   >[!TIP]
   >
   >Algunos objetos se crean inmediatamente, sin necesidad de confirmación.

1. (Opcional) Escriba peticiones de datos adicionales para editar más los objetos.
1. (Opcional) Haga clic en el icono **Mostrar u ocultar pantalla de vista previa** ![Ocultar o mostrar icono de pantalla de vista previa](assets/hide-show-preview-screen-in-planning-designer.png) para abrir o cerrar la pantalla de vista previa a la derecha.
1. Haga clic en el icono **Abrir espacio de trabajo en ficha nueva** ![Abrir espacio de trabajo en ficha nueva](assets/open-workspace-on-new-tab-icon.png) para abrir el espacio de trabajo que está actualizando en una ficha nueva.
1. Haga clic en el icono **Cerrar** **X** para cerrar Planning Designer y abrir el área de Workspaces.
1. (Opcional) Para editar un espacio de trabajo, siga uno de estos procedimientos:

   * Abra el espacio de trabajo y realice cambios manualmente en él. Para obtener más información, consulte [Edición de espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).
   * Abra el área de trabajo y haga clic en **Editar con IA**. Se abrirá Planning Designer. Repita los pasos anteriores para utilizar IA y realizar más cambios en el espacio de trabajo.


