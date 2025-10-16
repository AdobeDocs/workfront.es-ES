---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensaje de error al ejecutar un informe: "Actualmente no ha iniciado sesión".'
description: Obtenga información acerca del mensaje de error “Actualmente no ha iniciado sesión”.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 93%

---

# Mensaje de error al ejecutar un informe: “Actualmente no ha iniciado sesión”.

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
     <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

Al ejecutar un informe o mostrarlo en un panel de control, se devuelve el siguiente error:\
*Intentémoslo de nuevo. Aún no ha iniciado sesión.*

No se muestran resultados en el informe.

## Causa

El informe está configurado actualmente para ejecutarse como un usuario desactivado.

## Solución

Debe tener permisos de administración en el informe para poder cambiar la configuración del informe.\
Para ajustar el informe y ver los resultados:

1. Vaya al informe.
1. Haga clic en **Acciones de informe** > **Editar** > **Configuración de informe**.

1. Especifique el nombre de un usuario activo en el campo **Ejecutar este informe con los derechos de acceso de:**.\
   O\
   Deje el campo **Ejecutar este informe con los derechos de acceso de:** en blanco.

1. Haga clic en **Aceptar**.
1. Haga clic en **Guardar + Cerrar**.\
   El error no debería aparecer de nuevo al ejecutar este informe.
