---
title: Concesión de acceso a proyectos
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los proyectos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e47f5d06d0c7d72c171583b53b69f951e4e99afe
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Concesión de acceso a proyectos

<!-- Audited: 12/2023 -->

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los proyectos, como se explica en los siguientes artículos:
* [Información general sobre niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [Información general sobre nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
 <p>o</p> 
<p>Actual: plan </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar el acceso de los usuarios a los proyectos mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el **Ver** o **Editar** a la derecha de Proyectos y, a continuación, seleccione las capacidades que desea conceder en **Ajuste la configuración**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Los usuarios con una licencia de trabajo tienen derechos limitados sobre el proyecto. Pueden contribuir a un proyecto, pero no administrarlo.
   >* Los usuarios con una licencia de revisión tienen derechos de visualización en los proyectos de problemas convertidos, pero sus derechos de visualización son limitados.
   >* Para obtener información sobre los permisos que los usuarios pueden conceder al compartir proyectos con otros usuarios, consulte [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Cuando se establece una configuración de nivel de acceso para un tipo determinado de objeto, esa configuración no afecta al acceso de los usuarios a los objetos con una clasificación inferior. Por ejemplo, puede restringir la eliminación de proyectos en su nivel de acceso por parte de los usuarios, pero esto no les impide eliminar tareas, que son de menor clasificación que los proyectos. Para obtener más información sobre la jerarquía de objetos, vea la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Haga clic en **establecer valores predeterminados de uso compartido** a la derecha de la opción Crear, luego **Agregar regla** para agregar una regla de uso compartido para nuevos proyectos.

   Cuando el usuario con este nivel de acceso crea un proyecto, este se comparte automáticamente con los usuarios seleccionados en el menú de la izquierda.

   ![](assets/project-sharing-menu.png)

   En el menú de la derecha, especifique cómo desea que se comparta el proyecto con esos usuarios:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Si un usuario con este nivel de acceso utiliza una plantilla de acceso al proyecto, la plantilla anula la configuración de uso compartido en el nivel de acceso. Para obtener información sobre las plantillas de acceso a proyectos, consulte [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   Puede repetir este paso para agregar tantas reglas de uso compartido de proyectos como necesite para el nivel de acceso.

1. Haga clic en la X para cerrar **Ajuste la configuración** cuadro.
1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas del nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a informes, tableros y calendarios por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, consulte la sección [Proyectos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a proyectos compartidos

Como propietario o creador de un problema, puede compartirlo con otros usuarios otorgándoles permisos, tal como se explica en [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto
