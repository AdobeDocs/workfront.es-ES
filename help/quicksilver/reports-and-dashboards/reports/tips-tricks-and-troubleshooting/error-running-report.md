---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Mensaje de error al ejecutar un informe: ''Actualmente no ha iniciado sesión''".'
description: Obtenga información acerca del mensaje de error "Actualmente no ha iniciado sesión".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 3%

---

# Mensaje de error al ejecutar un informe: &quot;Actualmente no ha iniciado sesión&quot;.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, Trabajo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Problema

Al ejecutar un informe o mostrarlo en un panel, se devuelve el siguiente error:\
*Intentémoslo de nuevo. Actualmente no ha iniciado sesión.*

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

1. Haga clic en **Listo**.
1. Haga clic en **Guardar + Cerrar**.\
   El error no debería aparecer de nuevo al ejecutar este informe.
