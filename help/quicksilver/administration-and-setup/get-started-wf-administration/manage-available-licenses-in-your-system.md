---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Administre las licencias disponibles en su sistema
description: Como administrador de Adobe Workfront, puede acceder a información sobre su cuenta de Workfront, incluido el número de licencias adquiridas para su organización, así como el número de licencias actualmente en uso.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: a39720a4529dcd974483f7730b6feb4d6cd6f994
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# Administre las licencias disponibles en su sistema

Como administrador de Adobe Workfront, puede acceder a información sobre su cuenta de Workfront, incluido el número de licencias adquiridas para su organización, así como el número de licencias actualmente en uso.

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
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ver las licencias de su organización

El número de licencias usadas se actualiza automáticamente al asignar niveles de acceso a los usuarios que agregue a Workfront. Para obtener más información, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para ver la información de licencia en su sistema:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En la parte inferior del panel izquierdo, haga clic en **Sistema** > **Licencias**.

   Para obtener más información sobre las licencias enumeradas en esta página, consulte [Información general sobre licencias heredadas](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Las licencias de prueba solo están disponibles para los clientes que hayan comprado el complemento de prueba de Workfront de pago además de su licencia de Workfront. Para obtener información sobre este complemento, consulte [Prueba de Workfront](../../workfront-proof/workfront-proof.md).

1. (Condicional) Si ve el mensaje **Para establecer un máximo, debe agregar un grupo de inicio**, agregue grupos principales en el sistema como se explica en la sección [Agregar o quitar un grupo de inicio a la página Licencias](#add-or-remove-a-home-group-to-the-licenses-page) en este artículo.

## Ver información sobre licencias para complementos de Workfront

En la captura de pantalla siguiente, **5 de 10 licencias de prueba** indica que esta organización tiene el complemento de pago Workfront Proof y que actualmente está utilizando 5 de las 10 licencias de Workfront Proof que compró.

![](assets/updated-licenses-page.png)

Si su organización ha comprado Workfront Goal, la información de licencia de este producto también se muestra aquí. En este caso, puede ver la siguiente información:

* El número total de licencias de objetivos de Workfront que su empresa ha adquirido
* Número de licencias de objetivos de Workfront asociadas a los usuarios. Este es el número de usuarios a los que se ha concedido al menos Ver acceso a los Objetivos en su nivel de acceso.

Para obtener información sobre los objetivos de Workfront, consulte [Información general sobre los objetivos de Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Para obtener información sobre el acceso a los objetivos de Workfront, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront le permite asignar más licencias de objetivos de Workfront que haya adquirido. Sin embargo, cuando asigne más licencias de las que permite el contrato de objetivos de Workfront, un administrador de cuentas de Workfront se pondrá en contacto con usted para informarle de que ha superado su número contractual.

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Los usuarios sin acceso administrativo pueden utilizar un informe de grupo para ver el recuento de licencias. En la pestaña Informe , cree un nuevo informe de grupo y agregue las columnas siguientes:>
>* Límite de tipo de licencia: Límite de trabajo
>* Límite de tipo de licencia: Límite del planificador
>
>Para obtener más información sobre la creación de informes, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ver información sobre pruebas mensuales y habilitaciones de decisión de documentos

Las pruebas y las decisiones documentales están limitadas para todas las licencias de Workfront no pagadas. Los límites se restablecen por usuario cada mes.

>[!IMPORTANT]
>
>Los límites de pruebas y decisiones de documentos no se aplican a los usuarios en [licencias heredadas de Workfront y niveles de acceso](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Los límites de decisión para cada licencia difieren según el plan en el que esté. Puede consultar la asignación mensual en Configuración > Licencias.

Para obtener más información sobre los límites de pruebas y decisiones de documentos, consulte [Información general sobre la resolución limitada de documentos y pruebas para usuarios no pagados](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![](assets/monthly-decision-allotment.png)

## Agregar o quitar un grupo de inicio a la página Licencias {#add-or-remove-a-home-group-to-the-licenses-page}

Se requiere un plan de Business o Enterprise Workfront para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront.](https://www.workfront.com/plans)

Cada usuario puede asignarse a un solo grupo de inicio. Workfront proporciona un recuento de licencias con orientación de grupo calculando cuántas licencias se asignan y se utilizan actualmente en cada grupo de inicio.

Si ve el mensaje **Para establecer un máximo, debe agregar un grupo de inicio** en la página Licencias , debe agregar al menos un grupo de inicio a la página Licencias .

>[!IMPORTANT]
>
>* Para administrar de forma eficaz las licencias con grupos principales, se recomienda configurar grupos principales específicos para unidades empresariales antes de actualizar el recuento máximo de licencias. Para obtener más información, consulte [Información general sobre los grupos de inicio](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Solo se pueden agregar grupos de nivel superior como grupos de inicio, no como subgrupos. Si un usuario tiene un subgrupo asignado como grupo principal, su licencia se agrega al recuento de licencias del grupo de nivel superior situado encima de ese subgrupo.
>


Para agregar o quitar un grupo de inicio a la página Licencias:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En la parte inferior del panel izquierdo, haga clic en **Sistema** > **Licencias**.

1. Haga clic en **Administrar lista de grupos**.
1. Empiece a escribir el nombre del grupo de nivel superior en la **Grupos de inicio** en la ventana
1. Para agregar el grupo, haga clic en su nombre cuando aparezca.

   O

   Para quitar el grupo, haga clic en el icono X a la derecha de su nombre.

1. Haga clic en **Guardar**.

Como administrador de Workfront, puede establecer recuentos máximos de licencias para los grupos principales para evitar que una unidad empresarial use las licencias de Workfront adquiridas para otras unidades de negocio. Para obtener instrucciones, consulte [Establezca el número máximo de licencias para un grupo en el hogar](#set-the-maximum-license-count-for-a-home-group) en este artículo.

## Establezca el número máximo de licencias para un grupo en el hogar {#set-the-maximum-license-count-for-a-home-group}

Como administrador de Workfront, puede configurar recuentos máximos de licencias para los grupos principales de su sistema. Esto le permite evitar que una unidad empresarial utilice las licencias de Workfront adquiridas para otras unidades empresariales de su organización.

De forma predeterminada, el recuento máximo de licencias está establecido en N/A, lo que significa que no hay límite.

Los administradores de grupo pueden ver el número de licencias asignadas y utilizadas en un grupo de inicio que administran. Para obtener más información, consulte [Ver el número de licencias asignadas y utilizadas en un grupo en la nueva experiencia de Adobe Workfront](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Para establecer el recuento máximo de licencias para un grupo en el hogar:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En la parte inferior del panel izquierdo, haga clic en **Sistema** > **Licencias**.

1. Busque el grupo de inicio en la lista.
1. En el **Max** del grupo, haga clic en el valor para el que desee establecer un máximo.
1. Escriba el número máximo y pulse Intro.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Para volver a establecer el valor máximo de licencia de un grupo en el valor predeterminado, no escriba 0. En su lugar, elimine el número en el cuadro . Si establece el valor máximo de la licencia en 0, se indicará que no hay licencias asignadas a ese grupo.
