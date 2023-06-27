---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de traducción gestionada por SDL
description: En un [!DNL Adobe Workfront Fusion] En esta situación, puede conectar su cuenta de SDL Managed Translation a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] módulos

En un [!DNL Adobe Workfront Fusion] , puede conectar su [!DNL SDL Managed Translation] a varias aplicaciones y servicios de terceros.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Módulos

>[!NOTE]
>
>Tiempo de espera de la operación para llamadas a [!DNL SDL Managed Translation] es **120 segundos**.

### Archivos

#### [!UICONTROL Descargar archivo traducido]

Este módulo recupera el contenido de un solo archivo traducido, contenido en el proyecto especificado. Si el archivo solicitado aún no se encuentra en el estado Downland, es posible que el contenido del archivo aún no se haya traducido completamente. Si el archivo está en estado de descarga y lo ha recuperado correctamente, asegúrese de marcar el archivo como completado con el `Cancel or Complete File` método.

#### [!UICONTROL Cargar un archivo]

Este módulo permite cargar archivos para su traducción o inclusión en un proyecto de traducción como material de referencia. Las cargas deben enviarse con multipart/form-data y pueden contener más de un archivo. Usted especifica el `ProjectOptionId` que deben utilizarse para evaluar los archivos cargados. Esto determina si cada archivo que carga es un posible candidato para la traducción o debe manejarse como material de referencia. En el caso de los archivos (`zip `, `rar`, `7z`, `tar` archivos) la aplicación examina el contenido del archivo e indica si el archivo en su conjunto se puede traducir o si contiene una mezcla de archivos traducibles y no traducibles.

>[!NOTE]
>
>No se recomienda cargar más de un archivo a la vez, ya que puede aumentar el impacto de cualquier error.

#### [!UICONTROL Añadir un archivo de referencia]

Este módulo añade un archivo de referencia.

### Proyectos

#### [!UICONTROL Crear un proyecto]

Este módulo crea el proyecto especificado.

#### Cancelar o completar un proyecto

Este módulo cancela o completa el proyecto especificado. Si el proyecto está a la espera de descarga, pasa a través de los pasos finales del flujo de trabajo y, finalmente, se mueve a finalización. Si el proyecto está a la espera de aprobación o si se cancela la selección del proveedor. Si el proyecto se encuentra en cualquier otro estado, la solicitud fallará.

#### [!UICONTROL Descargar archivo comprimido del proyecto]

Este módulo obtiene el `zip` archivo de archivos traducidos para el proyecto especificado.

#### [!UICONTROL Leer un proyecto]

Este módulo obtiene el proyecto especificado.

#### [!UICONTROL Obtener proyectos en estado]

Este módulo obtiene todos los proyectos disponibles en el estado especificado. Este método permite paginar los resultados, especificando `$top`, `$skip`, y `$orderby` parámetros de consulta.

#### [!UICONTROL Obtener lista de proyectos]

Obtiene una lista simple de todos los proyectos, que proporciona información general sobre cada proyecto. Este método permite que los resultados sean páginas, al especificar `$top`, `$skip`, y `$orderby` parámetros de consulta.

#### [!UICONTROL Buscar opciones de creación de proyectos]

Este módulo obtiene las opciones de creación de proyectos.

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada de API autorizada arbitraria.
