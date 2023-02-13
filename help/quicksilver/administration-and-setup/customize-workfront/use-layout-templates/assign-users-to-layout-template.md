---
title: Asignar usuarios a una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede asignar una plantilla de diseño que haya creado a cualquier usuario, función de trabajo, equipo o grupo que necesite utilizarla.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Asignar usuarios a una plantilla de diseño

Puede asignar una plantilla de diseño que haya creado a cualquier usuario, función de trabajo, equipo o grupo que necesite utilizarla.

Para los usuarios que no tienen una plantilla de diseño asignada, se utiliza el diseño predeterminado. Para obtener más información sobre el diseño predeterminado, consulte [Acerca del diseño predeterminado de Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Los usuarios también pueden asignarse una plantilla de diseño a sí mismos, tal como se describe en Cambiar las áreas Mi trabajo y Solicitudes de trabajo con plantillas de diseño.

Puede asignar varias plantillas de diseño diferentes al mismo nombre. Para obtener más información sobre qué plantilla de diseño está en vigor para un usuario, función, grupo o equipo, consulte [Prioridad de asignación de plantilla de diseño](#layout-template-assignment-priority) más adelante en este artículo.

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
   <td> <p>Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso del administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de dicho grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Asignar una plantilla de diseño a los usuarios

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Cuando esté satisfecho con la plantilla de diseño, le recomendamos que la pruebe, tal como se describe en [Prueba de una nueva plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Haga clic en **Asigne esto a** en la sección superior de la página.
1. En el cuadro que aparece, haga clic en **Agregar un usuario, función de trabajo, equipo o grupo**, empiece a escribir el nombre de un usuario, función de trabajo, equipo o grupo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   Los nombres agregados recientemente se muestran con un fondo azul. Esto resulta útil cuando edita una plantilla de diseño existente, ya que puede distinguir los nombres que acaba de agregar de los que ya estaban en la lista.

   Un icono de información ![](assets/info-icon.png) se muestra a la derecha del nombre de cualquier usuario, función de trabajo, equipo o grupo que ya esté asignado a otra plantilla de diseño. Puede situarse sobre el icono para ver el nombre de esa plantilla de diseño y decidir si desea anular la asignación existente.

1. Repita los dos pasos anteriores para asignar la plantilla de diseño a otros usuarios, funciones de trabajo, equipos o grupos según sea necesario.

   Puede asignar hasta 100 usuarios a la vez.

1. Haga clic en **Listo** y haga clic en **Guardar** en la esquina inferior izquierda.

   Este paso completa el proceso de creación y asignación de una plantilla de diseño.

## Prioridad de asignación de plantilla de diseño {#layout-template-assignment-priority}

Usted y otros administradores de Workfront pueden asignar varias plantillas de diseño diferentes al mismo usuario de estas cuatro formas diferentes:

* Al usuario individual
* Para una función de trabajo determinada que el usuario tiene
* Para un equipo determinado, el usuario se encuentra en
* Para un grupo determinado, el usuario se encuentra en

Sin embargo, el usuario solo puede ver una plantilla de diseño en un momento dado. La plantilla visible está determinada por la siguiente jerarquía de prioridad:

* **Usuario individual**: La plantilla de diseño asignada a la persona como usuario individual anula a todos los demás. Puede anular una asignación anterior realizada para un usuario individual realizando una nueva asignación; el más reciente tiene prioridad.
* **Función de trabajo principal**: Si a la persona no se le asigna una plantilla de diseño como un solo usuario, verá la plantilla asignada para su función de trabajo principal.

   El usuario solo puede ver la plantilla de diseño asignada a la función de trabajo principal de un usuario. Las plantillas asignadas a cualquier función de trabajo secundaria que tenga el usuario no están visibles.

* **Equipo principal**: Si a la persona no se le asigna una plantilla de diseño como usuario individual, ni como usuario con una función de trabajo principal, verá la plantilla asignada a su equipo de inicio.

   El usuario solo puede ver la plantilla asignada al equipo de inicio de un usuario. Las plantillas asignadas a otros equipos en los que el usuario es miembro no están visibles.

* **Grupo de inicio**: Si a la persona no se le asigna una plantilla de diseño como usuario individual, como usuario con una función de trabajo principal o como miembro de un equipo de Inicio, verá la plantilla asignada a su grupo de Inicio.

   El usuario solo puede ver la plantilla asignada al grupo Inicio de un usuario. Las plantillas asignadas a cualquiera de sus otros grupos no están visibles.

## Gran número de usuarios asignados a una plantilla de diseño

Si edita una plantilla de diseño asignada a más de 2000 usuarios y realiza cambios, solo los primeros 2000 usuarios se mantendrán en la plantilla de diseño y verán los cambios realizados. La plantilla de diseño se elimina de todas las demás.

Si tiene más de 2000 usuarios para asignar a una plantilla de diseño, le recomendamos que realice una de las siguientes acciones:

* Organice a los usuarios en grupos o equipos y asigne la plantilla de diseño a esos grupos o equipos. Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Crear y administrar equipos](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Asigne funciones de trabajo a los usuarios y asigne la plantilla de diseño a su función de trabajo principal. Para obtener más información, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
