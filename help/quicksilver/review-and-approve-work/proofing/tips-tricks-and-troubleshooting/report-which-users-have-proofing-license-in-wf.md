---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Enumerar usuarios con una licencia de revisión en Adobe Workfront
description: Puede ver qué usuarios de Adobe Workfront tienen actualmente habilitada la opción "El usuario puede generar pruebas" de cualquiera de las siguientes maneras.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 100%

---

# Enumerar usuarios con una licencia de revisión en Adobe Workfront

Puede ver qué usuarios de Adobe Workfront tienen actualmente habilitada la opción &quot;El usuario puede generar pruebas&quot; de cualquiera de las siguientes maneras.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
   <p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de edición a:</p> 
    <ul> 
     <li> <p>Creación de informes, paneles de control y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un informe de usuario

Puede crear un informe de usuario para ver qué usuarios pueden generar pruebas:

1. Vaya al área **Creación de informes**.
1. Haga clic en el menú desplegable **Nuevo informe** y seleccione **Informe de usuario**.

1. En la ficha **Filtros**, haga clic en **Añadir una regla de filtro**.

1. En el campo disponible, expanda **Usuario** y luego haga clic en **Tiene licencia de revisión**.

1. Seleccione **Igual** > **Verdadero**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Haga clic en **Guardar + Cerrar**.

   El informe muestra todos los usuarios de Workfront que tienen asignada una licencia de revisión.

## Actualizar la vista Personas

Puede añadir una nueva columna en la vista Personas para ver qué usuarios pueden generar pruebas:

1. Vaya al área **Personas**.
1. Haga clic en la pestaña **Personas**.
1. En el menú desplegable **Ver**, realice una de las siguientes acciones:

   * Para añadir esta información a una vista existente, seleccione la vista que desee personalizar y, a continuación, haga clic en **Personalizar vista**.
   * Para añadir esta información a una nueva vista, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. En el campo disponible, expanda **Usuario** y luego haga clic en **Tiene licencia de revisión**.

1. Haga clic en **Listo** y, a continuación, haga clic en **Guardar vista** o en **Guardar como nueva vista**.

   La vista muestra **Verdadero** o **Falso**, dependiendo de si el usuario tiene asignada una licencia de revisión.
