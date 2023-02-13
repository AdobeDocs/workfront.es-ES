---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Compartir un informe en Adobe Workfront
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a problemas, consulte Concesión de acceso a informes, tableros y calendarios.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Compartir un informe en Adobe Workfront

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a problemas, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Junto con el nivel de acceso al que se concede a los usuarios, también puede concederles permisos para ver o administrar informes específicos a los que tenga acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento.

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos para cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

## Requisitos de acceso

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores del informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre cómo compartir informes

Además de las consideraciones siguientes, consulte [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Puede compartir informes que cree con otras personas, equipos, grupos, roles de trabajo o empresas. También puede compartir informes creados por otros usuarios y compartidos con usted.
* También puede compartirlas con toda la organización o hacerlas públicas. Si un informe se hace público, se genera una dirección URL que se puede compartir con otros usuarios.
* Puede compartir un informe individual o varios informes de una lista de informes.

## Formas de compartir informes

Puede compartir informes en Workfront de la siguiente manera:

* Manualmente, tal como se describe en la sección [Compartir un informe](#share-a-report) a continuación.
* De forma automática, heredando los permisos de Vista de un tablero que contiene el informe que se ha compartido. Para obtener información sobre la visualización de permisos heredados en objetos, consulte [Ver permisos heredados en objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartir un informe {#share-a-report}

Compartir uno o varios informes de una lista es idéntico.

1. Vaya a la lista de informes, seleccione uno o varios informes y haga clic en **Compartir**.

   O

   Haga clic en el nombre de un informe y, a continuación, haga clic en **Acciones de informe >****Uso compartido**.

   ![](assets/qs-report-actions-sharing.png)

1. En el cuadro que aparece, en la sección **Agregar personas, equipos, funciones, grupos o empresas...** campo empiece a escribir el nombre del usuario, equipo, función de trabajo, grupo o empresa con el que desee compartir el informe y, a continuación, presione **Entrar** cuando se muestre el nombre.

1. Para ajustar el nivel de acceso de un nombre agregado, haga clic en el menú desplegable a la derecha del nombre y, a continuación, elija una de las opciones siguientes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Permite que el destinatario vea el informe en la variable <strong>Informes</strong> <img src="assets/reports-in-main-menu.png"> y ejecútelo.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan <strong>Compartir</strong> con cualquiera del sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Permite que el destinatario tenga acceso completo a la edición del informe.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan <strong>Eliminar</strong> el informe del sistema y <strong>Compartir</strong> con cualquiera del sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los dos pasos anteriores para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Haga clic en el **Engranaje** icono ![](assets/gear-icon-settings-with-dn-arrow.jpg) en la esquina superior derecha del cuadro de uso compartido, seleccione una de las siguientes opciones:

   * **Convertir esto en público para usuarios externos:** Seleccione esta opción para generar una URL que se pueda compartir con otros usuarios. Cualquier persona con la dirección URL puede acceder al informe sin tener una licencia de Adobe Workfront.

      >[!CAUTION]
      >
      >Se recomienda tener cuidado al compartir un objeto que contenga información confidencial con usuarios externos. Esto les permite ver información sin ser usuarios de Workfront ni formar parte de su organización.

      >[!NOTE]
      >
      >Si el informe tiene una solicitud y la comparte públicamente, los usuarios que lo ejecuten deben iniciar sesión en Workfront para poder ejecutar el informe mediante la solicitud. Si no pueden iniciar sesión en Workfront, verán el informe sin la solicitud aplicada. Para obtener más información sobre las limitaciones al compartir informes con mensajes, consulte la sección [Limitaciones en el uso compartido de los informes solicitados](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) en el artículo [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Haga que esto sea visible en todo el sistema:** Seleccione esta opción para que todos los usuarios de Workfront con acceso a los informes puedan ver el informe.

1. Haga clic en **Guardar**.
