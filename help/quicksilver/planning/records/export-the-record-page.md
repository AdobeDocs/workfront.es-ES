---
title: Exportar la página de registro
description: Puede exportar la vista previa o la página de detalles de un registro desde Adobe Workfront Planning a un archivo de Microsoft Word.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6mGLH9rvSZu9TEoVyuYHyrqPNr78Rruy97jxvayl1nc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a93c6c9faf26d5eab1c223bd4a2646af896bf97d
workflow-type: tm+mt
source-wordcount: 441
ht-degree: 22%

---

# Exportar detalles de un registro


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes o en el entorno de producción para los clientes que habilitaron versiones rápidas.</span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Para colaborar de forma más eficaz con otras personas que no tengan una cuenta de Workfront, puede exportar la página de detalles de un registro a un archivo de Microsoft Word y compartirlo con ellas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p> <p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Ligero o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Ver permisos superiores a un área de trabajo, tipo de registro y <span class="preview">registro</span> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
  </tr>

</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Light or higher</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
 -->


## Consideraciones sobre la exportación de los detalles de un registro:

* Puede exportar los detalles de un registro a los siguientes formatos de archivo:

   * .docx Word
   * .pdf

* Sólo se puede exportar la ficha Detalles de la página o del área de vista previa de un registro.

* El archivo exportado conserva el diseño de la página de registro, incluidas las miniaturas y las imágenes de la portada.

## Exportar detalles de un registro

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran en tarjetas.

1. Haga clic en una tarjeta de tipo de registro.
Se abre la página de tipo de registro y se muestran todos los registros de ese tipo.

1. En cualquier vista, haga clic en el nombre de un registro.

   Se abre el cuadro de vista previa del registro.

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) para abrir la página del registro.

1. Elija la ficha **Detalles**. La pestaña Detalles se debe abrir de forma predeterminada.

1. Haga clic en el icono **Exportar** del menú ![Exportar en la página de detalles del registro](assets/export-icon-in-record-details-page.png), ya sea en la vista previa o en la página del registro y, a continuación, haga clic en una de las siguientes opciones:

   * **Microsoft Word**
   * **Adobe PDF**

   Un archivo de Word (.docx) o PDF se descarga y se guarda en el equipo.

   El nombre del archivo exportado es el campo Primary del registro.

   ![Archivo de Word exportado](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    La información adicional que no se muestra en la página y que solo está visible después de hacer clic en Mostrar más en el área de detalles del registro no se muestra en el archivo PDF exportado. En el archivo exportado solo se muestra la información visible en la página.


1. (Opcional) Vaya al archivo descargado, ábralo y edítelo (si es un archivo de Word), o compártalo con otros.

