---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ejecutar y enviar un informe con los derechos de acceso de otro usuario
description: De forma predeterminada, los usuarios solo pueden ver los objetos de un informe para los que tengan permisos de visualización.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 269340bc6a0c237edf44f5aa325d4ff95b647df8
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Ejecutar y enviar un informe con los derechos de acceso de otro usuario

De forma predeterminada, los usuarios solo pueden ver los objetos de un informe para los que tengan permisos de visualización.

Puede permitir que todos los usuarios vean los mismos resultados que los demás usuarios en un informe, independientemente de su nivel de acceso o de permiso, en los objetos del informe.

Si ejecuta un informe con los derechos de acceso de otro usuario que tiene mayor acceso (por ejemplo, los derechos de acceso de un administrador de Adobe Workfront), todos los usuarios que tengan permisos para Ver el informe podrán ver la información en el informe como el usuario especificado en el creador de informes. Puede configurarlo para los informes que los usuarios encuentren en la interfaz de Workfront o para los informes que se envíen a los usuarios como datos adjuntos a un correo electrónico.

>[!TIP]
>
>Debe reemplazar el **Ejecute este informe con los derechos de acceso de:** con un usuario activo solo cuando desee que el informe se muestre con los derechos de acceso de ese usuario. Por ejemplo, es posible que un usuario de licencia de trabajo no tenga permisos para ver todos los elementos de un informe creado por un usuario con licencia de plan o un administrador del sistema, a menos que el informe se muestre con los derechos de acceso de un planificador o un administrador del sistema.\
Si el informe se comparte con usuarios con acceso similar al especificado en la variable **Ejecute este informe con los derechos de acceso de:** , puede dejar este campo en blanco.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de un informe (para ver el informe enviado)</p> <p>Administrar permisos para un informe (para ejecutar el informe)</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar un informe con los derechos de acceso de otro usuario

Rellenar el **Ejecute este informe con los derechos de acceso de:** garantiza que un informe contenga los mismos datos, independientemente de qué usuario acceda al informe. El informe se muestra como lo haría para el usuario especificado.

Los usuarios que accedan al informe deben tener al menos permisos de visualización en el informe para poder verlo. Si el usuario aparece en la lista **Ejecute este informe con los derechos de acceso de:** está desactivado, el informe ya no se muestra para ningún otro usuario con el que se comparta el informe.

Para ejecutar un informe con los derechos de acceso de otro usuario:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. Seleccione el informe que desee mostrar con los derechos de acceso de otro usuario.
1. Haga clic en **Acciones de informe** y haga clic en **Editar**.

1. Haga clic en **Configuración de informes**.

1. En el **Ejecute este informe con los derechos de acceso de:** , empiece a escribir el nombre del usuario como desea que se muestre el informe y, a continuación, selecciónelo cuando lo vea en la lista.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   Los usuarios con un nivel de acceso inferior a los que se les permite crear informes no tienen la capacidad de seleccionar otro usuario para el **Ejecute este informe con los derechos de acceso de:** campo .

1. Haga clic en **Listo**.
1. Haga clic en **Guardar + Cerrar**.\
   El informe ahora se muestra para todos los usuarios con los que se comparte el informe como si lo hubiera visto el usuario especificado en la sección **Ejecute este informe con los derechos de acceso de:** campo .

>[!IMPORTANT]
Introducción de un usuario que no sea el usuario que ha iniciado sesión para el **Ejecute este informe con los derechos de acceso de:** afecta a la información mostrada en el informe si el informe contiene un filtro que utiliza un comodín que hace referencia al usuario que ha iniciado sesión. El informe se muestra según el valor especificado en la variable **Ejecute este informe con los derechos de acceso de:** en lugar de lo que se define en el filtro comodín.
Para obtener más información sobre los comodines de los campos de usuario, consulte la sección &quot;Variables basadas en el usuario&quot; en [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Enviar un informe con los derechos de acceso de otro usuario

Puede configurar los informes para que se envíen como adjuntos a un correo electrónico. Puede configurar los informes entregados para que se muestren a los usuarios con un nivel de acceso superior, de modo que todos los usuarios puedan ver la misma información en los informes enviados. Los usuarios que verán el informe entregado en el correo electrónico deben agregarse a la lista Enviar a de destinatarios dentro de la entrega del informe. Para obtener más información sobre la configuración de un informe para su envío, consulte el artículo [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Para enviar un informe con los derechos de acceso de otro usuario:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. Seleccione el informe que desee enviar con los derechos de acceso de otro usuario.
1. Haga clic en el nombre del informe para seleccionarlo.
1. Haga clic en **Acciones de informe**.
1. Haga clic en **Enviar informe**.

1. En el **Enviar este informe con los derechos de acceso de:** , empiece a escribir el nombre del usuario que desea que el informe se muestre como cuando se envíe en un mensaje de correo electrónico y, a continuación, selecciónelo cuando lo vea en la lista. El valor predeterminado es el nombre del usuario que está creando el informe.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   Los usuarios con un nivel de acceso inferior a los que se les permite crear informes no tienen la capacidad de seleccionar un usuario distinto de sí mismos para el **Enviar este informe con los derechos de acceso de:** campo .

1. Seleccione el **Formato** desea que el informe se muestre en el correo electrónico:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Haga clic en **Enviar ahora** para enviarlo inmediatamente.\
   O\
   Haga clic en **Repetición de envío** para programar un envío recurrente del informe.\
   Para obtener más información sobre los envíos de informes, consulte el artículo [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).