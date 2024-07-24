---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Enumerar usuarios con una licencia de revisión en Adobe Workfront
description: Puede ver qué usuarios de Adobe Workfront tienen actualmente activada la opción "Usuario puede generar pruebas" de cualquiera de las siguientes maneras.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Enumerar usuarios con una licencia de revisión en Adobe Workfront

Puede ver qué usuarios de Adobe Workfront tienen actualmente activada la opción &quot;Usuario puede generar pruebas&quot; de cualquiera de las siguientes maneras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Creación de un informe de usuario

Puede crear un informe de usuario para ver qué usuarios pueden generar pruebas:

1. Vaya al área **Informes**.
1. Haga clic en el menú desplegable **Nuevo informe** y, a continuación, haga clic en **Informe del usuario**.

1. En la ficha **Filtros**, haga clic en **Agregar una regla de filtro**.

1. En el campo disponible, expanda **Usuario** y luego haga clic en **Tiene licencia de revisión**.

1. Seleccione **Igual** > **Verdadero**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Haga clic en **Guardar+Cerrar**.

   El informe muestra todos los usuarios de Workfront que tienen asignada una licencia de revisión.

## Actualizar la vista Personas

Puede agregar una nueva columna en la vista Personas para ver qué usuarios pueden generar pruebas:

1. Vaya al área **Personas**.
1. Haga clic en la ficha **Personas**.
1. En el menú desplegable **Ver**, realice una de las acciones siguientes:

   * Para agregar esta información a una vista existente, seleccione la vista que desee personalizar y, a continuación, haga clic en **Personalizar vista**.
   * Para agregar esta información a una nueva vista, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. En el campo disponible, expanda **Usuario** y luego haga clic en **Tiene licencia de revisión**.

1. Haga clic en **Listo** y, a continuación, haga clic en **Guardar vista** o en **Guardar como nueva vista**.

   La vista muestra **True** o **False**, dependiendo de si el usuario tiene asignada una licencia de revisión.
