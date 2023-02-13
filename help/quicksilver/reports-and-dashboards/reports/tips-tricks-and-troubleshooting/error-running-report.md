---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Mensaje de error al ejecutar un informe: "Actualmente no ha iniciado sesión".'
description: 'Debe tener el siguiente acceso para realizar los pasos de este artículo: EDITAR.'
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# Mensaje de error al ejecutar un informe: &quot;Actualmente no ha iniciado sesión.&quot;

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, Trabajar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Problema

Al ejecutar un informe o mostrarlo en un tablero, se devuelve el siguiente error:\
*Intentémoslo de nuevo. Aún no ha iniciado sesión.*

No se muestran resultados en el informe.

## Causa

El informe está configurado para ejecutarse como usuario desactivado.

## Solución

Debe tener permisos de administración en el informe para poder cambiar la configuración del informe.\
Para ajustar el informe y ver los resultados:

1. Vaya al informe .
1. Haga clic en **Acciones de informe** > **Editar** > **Configuración de informes**.

1. Especifique el nombre de un usuario activo en la variable **Ejecute este informe con los derechos de acceso de:** campo .\
   O\
   Deje el **Ejecute este informe con los derechos de acceso de:** campo en blanco.

1. Haga clic en **Listo**.
1. Haga clic en **Guardar + Cerrar**.\
   El error no debería aparecer de nuevo al ejecutar este informe.
