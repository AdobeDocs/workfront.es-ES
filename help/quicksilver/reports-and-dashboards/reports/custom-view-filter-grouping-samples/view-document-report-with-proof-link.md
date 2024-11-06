---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: informe de documento con vínculo a una prueba"
description: "Ver: informe de documento con vínculo a una prueba"
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# Ver: informe de documento con vínculo a una prueba

<!--Audited: 11/2024-->

En esta vista de documento, puede insertar un vínculo a una prueba de la versión actual del documento.

![](assets/view-document-with-proof-link-350x92.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver un informe de documento con un vínculo a una prueba

Para aplicar esta vista:

1. Ir a una lista de documentos.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.
1. Haga clic en **Añadir columna**.
1. Haga clic en **Cambiar al modo de texto** y, a continuación, **Editar el modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

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

1. Haga clic en **Listo** y luego en **Guardar vista**.
1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
1. (Opcional) Para asegurarse de que solo se muestran los documentos con pruebas, agregue un filtro haciendo lo siguiente:

   1. Haga clic en el menú desplegable **Filtro** y luego haga clic en **Nuevo filtro**.
   1. Haga clic en **Agregar una regla de filtro** y empiece a escribir &quot;Propietario de prueba&quot;, luego seleccione **Identificador de propietario de prueba** cuando se muestre en la lista.
   1. Seleccione **No está en blanco** para el modificador de filtro.
   1. Haga clic en **Guardar filtro**.
   1. (Opcional) Actualice el nombre del filtro y, a continuación, haga clic en **Guardar filtro**.

1. Haga clic en el vínculo de la columna Vínculo de prueba para acceder a la prueba de la última versión del documento.
