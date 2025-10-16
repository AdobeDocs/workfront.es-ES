---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Proyectos en los que participo, incluidos resultados inesperados
description: Lea este artículo para solucionar los problemas del filtro Proyectos en los que participo, incluidos los resultados inesperados.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 25%

---

# El filtro proyectos en los que estoy incluye resultados inesperados

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>paquete de Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td><p>Estándar</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Problema

El filtro [!UICONTROL **Proyectos en los que participo**] incluye resultados que no esperaría, ya que no estoy asignado o asociado con esos proyectos.

## Solución

El filtro [!UICONTROL **Proyectos en los que participo**] incluye proyectos que contienen al usuario en cualquiera de sus campos [!UICONTROL **Detalles del proyecto**], incluidos los campos que se pueden perder fácilmente o que se rellenan automáticamente, como [!UICONTROL **Ingresado por**] o [!UICONTROL **Identificador de patrocinador**]. Para eliminar los resultados no deseados, existen dos soluciones posibles:

1. Compruebe [!UICONTROL **Detalles del proyecto**] para cada proyecto inesperado incluido por el filtro y quite el nombre de todos los campos.

   O

1. Intente usar un filtro similar, como [!UICONTROL **Proyectos de mi propiedad**], que solo incluye los proyectos que se le hayan asignado específicamente.

Para obtener más información sobre el uso de filtros en [!DNL Workfront], vea [Información general sobre filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
