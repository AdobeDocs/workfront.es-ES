---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar campos de fecha personalizados en un informe de calendario
description: Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede utilizar campos de fecha personalizados en un informe de calendario para tareas, problemas y proyectos.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# Usar campos de fecha personalizados en un informe de calendario

A [!UICONTROL calendario] es un informe dinámico que proporciona una representación visual del trabajo. Puede utilizar campos de fecha personalizados en un informe de calendario para los siguientes objetos:

* Tareas
* Problemas
* Proyectos

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Editar] acceso a [!UICONTROL Informes], [!UICONTROL Tableros] y [!UICONTROL Calendarios]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al informe de calendario</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

1. Debe tener campos de fecha personalizados y un valor dentro del campo disponible en el [!DNL Workfront] instancia. Si no tiene un formulario personalizado configurado con fechas personalizadas, siga las instrucciones de las dos primeras secciones de [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Adjunte el formulario personalizado a un proyecto, tarea o problema que planee agregar al calendario, y especifique una fecha. Para obtener más información, consulte [Adición de un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Configuración del grupo de elementos

Puede elegir cómo desea que se muestre el grupo de elementos en el calendario.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Calendarios]**.

1. Seleccione el calendario al que desee agregar un nuevo grupo de elementos.\
   O\
   Haga clic en **[!UICONTROL + Nuevo calendario]** e introduzca el nombre del calendario.

   >[!NOTE]
   >
   >Debe tener [!UICONTROL Editar] acceso a [!UICONTROL Informes], [!UICONTROL Tableros]y [!UICONTROL Calendarios] en el nivel de acceso para crear un informe de calendario.

1. A la izquierda, haga clic en **[!UICONTROL Agregar al calendario]** y haga clic en **[!UICONTROL Agregar elementos avanzados]**.

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Asigne un nombre a este grupo de elementos]</strong></td>
      <td>Escriba un nombre para el grupo de elementos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Seleccione un color para el grupo de elementos. Todos los elementos se muestran en el color seleccionado en el informe de calendario.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campo de fecha]</strong></td>
      <td>Choose <strong>[!UICONTROL Fechas personalizadas]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL En el calendario, mostrar]</strong></td>
      <td><p>Elija cómo desea que se muestren las fechas:</p>
       <ul>
        <li><strong>[!UICONTROL Fecha única]</strong>: El calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL Duration] (de inicio a fin)</strong>: El calendario muestra el objeto durante un intervalo de días.<br><p>Nota: Si elige <strong>[!UICONTROL Duración]</strong>, la fecha de finalización especificada debe ser posterior a la fecha de inicio o el elemento no se mostrará en el calendario.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Fechas personalizadas]</strong></td>
      <td><p>Introduzca el nombre de fecha personalizado adjunto al objeto que desea rastrear.</p></td>
     </tr>
    </tbody>
   </table>

1. Continúe con la siguiente sección.

## Agregar objetos al grupo de elementos

Después de configurar cómo desea que se muestren los elementos, debe agregar los objetos que desee ver en el calendario a la agrupación.

1. En el **[!UICONTROL ¿Qué desea agregar al calendario?]** , seleccione

   * **[!UICONTROL Tareas]**
   * **[!UICONTROL Proyectos]**
   * **[!UICONTROL Problemas]**

1. Haga clic en **[!UICONTROL Agregar tareas]**, **[!UICONTROL Agregar proyectos]** o **[!UICONTROL Agregar problemas]**, según el tipo de objeto que agregue al calendario.\
   ![Seleccionar objeto para calendario](assets/field-name.png)

1. En el menú desplegable, empiece a escribir el nombre del campo y, a continuación, seleccione el origen del campo del objeto que desea mostrar en el calendario (por ejemplo, **[!UICONTROL Tareas atrasadas]**).
1. Defina una condición para la agrupación de calendario.

   ![Condición](assets/condition-statement-calendar.png)

   Para obtener más información sobre la configuración de condiciones, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionales para la agrupación del calendario repitiendo los pasos del 1 al 4.
1. En el **[!UICONTROL Establezca las etiquetas Tareas/Proyectos/Problemas para que sean...]** , seleccione cómo se etiquetan en el calendario los objetos de esta agrupación de calendario.

   >[!NOTE]
   >
   >Si las opciones de etiqueta predeterminadas no están disponibles para un objeto determinado, se mostrará el nombre del objeto en su lugar. Por ejemplo, cuando la variable [!UICONTROL Tarea principal] la etiqueta está seleccionada y no hay ninguna tarea principal asociada al objeto, [!DNL Adobe Workfront] muestra el nombre del objeto que está viendo en el calendario.

1. Haga clic en **[!UICONTROL Guardar]**.
