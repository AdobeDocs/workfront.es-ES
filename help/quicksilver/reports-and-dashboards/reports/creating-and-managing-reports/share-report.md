---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Uso compartido de informes en Adobe Workfront
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a los problemas, consulte Conceder acceso a informes, paneles y calendarios.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Uso compartido de informes en Adobe Workfront

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a los problemas, consulte [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver o Administrar informes específicos que tiene acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos de un elemento en Workfront y definen qué acciones se pueden realizar sobre ese elemento.

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

## Requisitos de acceso

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver el acceso o superior a Informes, Paneles, Calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores en el informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre el uso compartido de informes

Además de las consideraciones siguientes, vea [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Puede compartir informes que cree con otras personas, equipos, grupos, funciones del puesto o empresas. También puede compartir informes creados por otros y que se compartieron con usted.
* También puede compartirlos con toda la organización o hacerlos públicos. Al hacer público un informe, se genera una dirección URL que se puede compartir con otros usuarios.
* Puede compartir un informe individual o varios informes a partir de una lista de informes.

## Formas de compartir informes

Puede compartir informes en Workfront de la siguiente manera:

* Manualmente, tal como se describe en la sección [Compartir un informe](#share-a-report) a continuación.
* De forma automática, heredando los permisos de Vista de un panel que contiene el informe que se ha compartido. Para obtener información acerca de cómo ver permisos heredados en objetos, vea [Ver permisos heredados en objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartir un informe {#share-a-report}

Compartir uno o varios informes de una lista es idéntico.

1. Vaya a una lista de informes y seleccione uno o varios informes; después, haga clic en **Compartir**.

   O

   Haga clic en el nombre de un informe y, a continuación, haga clic en **Acciones de informe >****Uso compartido**.

   ![](assets/qs-report-actions-sharing.png)

1. En el cuadro que aparece, en el campo **Agregar personas, equipos, roles, grupos o empresas ...**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir el informe y, a continuación, presione **Entrar** cuando aparezca el nombre.

1. Para ajustar el nivel de acceso de un nombre que haya agregado, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, elija una de las opciones siguientes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Permite que el destinatario acceda para ver el informe en el área de <strong>Informes</strong> <img src="assets/reports-in-main-menu.png"> y ejecutarlo.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan <strong>compartirlo</strong> con cualquier persona del sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Permite que el destinatario tenga acceso completo de edición al informe.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan <strong>eliminar</strong> el informe del sistema y <strong>compartirlo</strong> con cualquier persona del sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los dos pasos anteriores para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Haga clic en el icono **Engranaje** ![](assets/gear-icon-settings-with-dn-arrow.jpg) en la esquina superior derecha del cuadro para compartir y, a continuación, seleccione una de las siguientes opciones:

   * **Convertir esto en público para los usuarios externos:** Seleccione esta opción para generar una dirección URL que se pueda compartir con otros. Cualquier persona con la dirección URL puede acceder al informe sin tener una licencia de Adobe Workfront.

     >[!CAUTION]
     >
     >Se recomienda precaución al compartir un objeto que contenga información confidencial con usuarios externos. Esto les permite ver información sin ser usuarios de Workfront ni parte de su organización.

     >[!NOTE]
     >
     >Si el informe tiene una solicitud y usted lo comparte públicamente, los usuarios que ejecuten el informe a través del vínculo compartido público no podrán ejecutar el informe utilizando la solicitud. Verán el informe sin el mensaje aplicado, a menos que inicien sesión en Workfront y accedan al informe sin utilizar el vínculo compartido público. Para obtener más información acerca de las limitaciones de compartir informes con indicadores, vea la sección [Limitaciones del uso compartido de informes con mensajes](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) en el artículo [Agregar un mensaje a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Hacer esto visible en todo el sistema:** Seleccione esta opción para que todos los usuarios de Workfront con acceso a los informes puedan ver el informe.

1. Haga clic en **Guardar**.
