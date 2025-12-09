---
title: Enumerar los niveles de acceso y las licencias de los usuarios
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,nivel,licencia
navigation-topic: access-levels
description: Puede ver qué nivel de acceso y licencia se asigna a cada usuario en una lista de usuarios o informe.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5d85509d-276a-411e-813c-8b1fa2f512db
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 93%

---

# Enumerar los niveles de acceso y las licencias de los usuarios

>[!NOTE]
>
>La información de este artículo hace referencia a los niveles de acceso heredados. Para obtener información acerca de los nuevos niveles de acceso, vea [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Puede ver qué nivel de acceso y licencia se asigna a cada usuario en una lista de usuarios o informe.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver el acceso de los usuarios. Para obtener más información sobre el acceso para ver usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

+++

## Enumerar los niveles de acceso y las licencias de los usuarios

{{step-1-to-users}}

De forma predeterminada, todos los usuarios configurados como Activos se muestran en la lista.

1. En el menú desplegable **Ver**, seleccione **Licencias**.

   La columna Licencia muestra el nombre de la licencia asignada a cada usuario.

1. En el menú desplegable **Agrupación**, haga clic en **Tipo de licencia**.

   Esta vista agrupa a los usuarios que tienen los mismos tipos de licencia.

1. (Opcional) Para filtrar la lista por una licencia específica:

   1. Haga clic en el menú **Filtro** y seleccione **Nuevo filtro**.

   1. Haga clic en **Añadir regla de filtro**.
   1. Empiece a escribir **Licencia** y selecciónela cuando aparezca en la lista.
   1. Con el modificador **Equal** seleccionado, empiece a escribir el nombre de la licencia por la que desea filtrar la lista.

      Puede especificar más de un tipo de licencia.

   1. Haga clic en **Guardar filtro**.

      La lista muestra únicamente los usuarios asociados a los tipos de licencia especificados en el filtro.

   >[!TIP]
   >
   >También puede agrupar la lista por tipos de licencia o filtrarla por una licencia específica.

