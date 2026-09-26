---
title: Restringir el acceso a datos financieros en campos personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Al crear un campo personalizado, puede definir configuraciones opcionales para restringir el acceso a los datos financieros.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 11%
---
# Restringir el acceso a datos financieros en campos personalizados

Al crear un campo personalizado, puede definir configuraciones opcionales para restringir el acceso a los datos financieros. De este modo, los usuarios que tienen determinados permisos configurados en sus niveles de acceso pueden ver los datos y se les impide ver datos financieros a los que no deberían tener acceso.

Para obtener información sobre cómo crear un campo personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obtener información acerca de los niveles de acceso, vea [Información general sobre los niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Para obtener información acerca de los permisos de uso compartido y de, vea [Información general sobre los permisos de uso compartido en objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr>  
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a formularios personalizados</td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Restringir el acceso a los datos financieros en un campo personalizado

1. Cree un nuevo formulario personalizado o abra uno existente.

   Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Agregue un campo personalizado al formulario o seleccione un campo existente.

   Estos tipos de campo se pueden restringir en función del acceso a los datos financieros:

   * Texto de línea única
   * Párrafo
   * Menú desplegable de selección única
   * Menú desplegable de selección múltiple
   * Grupo de casillas de verificación
   * Botones de radio
   * Búsqueda externa
   * Consulta externa de selección múltiple
   * Calculado

1. En el campo **Formato**, seleccione **Moneda**.

   >[!NOTE]
   >
   >Para los campos calculados, se permite cualquier formato. Todos los demás tipos de campo deben usar el formato **Currency**; de lo contrario, el campo **Tipo de permiso Finance** no estará disponible.

1. (Opcional) Solo para campos calculados, active la opción **Permiso automático** para permitir que los permisos financieros provengan automáticamente de los campos de la fórmula.

1. Seleccione una opción para el **tipo de permiso Finanzas**.

   Los usuarios deben tener este tipo de permiso de finanzas para poder ver o editar este campo personalizado en el formulario.

   * **No se requieren permisos:** Todos los usuarios pueden ver este campo
   * **General:** Los usuarios deben tener permisos para editar o ver Finanzas generales
   * **Factura:** Los usuarios deben tener permisos para editar o ver las tarifas de facturación
   * **Costo:** Los usuarios deben tener permisos para editar o ver las tasas de costo

   Para campos calculados:

   * El campo **Tipo de permiso financiero** no está disponible para la configuración manual de permisos si el campo **Permiso automático** está activado.
   * Los campos utilizados en la fórmula determinan si el campo de permiso está activo. Si el campo de permiso está en blanco (y los permisos automáticos no están activados), los campos de la fórmula no admiten los permisos financieros.
   * El acceso es obligatorio para todos los campos de la fórmula. Por ejemplo, si se utilizan dos campos en un campo calculado y uno de ellos tiene permiso de facturación aplicado y el segundo tiene permiso de costes aplicado, el usuario debe tener permisos para ver las tarifas de facturación y de coste para ver el valor calculado.

1. Para guardar los cambios, haz clic en **Aplicar** y continúa creando el formulario.

   O

   Haga clic en **Guardar y Cerrar**.

## Ejemplo

Dos proyectos se comparten con un usuario:

* El usuario tiene permisos para editar todas las opciones financieras del primer proyecto
* El usuario tiene permisos para ver las tarifas de facturación y las finanzas generales del segundo proyecto

Cuando el usuario edita el primer proyecto, todos los campos financieros del formulario personalizado se pueden editar. Cuando el usuario edita el segundo proyecto, los campos establecidos en **Bill** o **General** son de solo lectura y los campos establecidos en **Cost** no son visibles.

Cuando el usuario ve los proyectos en una lista o informe:

* Los campos de finanzas se pueden ver o editar según los permisos y la configuración del informe
* Los campos de finanzas están en blanco si el usuario no tiene permisos para verlos

La exportación de detalles del proyecto muestra los mismos valores de campo financiero (o campos en blanco) que en la lista.

Al editar ambos proyectos por lotes, los campos facturación y finanzas generales se muestran como de solo lectura, y los campos de coste como N/A.
