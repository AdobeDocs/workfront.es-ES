---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: informe de documento con vínculo a una prueba"
description: "Ver: informe de documento con vínculo a una prueba"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

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
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver un informe de documento con un vínculo a una prueba

Para aplicar esta vista:

1. Ir a una lista de documentos.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Sustituya &quot;Su dominio&quot; por el dominio real de Workfront. Por ejemplo, si la dirección URL de Workfront de su compañía es *Company.my.workfront.com*, su dominio será &quot;Compañía&quot;.

1. Haz clic en **Guardar** y luego en **Guardar vista**.
1. Escriba un nombre para la vista y haga clic en **Guardar vista**.
1. (Opcional) Para asegurarse de que solo se muestran los documentos con pruebas, agregue un filtro haciendo lo siguiente:

   1. Haga clic en el menú desplegable **Filtro** y luego haga clic en **Nuevo filtro**.
   1. Haga clic en **Agregar una regla de filtro** y empiece a escribir Propietario de prueba; a continuación, seleccione **Identificador de propietario de prueba** cuando se muestre en la lista.
   1. Seleccione **No está en blanco** para el modificador de filtro.
   1. Haga clic en **Guardar filtro**, escriba el nombre del filtro y, a continuación, haga clic en **Guardar filtro**.

1. Haga clic en el vínculo de la columna Vínculo de prueba para acceder a la prueba de la última versión del documento.
