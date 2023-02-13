---
product-area: enterprise-scenario-planner-product-area
keywords: plan,permisos,compartir,iniciativas,escenarios,escenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Compartir un plan en el planificador de escenarios
description: Puede compartir un plan que haya creado en Adobe Workfront Scenario Planner con otros usuarios.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# Compartir un plan en [!DNL Scenario Planner]

Puede compartir un plan en la [!DNL Adobe Workfront Scenario Planner] con otros usuarios, para que puedan colaborar en el mismo trabajo que usted.

>[!TIP]
>
>Si envía un enlace a un plan a otros, también debe compartir el plan con ellos para que puedan verlo.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de [!UICONTROL Edit] a la variable [!DNL Scenario Planner]</p> <p>Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p> Permisos de [!UICONTROL Administrar] para el plan
     <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Acceso a [!UICONTROL Request] a un plan en la variable [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

* Los usuarios a los que se hayan otorgado permisos para el plan deben tener acceso al [!DNL Scenario Planner] en sus niveles de acceso, tal como le haya concedido su [!DNL Workfront] administrador, para recibir permisos para un plan.

   Por ejemplo, [!UICONTROL Solicitantes] no pueden ver, crear ni editar planes. Debe tener esto en cuenta al compartir un plan con un usuario que tenga una licencia de Solicitante.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Para obtener más información sobre el acceso a la variable [!DNL Scenario Planner] para varios tipos de licencia, consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Consideraciones sobre el uso compartido de planes

* Puede compartir un solo plan o varios planes de forma masiva.
* No puede ver los planes que no ha creado o que no se han compartido con usted.
* Solo puede compartir un plan con otros usuarios. No puede compartir planes con grupos, equipos o empresas.
* Primero debe guardar un plan para poder compartirlo.
* Puede compartir una URL con un plan con otro usuario. Si el usuario no tiene permisos para ver al menos el plan, puede solicitar acceso al plan a otro usuario cuando reciba la dirección URL. Para obtener información sobre cómo solicitar acceso a un plan, consulte [Solicitar acceso a un plan en la [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Al compartir varios planes que ya se han compartido con otros usuarios, los usuarios que comparta con no se reemplazan, sino que se agregan a los usuarios existentes en cada plan seleccionado.

## Compartir planes

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **[!UICONTROL Situaciones]**.
1. Haga clic en el nombre de un plan para abrirlo

   O

   Seleccione varios planes para compartirlos de forma masiva.

   >[!TIP]
   >
   >Puede compartir un plan haciendo clic en los avatares de los usuarios con los que se comparte el plan en la esquina superior derecha del encabezado del plan.

1. (Condicional) Si ha abierto un plan, haga clic en el **[!UICONTROL Más]** icono ![](assets/more-icon.png) a la derecha del [!UICONTROL Plan] nombre y haga clic en **[!UICONTROL Compartir]**

   O

   Si ha seleccionado varios planes para compartirlos de forma masiva, haga clic en el botón **[!UICONTROL Compartir]** icono ![](assets/share-icon-26x26.png) en la parte superior de la lista de planes para abrir [!UICONTROL Plan] de acceso.

   >[!TIP]
   >
   >* Los usuarios que tengan permisos para todos los planes que seleccione se mostrarán en la [!UICONTROL Plan] de acceso.
   >* Los usuarios adicionales se añaden a y no reemplazan a los usuarios existentes en todos los planes seleccionados.


1. En el **[!UICONTROL Proporcionar acceso al plan para]** , empiece a escribir el nombre de los usuarios con los que desea compartir el plan y, a continuación, selecciónelos cuando aparezcan en la lista.
1. En el menú desplegable de permisos situado a la derecha del nombre de usuario, seleccione el nivel de permiso que desea conceder al plan.
1. Seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Los usuarios con los que comparta el plan tendrán permisos para verlo. No pueden editar información sobre el plan, agregar iniciativas, escenarios ni publicar escenarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Administrar]</td> 
      <td> <p>Los usuarios con los que comparta el plan tienen permisos para administrarlo, lo que incluye editar información, agregar iniciativas, escenarios y publicar el plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sólo puede eliminar un plan cuando lo haya creado. No puede eliminar planes que se hayan compartido con usted.

1. Haga clic en **[!UICONTROL Guardar]**.

   El plan ahora se comparte con los usuarios especificados.

   Puede ver los usuarios que tienen permisos para el plan en la columna Compartido conmigo de una lista de planes o en la esquina superior derecha del encabezado del plan.

   >[!TIP]
   >
   >Puede ver los planes que se han compartido con usted aplicando la variable [!UICONTROL Compartido conmigo] filtrar en una lista de planes.

## Opciones de permiso del plan

En la tabla siguiente se enumeran los permisos que puede conceder al compartir un plan. Para obtener más información sobre el acceso que los usuarios obtienen en función de su licencia, consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Acciones</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Administrar]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ver plan </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ver iniciativas </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Ver escenarios</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Ver funciones de trabajo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ver información de costo y presupuesto*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Administrar información de costo y presupuesto*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Crear iniciativas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Crear escenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar iniciativas o escenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copiar escenarios</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Situaciones de publicación**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Debe tener acceso a los Datos financieros para poder ver o administrar la información financiera de los planes, incluso si tiene permisos de gestión para los planes. Para obtener información sobre el acceso a los datos financieros, consulte [Concesión de acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Debe tener acceso a crear y permisos para administrar proyectos para poder publicar escenarios.

Para obtener información sobre el nivel de acceso al proyecto, consulte [Concesión de acceso a proyectos](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información sobre los permisos del proyecto, consulte [Compartir un proyecto en [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
