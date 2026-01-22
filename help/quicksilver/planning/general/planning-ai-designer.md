---
title: Introducción a Adobe Workfront Planning Designer
description: Con Adobe Planning Designer, puede generar un nuevo espacio de trabajo, con tipos de registro y campos en Workfront Planning, agregar objetos a un espacio de trabajo o ver el historial de cambios en los registros.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 10%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Introducción a Adobe Workfront Planning Designer

{{planning-important-intro}}

Puede utilizar Adobe Planning Designer con tecnología de IA para generar un nuevo espacio de trabajo, agregar objetos a un espacio de trabajo (tipos de registro, registros, vistas o campos) o ver el historial de cambios en los registros.

>[!IMPORTANT]
>
>En este momento, Planning Designer solo está disponible para los usuarios que participan en el programa Cerrado de Beta.

Para obtener información sobre Workfront Planning, consulte los siguientes artículos:

* [Información general sobre Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Requisitos de acceso

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
<p>Cualquier paquete de Workfront y Planning</p>
<p>Cualquier paquete de flujo de trabajo y planificación</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inscripción en el programa Beta cerrado para Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

Actualmente, puede solicitar participar en el programa Beta cerrado para Planning Designer.

## Consideraciones sobre Planning Designer

* Para utilizar el Designer de Planning, su organización debe cumplir los requisitos para utilizar el asistente de IA de Workfront.

  Para obtener más información, consulte [Requisitos previos para el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Para utilizar Planning Designer, un administrador del sistema debe activarlo en el área Preferencias del sistema de la configuración.

* Puede utilizar indicadores para crear objetos de Planning mediante el Asistente de IA de Workfront desde el área de Planning o mediante el Designer de Planning.

* Las acciones que realiza el Asistente de IA en el área de Planning o las que realiza Planning Designer se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por Planning Designer en nombre del usuario se rastrean en el panel del historial del registro.

* Puede utilizar comandos para deshacer las acciones. Por ejemplo, puede escribir “Deshacer el último cambio” para revertir el cambio.

* Al crear, actualizar o eliminar un objeto a través de Planning Designer, muestra las acciones deseadas y solicita confirmación. A continuación, puede confirmar o cancelar las acciones.

* Cuando se crean espacios de trabajo y tipos de registros utilizando Planning Designer, las vistas y los campos también se crean automáticamente.

## Funcionalidad disponible actualmente para Planning Designer

Puede utilizar Planning Designer o el asistente de IA para realizar cualquiera de las siguientes acciones:

* Creación y configuración de espacios de trabajo

* Crear tipos de registro

* Campos de diseño o campos de fórmula

* Crear, eliminar, duplicar y restaurar registros

* Editar, actualizar y anexar un campo en un registro

* Vincular registros a otros registros

* Acceder a historial de cambios de registro

* Creación de vistas personalizadas

* Crear registros importando un documento.

  La creación de registros a partir de un documento importado sólo está disponible en Planning Designer y no en el asistente de IA.

  Para obtener información sobre los tipos y tamaños de archivo aceptados, consulte la sección &quot;Protecciones de documentos&quot; en el artículo [Usar el relleno de formulario con tecnología de IA para rellenar una solicitud mediante peticiones de datos o documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Habilitar Planning Designer para su organización

Como administrador de Workfront, primero debe habilitar Planning Designer para su organización.

<!--add steps here-->

1. Inicie sesión en Workfront como administrador del sistema.
1. Haga clic en **Menú principal** ![Icono del menú principal](assets/main-menu-shell.png) en la esquina superior izquierda de la pantalla y, a continuación, haga clic en **Configuración**.
1. Haga clic en **Sistema** > en el panel izquierdo y, a continuación, vaya al área de **preferencias de IA**.
1. Active la siguiente configuración:
   * **Habilitar IA**
   * **Adherirse a las beta de IA**
   * **Planificación de Designer**

   ![Configuración de Planning Designer en Preferencias del sistema](assets/planning-designer-toggle-in-system-preferences.png)
1. Haga clic en **Guardar**.

   Todos los usuarios del sistema que tengan una licencia Standard ahora pueden ver el botón **Diseñar con IA** en la página principal de Workspaces en el área de Planning. <!--check screen shot-->

   ![Diseño con botón de IA en la página de Workspace](assets/design-with-ai-button-on-workspaces-page.png)

   Ahora todos los usuarios pueden iniciar y utilizar Planning Designer para crear y actualizar objetos de Workfront Planning.

## Creación o actualización de objetos mediante Planning Designer

Puede crear o actualizar objetos en Workfront Planning mediante Planning Designer o el Asistente de IA, a menos que se especifique lo contrario.

1. Inicie sesión en Workfront y, a continuación, haga clic en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda.

1. Haga clic en **Planificación**. Se abre el área de Planning.

1. Haga clic en **Diseñar con IA**.

   Se abre la ventana **Planning Designer**.

   ![Ventana de Planning Designer](assets/planning-designer-window.png)

1. En el espacio proporcionado, empiece a escribir comandos para el asistente de IA y, a continuación, haga clic en Intro cuando haya terminado.

   <!--add screen shot-->

   Por ejemplo, puede escribir una solicitud similar a las siguientes:

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

   Puede revisar espacios de trabajo, tipos de registros, campos, vistas y registros en el área de vista previa a la derecha del mensaje.
1. (Opcional) Escriba peticiones de datos adicionales para editar más los objetos.
1. (Opcional) Haga clic en el icono **Alternar la pantalla de vista previa de AI Workspace** ![Ocultar o mostrar el icono de la pantalla de vista previa](assets/hide-show-preview-screen-in-planning-designer.png) para abrir o cerrar la pantalla de vista previa a la derecha.
1. Haga clic en el icono **Abrir espacio de trabajo en ficha nueva** ![Abrir espacio de trabajo en ficha nueva](assets/open-workspace-on-new-tab-icon.png) para abrir el espacio de trabajo que está actualizando en una ficha nueva.
1. Haga clic en el icono **Cerrar** **X** para cerrar Planning Designer y abrir el área de Workspaces.
1. Abra el espacio de trabajo editado con Planning Designer y realice más cambios en sus objetos.




