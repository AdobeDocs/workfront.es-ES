---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incrustar una página web externa en un panel de control
description: Puede incrustar una página web externa en un panel de control para proporcionar acceso a información relacionada de otros sistemas dentro de Adobe Workfront o a otras páginas de Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 87%

---

# Incrustar una página web externa en un panel de control

<!--Audited: 01/2025-->

Puede incrustar una página web externa en un panel de control para proporcionar acceso a información relacionada desde otros sistemas o desde Adobe Workfront.

Por ejemplo, si su organización tiene un repositorio de documentos basado en web, una wiki u otro sistema de administración de contenido que contenga información del proyecto a la que se accede regularmente a través de una dirección URL, puede mostrar esa información en Workfront creando una página externa en un panel de control.

>[!IMPORTANT]
>
>* Por motivos de seguridad, algunos sitios web no permiten incrustar páginas web como un iframe. Si la página web que desea incrustar en un panel de control no lo permite, la página no se mostrará en dicho panel. Sin embargo, aún puede acceder a la página externa haciendo clic en el nombre del panel de control.\
>![Informe de página externa vacío](assets/qs-empty-external-page-report-350x165.png)\
>Para permitir la incrustación en un sitio web de su propiedad, trabaje con el administrador web para configurar **X-Frame-Options**. Para obtener más información, consulte [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* Las páginas de panel de control ya no se admiten como páginas externas incrustadas en los paneles de control. Aunque los tableros existentes no se modificarán automáticamente para eliminar estas páginas externas, cualquier modificación en un panel de control que incluya una referencia de este tipo no podrá guardarse hasta que se elimine o cambie la referencia.
>  > En concreto, los subdominios Workfront.com que ya no se admiten son los siguientes:
>
>     * /dashboards
>     * /dashboard/:ID&#x200B;
>     * /portfolio/:ID/content-dashboard__:dashboardID&#x200B;
>     * /program/:ID/content-dashboard__:dashboardID&#x200B;
>     * /project/:ID/content-dashboard__:dashboardID&#x200B;
>     * /task/:ID/content-dashboard__:dashboardID&#x200B;
>     * /template/:ID/content-dashboard__:dashboardID&#x200B;
>     * /templatetask/:ID/content-dashboard__:dashboardID&#x200B;
>     * /resourcemanagement/:ID/
>     * content-dashboard__:dashboardID&#x200B;
>     * /team/:ID/content-dashboard__:dashboardID&#x200B;
>     * /iteration/:ID/content-dashboard__:dashboardID&#x200B;
>     * /requests/:ID/content-dashboard__:dashboardID&#x200B;
>     * /group/:ID/content-dashboard__:dashboardID&#x200B;
>     * /billingrecord/:ID/content-dashboard__:dashboardID
>
>Como solución alternativa, considere la posibilidad de incluir un informe de lista en su panel de control como se explica en [Añadir un informe a un panel de control](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso al panel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Requisitos previos

Debe crear un panel de control para poder incrustar una página externa en él.

Para obtener más información sobre cómo crear paneles de control, consulte [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incrustar una página externa en un panel de control

>[!IMPORTANT]
>
>Puede quitar una página externa de un panel de control si ya no es necesaria. Sin embargo, no es posible eliminar una página externa una vez creada en Workfront. Solamente puede eliminarsse una página externa mediante la API. Para obtener más información, consulte [Quitar una página externa de un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Busque la URL de la página que se mostrará en Workfront y copie la URL ubicada en la barra de direcciones.

   >[!NOTE]
   >
   >Si comparte URL con objetos de Workfront, recuerde que algunas caducan con el paso del tiempo. Por ejemplo, las URL de documentos caducan después de abrirse. Se configura como una medida de seguridad e, intencionadamente, se consideran URL no estáticas y no deben compartirse.

{{step1-to-dashboards}}

1. Para editar un panel de control existente, seleccione el panel en el que desea incrustar la página del sitio web, haga clic en **Acciones de panel de control** y, a continuación, haga clic en **Editar**
O\
   Para crear un nuevo panel de control, haga clic en **Nuevo panel de control**.\
   Para obtener más información sobre cómo crear un panel de control, consulte [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Haga clic en **Agregar página externa** en el área **Seleccionar diseño / Agregar informes / Agregar calendarios**.

   ![Agregar página externa](assets/qs-add-external-page-350x239.png)

   Se muestra el cuadro **Agregar página externa**.

1. Especifique la siguiente información sobre la página externa:

   * **Nombre**: agregue un nombre para el panel de control.
   * **Descripción**: agregue más información sobre el panel de control para identificar la información que contiene. La descripción se muestra en el panel de control para todas las personas que tengan acceso a él después de que la guarde.
   * **URL**: pegue la URL que copió anteriormente en este campo.

     Puede especificar los siguientes tipos de URL:

      * Una URL https (cifrada) a una página web.\
        Solo las páginas https (cifradas) se cargan con la URL.\
        ![Agregar cuadro de diálogo de página externa](assets/add-external-page-dialog-qs-350x247.png)

      * Una URL de plantilla que contiene información de la sesión de un sitio web específico.\
        Por ejemplo: *https://localhost/?session={!$$SESSION}*
Debe haber iniciado sesión en el sitio web especificado para visualizar la página externa.\
        Para obtener información sobre cómo obtener un SessionID de Workfront, consulte [Conceptos básicos sobre las API](../../../wf-api/general/api-basics.md).\
        El administrador de Workfront puede configurar las preferencias del sistema de forma que no permita el uso de información de sesión en las páginas externas por motivos de seguridad. En este caso, la página externa no se carga en el panel de control.\
        Para obtener más información acerca de las preferencias de seguridad del sistema, consulte [Configurar las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
        ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

     >[!WARNING]
     >
     >El uso de SessionID no es seguro y no se recomienda.
     >

   * **Altura**: introduzca un número mayor que 0 para definir el espacio que ocupa la página externa en el panel de control. La altura predeterminada es 500.

1. Haga clic en **Guardar**.

   La página se agrega automáticamente al panel de control.

   Si crea paneles de control adicionales, puede buscar esta página externa y agregarla a otros paneles de control. Puede encontrar todas las páginas externas existentes en la lista de Informes y calendarios disponibles al crear o editar un panel de control.

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## Actualización de una página externa en un panel de control

Para actualizar la información de una página externa utilizada en un panel de control:

{{step1-to-dashboards}}

1. Haga clic en el nombre del panel de control que desea actualizar para abrirlo, haga clic en **Acciones de panel de control** y, a continuación, en **Editar**.

   Se abre el cuadro **Detalles de panel de control**.

1. En el área **Seleccionar diseño / Agregar informes** del cuadro **Detalles del panel**, busque la página externa que desee actualizar, pase el ratón sobre ella y haga clic en el icono **Editar**.\
   ![Página externa de edición en línea](assets/nwe-inline-edit-external-page-350x226.png)

1. En el cuadro **Editar página externa**, actualice los campos que desee cambiar y, a continuación, haga clic en **Guardar**.
1. (Opcional) Haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png) para eliminar la página externa del panel. Para obtener más información, consulte [Quitar una página externa de un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Haga clic en **Guardar + Cerrar**.

## Ver páginas externas en un informe

Puede ver todas las páginas externas de Workfront en un informe de páginas externas.

{{step1-to-reports}}

1. Haga clic en **Nuevo informe** > seleccione **Sección externa**.

   ![Sección externa](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Opcional) Actualice las pestañas Ver, Filtros o Agrupaciones del informe.

   Para obtener más información, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Haga clic en **Guardar + Cerrar**.

   Puede ver el nombre y la dirección URL asociada con cualquier página externa del sistema en el nuevo informe.

