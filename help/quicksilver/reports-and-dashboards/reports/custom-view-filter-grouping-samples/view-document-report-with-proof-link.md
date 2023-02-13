---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: informe de documento con vínculo a una prueba'
description: 'Ver: informe de documento con vínculo a una prueba'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Ver: informe de documento con vínculo a una prueba

En esta vista de documento, puede insertar un vínculo a una prueba de la versión actual del documento.

![](assets/view-document-with-proof-link-350x92.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver un informe de documento con un vínculo a una prueba

Para aplicar esta vista:

1. Vaya a una lista de documentos.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. Haga clic en **Agregar columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Sustituya &quot;Su dominio&quot; por su dominio real de Workfront. Por ejemplo, si la dirección URL de Workfront de la empresa es *Company.my.workfront.com*, su dominio es &quot;Empresa&quot;.

1. Haga clic en **Guardar**, luego **Guardar vista**.
1. Escriba un nombre para la vista y haga clic en **Guardar vista**.
1. (Opcional) Para asegurarse de que solo se muestran documentos con pruebas, agregue un filtro haciendo lo siguiente:

   1. Haga clic en el **Filtro** menú desplegable y haga clic en **Nuevo filtro**.
   1. Haga clic en **Agregar una regla de filtro** y empiece a escribir Propietario de prueba, a continuación seleccione **ID del propietario de la prueba** cuando se muestre en la lista.
   1. Select **No está en blanco** para el modificador de filtro.
   1. Haga clic en **Guardar filtro**, escriba el nombre del filtro y haga clic en **Guardar filtro**.

1. Haga clic en el vínculo en la columna Proof Link para acceder a la prueba de la última versión del documento.
