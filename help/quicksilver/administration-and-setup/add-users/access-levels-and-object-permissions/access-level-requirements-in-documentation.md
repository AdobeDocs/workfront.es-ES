---
title: Requisitos de acceso en la documentación de Workfront
content-type: reference
product-area: system-administration
keywords: acceso,nivel,sistema,administrador,planificador,trabajador,revisor,solicitante,externo,usuario
navigation-topic: access-levels
description: Los artículos de procedimientos de la documentación de Workfront contienen una tabla que explica el acceso y los permisos necesarios para ese procedimiento. Este artículo explica la tabla de requisitos de acceso con más detalle y contiene vínculos para obtener más información.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Requisitos de acceso en la documentación de Workfront

Los artículos de procedimientos de la documentación de Workfront contienen una tabla que explica los requisitos de acceso y permisos necesarios para ese procedimiento. Esta tabla de requisitos de acceso le permite comprender si puede realizar una determinada acción en Workfront o por qué no. Este artículo explica cada elemento de la tabla de requisitos de acceso y proporciona sugerencias para la resolución de problemas y vínculos a información más detallada.

Si una fila está ausente de la tabla de requisitos de acceso de un artículo determinado, no hay requisitos de ese tipo para esa acción.

Algunas filas contienen información con las etiquetas &quot;Nuevo&quot; y &quot;Actual&quot;. Esto se debe a que Workfront está realizando una transición hacia un nuevo modelo de precios y empaquetado, en el que algunas organizaciones operan bajo el nuevo modelo y otras siguen utilizando el modelo actual. Para saber qué modelo utiliza su organización, póngase en contacto con el administrador de Workfront. Puede encontrar detalles y vínculos a información en la sección [Tabla de requisitos de acceso](#the-access-requirements-table) de este artículo.

>[!NOTE]
>
>Si tiene alguna pregunta sobre cómo se aplica cualquiera de los campos de esta tabla, póngase en contacto con el administrador de Workfront.

## La tabla Requisitos de acceso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> Los planes de Adobe Workfront hacen referencia al conjunto de funciones que su organización ha adquirido. La mayoría de las funciones de Workfront están disponibles en todos los planes, con algunas excepciones, la mayoría relacionadas con la planificación estratégica y los controles empresariales. 
   <ul><li>Para saber qué plan de Adobe Workfront utiliza su organización, incluido si su organización se encuentra en el modelo de empaquetado nuevo o actual, póngase en contacto con su administrador de Workfront.</li>
   <li>Para obtener instrucciones sobre cómo un administrador de Workfront puede localizar el plan Workfront de su organización, consulte <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Ver el clúster de su organización y el plan Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> Las licencias de Adobe Workfront hacen referencia al conjunto de funciones de Workfront incluidas en la licencia asignada. Por ejemplo, un usuario puede tener una licencia que incluye marcar los elementos de trabajo como completos y registrar el tiempo, mientras que otro usuario tiene una licencia que solo le permite aprobar recursos o enviar solicitudes. <p> 
   <ul>
   <li>Para saber qué licencia se le ha asignado, póngase en contacto con el administrador de Workfront.</li>
   <li>Adobe Workfront está realizando una transición hacia un nuevo modelo de precios y empaquetado. Para obtener más información sobre las licencias, consulte:
   <ul>
   <li>Nuevo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Información general sobre nuevas licencias</a></li>
   <li>Actual: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias</a></li></ul></li>
   <li>Si tiene el nivel de acceso correcto y aún no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront ofrece algunos productos que se pueden comprar además de Workfront.
   <p>Los artículos que describen los procedimientos realizados dentro de estos productos adicionales enumeran el producto requerido aquí.</p>
   <ul>
   <li>Adobe Experience Manager Assets para Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Planificador de escenarios de Workfront</li>
   </ul>
   <p>Para saber si su organización ha adquirido uno de estos productos adicionales, póngase en contacto con su administrador de Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> Los niveles de acceso son conjuntos de permisos para acciones que puede realizar en Workfront y que establece el administrador de Workfront. <p>Workfront tiene niveles de acceso integrados que corresponden a las licencias de Workfront, pero el administrador de Workfront puede crear niveles de acceso más amplios para reflejar con mayor precisión los conjuntos de permisos necesarios en su organización.</p>
   <ul>
    <li>Adobe Workfront está realizando una transición hacia un nuevo modelo de precios y empaquetado. Para obtener información sobre los niveles de acceso de cada modelo, consulte:
   <ul>
   <li>Nuevo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Información general sobre nuevos niveles de acceso</a></li>
   <li>Actual: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Resumen de niveles de acceso</a></li></ul></li>
    <li>Para obtener más información sobre el nivel de acceso, póngase en contacto con el administrador de Workfront</li>
    <li>Si es administrador de Workfront, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuración del acceso a Adobe Workfront</a> para obtener más información sobre la concesión de acceso a objetos específicos en el nivel de acceso.</li>  
   <li>Si tiene el nivel de acceso correcto y aún no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Los permisos de objeto hacen referencia al acceso que tiene a objetos de Workfront individuales cuando los crea o cuando se comparten con usted. Por ejemplo, debe tener acceso de Vista a un proyecto específico para ver el proyecto, aunque el nivel de acceso le permita ver los proyectos. Esta sección de la tabla de requisitos de acceso describe los permisos de objeto específicos que necesita para realizar la acción en el artículo.</p>
   <p>Para obtener información sobre cómo solicitar acceso adicional a un objeto, vea <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p><p>Para obtener información sobre cómo compartir un objeto, vea <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Compartir un objeto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Plantilla de diseño</td> 
   <td><p>Las plantillas de diseño controlan lo que se puede ver en el menú principal y las configura el administrador de Workfront. Esta línea indica cualquier área específica de Workfront que deba incluirse en el menú principal para realizar la acción.</p><p>En general, si un artículo le indica que haga clic en un área del menú principal y esa área no está visible en el menú principal, póngase en contacto con el administrador de Workfront para determinar si ese área está disponible para usted.</p><p>
   Para obtener información sobre cómo un administrador de Workfront puede configurar el menú principal, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personalizar el menú principal con una plantilla de diseño</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront Fusion</td> 
   <td>Adobe Workfront Fusion tiene un modelo de licencia independiente al de Workfront. 
   <ul><li>Actual: El modelo de licencia actual se basa en el número de operaciones realizadas y no tiene limitaciones en las acciones que puede realizar una organización. </li>
   <li>Heredado: las licencias heredadas se basan en si los escenarios pueden conectarse a aplicaciones de terceros o si solo se utilizan para la automatización de Workfront. </li>
   </ul>
   Para obtener información sobre las licencias de Fusion, consulte <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Licencias de Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
