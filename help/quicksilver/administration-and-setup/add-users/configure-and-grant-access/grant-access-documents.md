---
title: Concesión de acceso a documentos
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los documentos en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Concesión de acceso a documentos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los documentos, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Este acceso también se aplica a carpetas de documentos.

Para obtener información sobre el uso de niveles de acceso personalizados para administrar el acceso de los usuarios a otros tipos de objetos en Workfront, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Debe ser administrador de Workfront.&gt;.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuración del acceso de los usuarios a los documentos mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono del engranaje ![](assets/gear-icon-settings.png) en el **Ver** o **Editar** a la derecha de Documentos y, a continuación, seleccione las capacidades que desea conceder en **Ajustar la configuración**.

   ![document_access.png](assets/document-access.png)

   Puede permitir que los usuarios hagan lo siguiente en proyectos, tareas y problemas a los que tengan acceso:

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
      <td> <p>Elimine los documentos cargados.</p> <p>La variable <b>Crear</b> se activa automáticamente cuando esta opción está activada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir</td> 
      <td>Comparta documentos con usuarios específicos, funciones de trabajo y equipos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir documentos públicamente</td> 
      <td>Comparta documentos con usuarios externos (no tenga una licencia de Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir en todo el sistema</td> 
      <td> <p>Ponga los documentos a disposición de todos los usuarios de la instancia de Workfront.</p> <p>Cualquier usuario del sistema puede ver un documento compartido de esta manera si:</p> 
       <ul> 
        <li> <p>Les envía un enlace a la página Documentos donde se carga.</p> </li> 
        <li> <p>Lo buscan en Workfront</p> </li> 
       </ul> <p>La variable <b>Compartir</b> se activa automáticamente cuando esta opción está activada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Al configurar un nivel de acceso para un determinado tipo de objeto, esa configuración no afecta al acceso de los usuarios a los objetos con una clasificación inferior. Por ejemplo, puede restringir el acceso de los usuarios para que no eliminen proyectos en su nivel de acceso, pero esto no les impide eliminar documentos, que tienen una clasificación inferior a la de los proyectos. Para obtener más información sobre la jerarquía de objetos, consulte la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Para restringir los permisos heredados de documentos de objetos de clasificación superior, haga clic en **Establecer restricciones adicionales** y, a continuación, seleccione **Nunca heredar el acceso a los documentos de proyectos, tareas, problemas, etc.**.
1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a los documentos por tipo de licencia

Para obtener más información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los documentos, consulte la sección [Documentos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a documentos compartidos

Después de cargar un documento en Workfront, puede compartirlo con otros usuarios concediéndoles permisos, tal como se explica en [Compartir un documento](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario están determinados por una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* La configuración del nivel de acceso del destinatario para el tipo del objeto
