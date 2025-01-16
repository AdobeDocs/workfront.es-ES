---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de traducción gestionada por SDL
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 80%

---

# Módulos de [!DNL SDL Managed Translation]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de traducción administrada por SDL](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/sdl-managed-translation-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede conectar su cuenta de [!DNL SDL Managed Translation] a varias aplicaciones y servicios de terceros.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Información de la API de traducción gestionada de SDL

El conector de traducción gestionada por SDL utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td>https://languagecloud.sdl.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.4.26</td> 
  </tr>
 </tbody> 
 </table>

## Módulos de [!DNL SDL Managed Translation]

>[!NOTE]
>
>El tiempo de espera de la operación para las llamadas a [!DNL SDL Managed Translation] es de **120 segundos**.

### Archivos

#### [!UICONTROL Download Translated File]

Este módulo recupera el contenido de un solo archivo traducido, contenido en el proyecto especificado. Si el archivo solicitado aún no se encuentra en el estado de descarga, es posible que el contenido del archivo aún no se haya traducido completamente. Si el archivo se encuentra en estado de descarga y lo ha recuperado correctamente, asegúrese de marcar el archivo como completado con el método `Cancel or Complete File`.

#### [!UICONTROL Upload a File]

Este módulo permite cargar archivos para su traducción o inclusión en un proyecto de traducción como material de referencia. Las cargas deben enviarse con multipart/form-data y pueden contener más de un archivo. Usted especifica los `ProjectOptionId` que se deben usar para evaluar los archivos cargados. Esto determina si cada archivo que carga es un posible candidato para la traducción o debe manejarse como material de referencia. En el caso de los archivos (`zip `, `rar`, `7z`, `tar`), la aplicación examina el contenido del archivo e indica si el archivo en su conjunto se puede traducir o si contiene una mezcla de archivos traducibles y no traducibles.

>[!NOTE]
>
>No se recomienda cargar más de un archivo a la vez, ya que puede aumentar el impacto de cualquier error.

#### [!UICONTROL Add a Reference File]

Este módulo añade un archivo de referencia.

### Proyectos

#### [!UICONTROL Create a project]

Este módulo crea el proyecto especificado.

#### Cancelar o completar un proyecto

Este módulo cancela o completa el proyecto especificado. Si el proyecto está a la espera de descarga, pasa a través de los pasos finales del flujo de trabajo y, finalmente, se mueve a finalización. Si el proyecto está a la espera de aprobación o si se cancela la selección del proveedor. Si el proyecto se encuentra en cualquier otro estado, la solicitud fallará.

#### [!UICONTROL Download Project Zip]

Este módulo obtiene el archivo `zip` de archivos traducidos para el proyecto especificado.

#### [!UICONTROL Read a Project]

Este módulo obtiene el proyecto especificado.

#### [!UICONTROL Obtener proyectos en estado]

Este módulo obtiene todos los proyectos disponibles en el estado especificado. Este método permite paginar los resultados especificando los parámetros de consulta `$top`, `$skip` y `$orderby`.

#### [!UICONTROL Obtener lista de proyectos]

Obtiene una lista simple de todos los proyectos, proporcionando información general sobre cada proyecto. Este método permite que los resultados sean páginas especificando los parámetros de consulta `$top`, `$skip` y `$orderby`.

#### [!UICONTROL Buscar opciones de creación de proyectos]

Este módulo obtiene las opciones de creación de proyectos.

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada de API autorizada arbitraria.
