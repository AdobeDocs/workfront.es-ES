---
product-area: enterprise-scenario-planner-product-area
keywords: plan,permisos,compartir,iniciativas,escenarios,escenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Compartir un plan en el planificador de escenarios
description: Puede compartir un plan que haya creado en el Planificador de escenarios de Adobe Workfront con otros usuarios.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 86%

---

# Compartir un plan en el [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Puede compartir un plan en [!DNL Adobe Workfront Scenario Planner] con otros usuarios para que puedan colaborar en el mismo trabajo que usted realiza.

>[!TIP]
>
>Si envía un vínculo a un plan a otras personas, también debe compartir el plan con ellas para que puedan verlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquete</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Hable con su representante de Workfront si tiene un paquete de Workfront diferente.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Light] o superior</p> 
   <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
    <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el acceso al Scenario Planner, consulte [Acceso necesario para usar el [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Para obtener información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

* Los usuarios a los que se han concedido permisos para el plan deben tener acceso al área [!DNL Scenario Planner] en sus niveles de acceso, tal como ha concedido el administrador de [!DNL Workfront], para poder recibir permisos para un plan.

  Por ejemplo, los [!UICONTROL solicitantes] no pueden ver, crear ni editar planes. Debe tener esto en cuenta al compartir un plan con un usuario que tenga una licencia de solicitante.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Para obtener más información sobre el acceso a [!DNL Scenario Planner] para varios tipos de licencia, consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Consideraciones sobre el uso compartido de un plan

* Todos los usuarios, incluidos los administradores del sistema, solo tienen acceso a los planes que han creado.
* Puede compartir un solo plan o varios planes en lote.
* No puede ver los planes que no ha creado o que no se han compartido con usted.
* Solo puede compartir un plan con otros usuarios. No puede compartir las metas con grupos, equipos o compañías. 
* Debe guardar el plan para poder compartirlo.
* Puede compartir una dirección URL de un plan con otro usuario. Si el usuario no tiene permisos para ver al menos el plan, puede solicitar acceso al plan a otro usuario cuando reciba la dirección URL. Para obtener información sobre cómo solicitar acceso a un plan, consulte [Solicitar permisos para un plan en [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Cuando comparte varios planes que ya se han compartido con otros, los usuarios con los que comparte no sustituyen a los existentes, sino que se añaden a ellos en cada plan seleccionado.

## Opciones de permiso de un plan

En la tabla siguiente se enumeran los permisos que puede conceder al compartir un plan. Para obtener más información sobre el acceso que obtienen los usuarios según su licencia, consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Acciones</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
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
   <td>Ver funciones</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ver información de coste y presupuesto*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Administración de la información de costes y presupuestos*</td> 
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
   <td>Publicar escenarios**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Debe tener acceso a los datos financieros para poder ver o administrar la información financiera de los planes, incluso si tiene permisos de administración de planes. Para obtener información sobre el acceso a los datos financieros, consulte [Conceder acceso a los datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Debe tener acceso para crear y permisos para administrar proyectos para poder publicar escenarios.

Para obtener información acerca del nivel de acceso al proyecto, consulte [Conceder acceso a proyectos](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información acerca de los permisos del proyecto, consulte [Compartir un proyecto en [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Compartir planes

{{step1-to-scenario-planner}}

1. Haga clic en el nombre de un plan para abrirlo.

   O

   Seleccione varios planes para compartirlos en lote.

   >[!TIP]
   >
   >Puede compartir un plan haciendo clic en los avatares de los usuarios con los que comparte el plan en la esquina superior derecha del encabezado del plan.

1. (Condicional) Si ha abierto un plan, haga clic en el icono **[!UICONTROL Más]** ![Más icono](assets/more-icon.png) a la derecha del nombre de [!UICONTROL Plan] y, a continuación, haga clic en **[!UICONTROL Compartir]**

   O

   Si seleccionó varios planes para compartirlos en lotes, haga clic en el icono **[!UICONTROL Compartir]** ![Compartir icono](assets/share-icon-26x26.png) que se encuentra en la parte superior de la lista de planes para abrir el cuadro de acceso de [!UICONTROL Plan].

   >[!TIP]
   >
   >* Los usuarios que tienen permisos para todos los planes que seleccione se mostrarán en la casilla de acceso al [!UICONTROL Plan].
   >* Los usuarios adicionales se añaden a y no reemplazan a los usuarios existentes en todos los planes seleccionados.

1. En el campo **[!UICONTROL Dar acceso al plan a]**, empiece a escribir el nombre de los usuarios con los que desea compartir el plan y, a continuación, selecciónelos cuando aparezcan en la lista.
1. En el menú desplegable de permisos que aparece a la derecha del nombre de usuario, seleccione el nivel de permiso que desea concederle al plan.
1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Los usuarios con los que comparta el plan tendrán permisos para ver el plan. No pueden editar información sobre el plan, añadir iniciativas, escenarios o publicar escenarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>Los usuarios con los que comparte el plan tienen permisos para administrar el plan, lo que incluye editar información, añadir iniciativas y escenarios, y publicar el plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Solamente puede eliminarse un plan cuando este ya se ha creado. No puede eliminar planes que se hayan compartido con usted.

1. Haga clic en **[!UICONTROL Guardar]**.

   El plan ahora se comparte con los usuarios especificados.

   Puede ver los usuarios que tienen permisos sobre el plan en la columna Compartido conmigo en una lista de planes o en la esquina superior derecha del encabezado del plan.

   >[!TIP]
   >
   >Puede ver los planes que se comparten con usted aplicando el filtro [!UICONTROL Compartido conmigo] en una lista de planes.


