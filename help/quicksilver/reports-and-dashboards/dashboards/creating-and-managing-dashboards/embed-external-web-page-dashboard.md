---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incrustar una página web externa en un panel
description: Puede incrustar una página web externa en un tablero para proporcionar acceso a la información relacionada de otros sistemas de Adobe Workfront o de otras páginas de Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: a8a3aec50b5538de5867ce3ba7723d92c046b50d
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Incrustar una página web externa en un panel

Puede incrustar una página web externa en un tablero para proporcionar acceso a la información relacionada de otros sistemas de Adobe Workfront o de otras páginas de Workfront.

Por ejemplo, si su organización tiene un repositorio de documentos basado en la web, wiki u otro sistema de administración de contenido que contenga información del proyecto a la que se accede regularmente a través de una dirección URL, puede mostrar esa información en Workfront creando una página externa en un panel.

>[!IMPORTANT]
>
>Por motivos de seguridad, algunos sitios web no permiten incrustar páginas web como iframe. Si la página web que desea incrustar en un tablero no lo permite, la página no se muestra en el tablero. Sin embargo, aún puede acceder a la página externa haciendo clic en el nombre del tablero.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Para permitir la incrustación de un sitio web propio, trabaje con el administrador web para ajustar la variable **X-Frame-Options** configuración. Para obtener más información, consulte [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>Las páginas de tablero ya no se admiten como páginas externas incorporadas en tableros. En concreto, los siguientes subdominios de Workfront.com ya no son compatibles:
>
>* /&#x200B; de tableros
>* /dashboard/:&#x200B; de ID
>* /portafolio/:ID/content-dashboard__:&#x200B; de ID de panel
>* /program/:ID/content-dashboard__:dashboardID &#x200B;
>* /project/:ID/content-dashboard__:dashboardID &#x200B;
>* /task/:ID/content-dashboard__:dashboardID &#x200B;
>* /template/:ID/content-dashboard__:dashboardID &#x200B;
>* /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>* /resourcemanagement/:ID/content-dashboard__:&#x200B; de ID de panel
>* /team/:ID/content-dashboard__:dashboardID &#x200B;
>* /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>* /request/:ID/content-dashboard__:dashboardID &#x200B;
>* /group/:ID/content-dashboard__:dashboardID &#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en el tablero</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear un tablero para poder incrustar una página externa en él.

Para obtener información sobre la creación de tableros, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incrustar una página externa en un tablero

>[!IMPORTANT]
>
>Puede eliminar una página externa de un tablero si ya no la necesita. Sin embargo, no puede eliminar una página externa después de haberla creado en Workfront. Solo puede eliminar una página externa mediante la API. Para obtener más información, consulte [Eliminar una página externa de un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Busque la dirección URL de la página para mostrarla en Workfront y copie la dirección URL ubicada en la barra de direcciones.

   >[!NOTE]
   >
   >Si comparte direcciones URL con objetos de Workfront, recuerde que algunas direcciones URL caducan con el tiempo. Por ejemplo, las direcciones URL del documento caducan después de abrirse. Esto se configura como una medida de seguridad y por diseño se consideran direcciones URL no estáticas y no se deben compartir.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Tableros**.

1. Para editar un tablero existente, seleccione el tablero en el que desea incrustar la página del sitio web y, a continuación, haga clic en **Acciones del panel** y seleccione **Editar** del menú .\
   O\
   Para crear un tablero nuevo, haga clic en **Nuevo tablero**.\
   Para obtener más información sobre cómo crear un tablero, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Haga clic en **Agregar página externa**.

   ![](assets/qs-add-external-page-350x239.png)

1. Especifique un **Nombre** para la página externa .
1. Especifique un **Descripción**.
1. Pegue la dirección URL que ha copiado anteriormente en el **URL** campo .\
   Puede especificar los siguientes tipos de direcciones URL:

   * Una URL (cifrada) https a una página web.\
      Solo las páginas https (cifradas) se cargan con la dirección URL.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * Una URL de plantilla que contiene información de sesión de un sitio web específico.\
      Por ejemplo: *https://localhost/?session={!$$SESSION}*
Debe iniciar sesión en el sitio web especificado para mostrar la Página externa.\
      Para obtener información sobre cómo obtener un SessionID de Workfront, consulte [Conceptos básicos de API](../../../wf-api/general/api-basics.md).\
      El administrador de Workfront puede configurar las preferencias del sistema de forma que no permita el uso de la información de sesión en las páginas externas por motivos de seguridad. En este caso, la página externa no se carga en el panel.\
      Para obtener más información sobre las preferencias de seguridad del sistema, consulte [Configuración de las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Haga clic en **Guardar**.\
   La página se agrega automáticamente al panel. Si se crean tableros futuros, se puede agregar la página externa. La página externa se encuentra entre los informes disponibles.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Actualizar una página externa en un tablero

Para actualizar la información de una página externa utilizada en un tablero:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Tableros**.
1. Seleccione el tablero que desea actualizar y haga clic en **Editar** ![](assets/edit-icon.png).

   ![Seleccione el icono Editar .](assets/nwe-editdashboard2021-350x188.png)

1. En el lado derecho de la pantalla, busque la página externa que desee actualizar y haga clic en el botón **Editar** icono.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. En el **Editar página externa** , actualice los campos que desee cambiar y haga clic en **Guardar**.
1. (Opcional) Haga clic en el **Eliminar** icono ![](assets/delete.png) para eliminar la página externa del tablero. Para obtener más información, consulte [Eliminar una página externa de un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. En la esquina inferior izquierda, haga clic en **Guardar + Cerrar**.

## Ver páginas externas en un informe

Puede ver todas las páginas externas en Workfront en un informe de página externa.

1. Vaya a la **Menú principal** icono ![](assets/main-menu-icon.png) > **Informes**.
1. Haga clic en **Nuevo informe** > seleccione **Página externa**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Opcional) Actualice las pestañas Ver, Filtros o Agrupaciones del informe.

   Para obtener más información, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Haga clic en **Guardar y cerrar**.

   Puede ver el nombre y la dirección URL asociados con las páginas externas del sistema en el nuevo informe.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
