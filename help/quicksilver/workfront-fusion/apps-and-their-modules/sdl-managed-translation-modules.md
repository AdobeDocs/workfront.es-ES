---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de traducción gestionada de SDL
description: En un [!DNL Adobe Workfront Fusion] , puede conectar su cuenta de traducción gestionada de SDL a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Módulos

>[!NOTE]
>
>El tiempo de espera de operación para las llamadas a [!DNL SDL Managed Translation] es **120 segundos**.

### Archivos

#### [!UICONTROL Descargar archivo traducido]

Este módulo recupera el contenido de un solo archivo traducido, incluido en el proyecto especificado. Si el archivo solicitado aún no está en estado de Downland, es posible que el contenido del archivo no se haya traducido por completo. Si el archivo está en estado de descarga y lo ha recuperado correctamente, asegúrese de marcar el archivo como completo mediante la función `Cancel or Complete File` método.

#### [!UICONTROL Cargar un archivo]

Este módulo permite cargar archivos para su traducción o para incluirlos en un proyecto de traducción como material de referencia. Las cargas deben enviarse mediante multipart/form-data y pueden contener más de un archivo. Especifique la variable `ProjectOptionId` que debe utilizarse para evaluar los archivos cargados. Esto determina si cada archivo que se carga es un posible candidato para la traducción o debe manejarse como material de referencia. En el caso de los archivos (`zip `, `rar`, `7z`, `tar` ) la aplicación examina el contenido del archivo e indica si se puede traducir el archivo en su conjunto o si contiene una mezcla de archivos traducibles y no traducibles.

>[!NOTE]
>
>No se recomienda cargar más de un archivo a la vez, ya que puede aumentar el impacto de cualquier error.

#### [!UICONTROL Agregar un archivo de referencia]

Este módulo agrega un archivo de referencia.

### Proyectos

#### [!UICONTROL Crear un proyecto]

Este módulo crea el proyecto especificado.

#### Cancelar o completar un proyecto

Este módulo cancela o completa el proyecto especificado. Si el proyecto está a la espera de su descarga, el proyecto pasa por cualquier paso final del flujo de trabajo y, finalmente, se traslada para completarse. Si el proyecto está a la espera de aprobación o se cancela la selección del proveedor. Si el proyecto se encuentra en cualquier otro estado, la solicitud fallará.

#### [!UICONTROL Descargar archivo comprimido del proyecto]

Este módulo obtiene la variable `zip` archivo de archivos traducidos para el proyecto especificado.

#### [!UICONTROL Leer un proyecto]

Este módulo obtiene el proyecto especificado.

#### [!UICONTROL Obtención de proyectos en estado]

Este módulo obtiene todos los proyectos disponibles en el estado especificado. Este método permite paginar los resultados, especificando `$top`, `$skip`y `$orderby` parámetros de consulta.

#### [!UICONTROL Obtener lista de proyectos]

Obtiene una lista sencilla de todos los proyectos, con información general sobre cada proyecto. Este método permite que los resultados sean páginas, especificando `$top`, `$skip`y `$orderby` parámetros de consulta.

#### [!UICONTROL Buscar opciones de creación de proyectos]

Este módulo obtiene Opciones de creación de proyectos.

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada API autorizada arbitraria.
