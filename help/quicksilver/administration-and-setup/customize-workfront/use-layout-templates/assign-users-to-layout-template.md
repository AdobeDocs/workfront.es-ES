---
title: Asignar usuarios a una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede asignar una plantilla de diseño que haya creado a cualquier usuario, función de trabajo, equipo o grupo que necesite utilizarla.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Asignar usuarios a una plantilla de diseño

Puede asignar una plantilla de diseño que haya creado a cualquier usuario, rol, equipo o grupo que necesite utilizarla.

Para los usuarios que no tienen asignada una plantilla de diseño, se utiliza el diseño predeterminado. Para obtener más información sobre el diseño predeterminado, consulte [Acerca del diseño predeterminado de Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Los usuarios también pueden asignarse una plantilla de diseño, tal como se describe en las áreas Cambiar el trabajo y Solicitudes de trabajo con plantillas de diseño.

Puede asignar varias plantillas de diseño diferentes al mismo nombre. Para obtener más información sobre qué plantilla de diseño está en vigor para un usuario, rol, grupo o equipo, consulte [Prioridad de asignación de plantilla de diseño](#layout-template-assignment-priority) más adelante en este artículo.

Para obtener más información sobre las plantillas de diseño, consulte [Plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Asignar una plantilla de diseño a los usuarios

1. Empiece a trabajar en una plantilla de diseño como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Cuando esté satisfecho con la plantilla de diseño, le recomendamos que la pruebe, tal como se describe en [Prueba de una nueva plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Clic **Asignar esto a** en la sección superior de la página.
1. En el cuadro que aparece, haga clic en **Agregar un usuario, un rol, un equipo o un grupo**, empiece a escribir el nombre de un usuario, función de trabajo, equipo o grupo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Los nombres añadidos recientemente se muestran con un fondo azul. Esto resulta útil cuando está editando una plantilla de diseño existente porque puede distinguir los nombres que acaba de agregar de los que ya estaban en la lista.

   Un icono de información ![](assets/info-icon.png) se muestra a la derecha del nombre de cualquier usuario, rol, equipo o grupo que ya esté asignado a otra plantilla de diseño. Puede situarse sobre el icono para ver el nombre de esa plantilla de diseño y decidir si desea anular la asignación existente.

1. Repita los dos pasos anteriores para asignar la plantilla de diseño a otros usuarios, roles, equipos o grupos según sea necesario.

   Puede asignar hasta 100 usuarios a la vez.

1. Clic **Listo**, luego haga clic en **Guardar** en la esquina inferior izquierda.

   Este paso completa el proceso de creación y asignación de una plantilla de diseño.

## Prioridad de asignación de plantilla de diseño {#layout-template-assignment-priority}

Usted y otros administradores de Workfront pueden asignar varias plantillas de diseño diferentes al mismo usuario de las cuatro formas siguientes:

* Para el usuario individual
* A un rol particular que el usuario tiene
* Para un equipo determinado el usuario está en
* Para un grupo determinado en el que se encuentra el usuario

Sin embargo, solo una plantilla de diseño es visible para el usuario en un momento determinado. La plantilla visible viene determinada por la siguiente jerarquía de prioridades:

* **Usuario individual**: la plantilla de diseño asignada a la persona como usuario individual anula todas las demás. Puede anular una asignación anterior realizada para un usuario individual realizando una nueva asignación; la más reciente tiene prioridad.
* **Rol principal**: Si la persona no tiene asignada una plantilla de diseño como usuario único, verá la plantilla asignada para su rol de trabajo principal.

  El usuario solo puede ver la plantilla de diseño asignada a la función de trabajo principal de un usuario. Las plantillas asignadas a cualquier puesto secundario que tenga el usuario no son visibles.

* **Equipo de inicio**: Si la persona no tiene asignada una plantilla de diseño como usuario individual, ni como usuario con una función de trabajo principal, verá la plantilla asignada a su equipo de inicio.

  Solo la plantilla asignada al equipo de inicio de un usuario es visible para el usuario. Las plantillas asignadas a otros equipos en los que un usuario es miembro no son visibles.

* **Grupo de inicio**: si a la persona no se le asigna una plantilla de diseño como usuario individual, como usuario con un rol de trabajo principal o como miembro de un equipo de inicio, verá la plantilla asignada a su grupo de inicio.

  El usuario solo puede ver la plantilla asignada al grupo de inicio de un usuario. Las plantillas asignadas a cualquiera de sus otros grupos no son visibles.

## Gran cantidad de usuarios asignados a una plantilla de diseño

Si edita una plantilla de diseño asignada a más de 2000 usuarios y realiza cambios en la misma, solo se conservarán los 2000 primeros usuarios en la plantilla y verán los cambios que ha realizado. La plantilla de diseño se elimina de todas las demás.

Si tiene más de 2000 usuarios para asignar a una plantilla de diseño, le recomendamos que realice una de las siguientes acciones:

* Organice los usuarios en grupos o equipos y asigne la plantilla de diseño a esos grupos o equipos. Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Creación y administración de equipos](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Asigne funciones a los usuarios y asigne la plantilla de diseño a su función de trabajo principal. Para obtener más información, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
