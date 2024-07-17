---
title: Conceder acceso a documentos
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los documentos de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Conceder acceso a documentos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los documentos, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Este acceso también se aplica a las carpetas de documentos.

Para obtener información acerca del uso de niveles de acceso personalizados para administrar el acceso de los usuarios a otros tipos de objetos en Workfront, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.&gt;.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar el acceso de los usuarios a los documentos mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Documentos y, a continuación, seleccione las capacidades que desea conceder en **Ajustar la configuración**.

   ![document_access.png](assets/document-access.png)

   Puede permitir que los usuarios hagan lo siguiente en los proyectos, tareas y problemas a los que tienen acceso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Crear</td> 
      <td>Cargar documentos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td> <p>Eliminar documentos cargados.</p> <p>La opción <b>Create</b> se habilita automáticamente cuando esta opción está habilitada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir</td> 
      <td>Comparta documentos con usuarios, funciones y equipos específicos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir documentos públicamente</td> 
      <td>Compartir documentos con usuarios externos (no tienen licencia de Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir en todo el sistema</td> 
      <td> <p>Poner los documentos a disposición de todos los usuarios de la instancia de Workfront.</p> <p>Cualquier persona del sistema puede ver un documento compartido de esta manera si:</p> 
       <ul> 
        <li> <p>Puede enviarles un vínculo a la página Documentos donde se ha cargado.</p> </li> 
        <li> <p>Lo buscan en Workfront</p> </li> 
       </ul> <p>La opción <b>Compartir</b> se habilita automáticamente cuando esta opción está habilitada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Cuando se establece una configuración de nivel de acceso para un tipo determinado de objeto, esa configuración no afecta al acceso de los usuarios a los objetos con una clasificación inferior. Por ejemplo, puede restringir la eliminación de proyectos en su nivel de acceso por parte de los usuarios, pero esto no les impide eliminar documentos, que son de menor clasificación que los proyectos. Para obtener más información sobre la jerarquía de objetos, vea la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Para restringir los permisos heredados para documentos de objetos de mayor clasificación, haga clic en **Establecer restricciones adicionales** y, a continuación, seleccione **No heredar nunca el acceso a documentos de proyectos, tareas, problemas, etc**.
1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a documentos por tipo de licencia

Para obtener más información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los documentos, vea la sección [Documentos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a documentos compartidos

Después de cargar un documento en Workfront, puedes compartirlo con otros usuarios concediéndoles permisos, como se explica en [Compartir un documento](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto
