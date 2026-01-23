---
title: Introducción a Adobe Workfront Planning Designer
description: Con Adobe Planning Designer, puede generar un nuevo espacio de trabajo, con tipos de registro y campos en Workfront Planning, agregar objetos a un espacio de trabajo o ver el historial de cambios en los registros.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bd3dde54d986416af847b2f3b2a1e8570d5ce3f2
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 6%

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

En la actualidad, puede solicitar participar en el programa Cerrado de Beta para Planning Designer enviándonos un correo electrónico a sargism@adobe.com.

Después de recibir el correo electrónico, nuestro equipo de ingeniería activará Planning Designer en su instancia de Workfront.

>[!IMPORTANT]
>
>En primer lugar, su empresa debe aceptar el contrato de asistente de IA antes de que Planning Designer esté disponible en el sistema.

## Consideraciones sobre Planning Designer

* Para utilizar Planning Designer, primero debe activar el asistente de IA para su organización. Debe establecerse lo siguiente para que el asistente de IA esté disponible para todos los miembros de la organización:

   * Workfront debe poner el asistente de IA a disposición de su organización.

     Para obtener más información, consulte [Requisitos previos para el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
   * Una vez que Workfront pone el asistente de IA a disposición de su organización, el administrador principal de Workfront puede acceder a él.

     Para obtener más información, consulte [Configurar información básica para el sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).
   * El administrador de Workfront debe aceptar el acuerdo del asistente de IA y, a continuación, activar el asistente de IA para todos los demás usuarios.

     Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).
* Una vez que el administrador del sistema ha activado el asistente de IA para su organización, el asistente de planificación está disponible para todos los usuarios, de forma predeterminada, si se ha puesto a disposición de su organización.
* Las acciones que realiza Planning Designer también las puede realizar el Asistente de IA cuando se utiliza en el área de Planning.
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
  >Aunque se admiten los tipos de archivo .XLSX y .CSV, no se pueden utilizar para la importación de registros a gran escala mediante Planning Designer.
  >Si necesita importar un número considerable de registros en este momento, le recomendamos que lo haga mediante las funciones manuales disponibles en Planning.
  >
  >Para obtener más información, vea [Crear registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Para ver las limitaciones de tipo de archivo, consulte la sección &quot;Obtener sugerencias basadas en un documento que haya cargado&quot; en [Usar el relleno de formulario con tecnología de IA para rellenar una solicitud mediante peticiones de datos o documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Creación o actualización de objetos mediante Planning Designer

Puede crear o actualizar objetos en Workfront Planning mediante Planning Designer o el Asistente de IA, a menos que se especifique lo contrario.

1. Inicie sesión en Workfront, luego haga clic en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **Planificación**.

   Se abre el área **Planificación**.

   ![Diseñar con el botón de IA en la página Espacios de trabajo](assets/design-with-ai-button-on-workspaces-page.png)

1. Haga clic en **Diseñar con IA**.

   Se abre la ventana **Planning Designer**.

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
1. Abra el espacio de trabajo editado con Planning Designer y realice más cambios en sus objetos.

## Desactive Planning Designer para su organización

Una vez que el administrador de Workfront acepta el acuerdo del Asistente de IA, Planning Designer se activa para todos los miembros de la organización de forma predeterminada.

Para desactivarla:

1. Inicie sesión en Workfront como administrador del sistema.
1. Haga clic en **Menú principal** ![Icono del menú principal](assets/main-menu-shell.png) en la esquina superior izquierda de la pantalla y, a continuación, haga clic en **Configuración**.
1. Haga clic en **Sistema** > en el panel izquierdo y, a continuación, vaya al área de **preferencias de IA**.
1. Desactive la configuración de **Planning Designer**. <!--add new screen shot with info icon-->

   ![Configuración de Planning Designer en Preferencias del sistema](assets/planning-designer-toggle-in-system-preferences.png)
1. Haga clic en **Guardar**.

   Esto elimina Planning Designer para todos los usuarios del sistema.






