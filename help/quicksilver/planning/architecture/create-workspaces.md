---
title: Crear espacios de trabajo
description: Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning. Los tipos de registro están organizados por secciones en un espacio de trabajo.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ca8f1375d641531eaf11e3889ccb67a6fbe1788f
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 35%

---


# Crear espacios de trabajo

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning.

Para obtener información general acerca de los espacios de trabajo, consulte [Información general sobre los espacios de trabajo](/help/quicksilver/planning/architecture/workspaces-overview.md).

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
<p>Cualquier paquete de flujo de trabajo o Workfront</p> 
<p>Cualquier paquete de Workfront Planning</p>
<p>Un paquete de Workfront Planning Prime o superior <span class="preview"> para crear varios espacios de trabajo a la vez</span></p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   <p><span class="preview">Administrador del sistema para crear varios espacios de trabajo al mismo tiempo mediante el paquete de plantillas de prácticas recomendadas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Crear un espacio de trabajo

Puede crear un espacio de trabajo y agregarle tipos de registro para organizar los objetos en Workfront Planning.

Para obtener más información acerca de cómo editar un área de trabajo, vea [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

Puede crear espacios de trabajo de las siguientes maneras:

* Crear un espacio de trabajo desde cero o desde una plantilla

  Para obtener más información, vea la sección [Crear un área de trabajo desde cero o desde una plantilla](#create-a-workspace-from-scratch-or-from-a-template) en este artículo.
* Cree un espacio de trabajo con Planning Designer con tecnología de IA. Actualmente, esta función solo está disponible para un número limitado de clientes en un programa de Beta.

  Para obtener más información, consulte [Introducción a Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

<div class="preview">

* Cree varios espacios de trabajo con un paquete de plantillas de varios espacios de trabajo de prácticas recomendadas

  Para obtener más información, consulte la sección [Crear varios espacios de trabajo mediante un paquete de plantillas de varios espacios de trabajo de prácticas recomendadas](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) en este artículo

  >[!TIP]
  >
  >Solo puede crear varios espacios de trabajo al mismo tiempo si utiliza el paquete de plantillas de prácticas recomendadas.


</div>

### Crear un espacio de trabajo desde cero o desde una plantilla

{{step1-to-planning}}

1. Haga clic en **Crear espacio de trabajo**

   Se muestra el cuadro Crear espacio de trabajo. Puede crear un espacio de trabajo desde cero o crearlo con una de las plantillas disponibles.

1. (Opcional y condicional) Haga clic en **Vista previa** dentro de cualquiera de las siguientes plantillas de área de trabajo predefinidas:

   * Básico: administración de marketing
   * Administración avanzada de marketing
   * Empresa: administración de marketing
   * Administración de ventas
   * Administración de productos

   Se abrirá el cuadro de vista previa de plantilla.

   Existe una indicación de qué tipos de registros operativos, taxonomías y cuántos campos están asociados a cada plantilla.

   ![Vista previa de una plantilla de área de trabajo](assets/previewing-a-workspace-template.png)

   Para obtener información acerca de las plantillas de espacio de trabajo de Workfront Planning, consulte [Lista de plantillas de espacio de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

1. En el cuadro de vista previa de la plantilla, haga clic en **Usar plantilla** para comenzar a crear el espacio de trabajo a partir de la plantilla seleccionada

   O

   Haga clic en **Atrás** y, a continuación, haga clic en **Nuevo espacio de trabajo** para crear un espacio de trabajo desde cero.

   Se crea uno para los siguientes tipos de espacios de trabajo:

   * Un espacio de trabajo vacío denominado **Espacio de trabajo sin título** donde puede empezar a añadir tipos de registros manualmente al crear un espacio de trabajo desde cero.
   * Espacio de trabajo con el nombre de la plantilla seleccionada que se rellena con tipos de registros de ejemplo. Puede personalizar aún más los tipos de registro y el espacio de trabajo.

   Para los administradores de Workfront, el nuevo espacio de trabajo se muestra en la ficha **Espacios de trabajo en los que participo**.

   Para todos los demás usuarios que pueden crear espacios de trabajo, el nuevo espacio de trabajo se muestra en el área **Espacios de trabajo**.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse Entrar.

1. (Opcional y condicional) Si creó el área de trabajo a partir de una plantilla, haga clic dentro del nombre de las secciones **Tipos de registros operativos** o **Taxonomías**

   O

   Pase el ratón sobre el nombre de una sección, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre de la sección.

   >[!TIP]
   >
   >Puede cambiar el nombre de cualquier sección desde cualquier espacio de trabajo, incluso si no ha creado la sección.

   Para obtener más información sobre la edición de espacios de trabajo, incluida la edición de espacios de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Haga clic en **Añadir tipo de registro** para añadir tipos de registro al área de trabajo en cualquier sección.

   Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obtener más información sobre la edición y eliminación de tipos de registros en un área de trabajo, consulte [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Haga clic en la flecha hacia atrás situada a la izquierda del nuevo espacio de trabajo para abrir la página principal de Planning. Se crea una tarjeta de área de trabajo nueva para el área de trabajo nueva en la ficha **Espacios de trabajo en los que estoy**.

   El nombre del usuario que creó el espacio de trabajo se guarda en la tarjeta del espacio de trabajo como Propietario.

   >[!NOTE]
   >
   >Para los usuarios que están realizando la transición al sistema Identity Management de Adobe (IMS), los espacios de trabajo creados por usuarios solo de Workfront que no son usuarios de IMS se muestran según lo creado por **System**.
   >
   >Para obtener información sobre IMS, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

<div class="preview">

### Cree varios espacios de trabajo con un paquete de plantillas de varios espacios de trabajo de prácticas recomendadas

>[!IMPORTANT]
>
>La creación de varios espacios de trabajo a la vez mediante el paquete de plantillas de prácticas recomendadas solo está disponible cuando se cumplen los siguientes requisitos previos:
>
>* Su organización ha adquirido un paquete de Workfront Planning Prime o Ultimate.
>* Usted es administrador de sistemas

Puede utilizar un paquete de plantillas de varios espacios de trabajo para crear 6 espacios de trabajo con un solo clic.

Las plantillas incluidas en el paquete contienen espacios de trabajo, tipos de registros, registros, vistas y campos para ayudarle a empezar con la implementación de Planning.

>[!IMPORTANT]
>
>Los nombres de los espacios de trabajo y los registros incluidos en el paquete son ejemplos y no reflejan su propio entorno.
>
>Los nombres de los tipos de registros y campos se pueden utilizar en cualquier organización como estándar para la implementación en cualquier sector, según nuestra recomendación.
>

{{step1-to-planning}}

1. Haga clic en **Crear espacio de trabajo**

   Se muestra el cuadro Crear espacio de trabajo. Puede crear un espacio de trabajo desde cero o crearlo con una de las plantillas disponibles.

1. Haga clic en **Revisar configuración del área de trabajo** en el área **Comenzar aquí (recomendado)**.
1. (Opcional) Haga clic en **Vista previa** dentro de cualquiera de las siguientes plantillas de área de trabajo predefinidas para abrir el cuadro Vista previa de cada plantilla:

   * 1.Clasificaciones globales y taxonomías

     La plantilla Clasificaciones globales y taxonomías incluye todos los tipos de registros y campos que le recomendamos que cree en su entorno para una implementación correcta de Workfront Planning.

     Posteriormente, puede vincular o importar los tipos de registros de esta plantilla en otros espacios de trabajo que cree.
   * 2.Fréscopa Marketing global
   * 3.Fréscopa Social Marketing
   * 4.Fréscopa Media &amp; PR
   * 5.Eventos globales de Fréscopa
   * 6.Fréscopa Executive Liderazgo de la empresa

1. Después de abrir el cuadro **Vista previa** para cada plantilla de área de trabajo, haga clic en Atrás para volver al cuadro **Crear área de trabajo** o haga clic en Usar plantillas para usar las plantillas, incluso en el paquete y crear áreas de trabajo.

   Los espacios de trabajo se crean y se muestran en las fichas **Espacios de trabajo en los que estoy** y **Todos los espacios de trabajo** para los administradores del sistema. Todos los usuarios con licencia estándar verán los espacios de trabajo en su área de espacios de trabajo después de que un administrador del sistema los cree y comparta los nuevos espacios de trabajo con ellos.

1. Comience a editar los espacios de trabajo que ha creado y a añadir tipos de registros, registros, vistas y campos que sean pertinentes para su organización.

   Para obtener más información acerca de las prácticas recomendadas para implementar Workfront, vea los artículos de la sección [Prácticas recomendadas de Adobe Workfront Planning: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

   Para obtener información sobre cómo editar espacios de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

</div>



