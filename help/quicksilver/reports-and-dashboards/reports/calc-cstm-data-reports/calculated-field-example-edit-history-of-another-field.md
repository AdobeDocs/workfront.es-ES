---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: 'Ejemplo de campo personalizado calculado: mostrar el historial de ediciones de un campo'
description: Si los usuarios actualizan los campos personalizados de forma regular y desea capturar un registro de todos los cambios realizados en un campo, así como una fecha en la que se produzcan los cambios, puede capturar esta información en un campo personalizado calculado.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 54%

---

# Ejemplo de campo personalizado calculado: mostrar el historial de ediciones de un campo

Si los usuarios actualizan los campos personalizados de forma regular y desea capturar un registro de todos los cambios realizados en un campo, así como una fecha en la que se produzcan los cambios, puede capturar esta información en un campo personalizado calculado.

El siguiente ejemplo muestra cómo crear el campo calculado Instructions Edit History para capturar todos los cambios realizados en un campo de texto de una sola línea denominado Instructions.

>[!TIP]
>
>Puede seguir este ejemplo para todos los tipos de campos personalizados, no solo para los campos de texto de una sola línea.

Esto hace lo siguiente:

* Limita el campo Historial de edición de instrucciones a los últimos 2000 caracteres para permanecer dentro del límite de la base de datos de Workfront.
* Comprueba si el valor actual del campo Instrucciones coincide con la parte frontal del valor Historial de edición de instrucciones; supone que está en blanco y, si no lo está, hace lo siguiente:

   * Si coinciden, deja el Historial de edición de instrucciones tal cual;
   * Si no coinciden, reemplaza el historial de edición de instrucciones con el último valor del campo Instrucciones, seguido de la fecha actual entre paréntesis, una barra vertical y el historial de edición de instrucciones anterior, que conserva los valores anteriores y la fecha en que se introdujeron.

## Requisitos de acceso

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>paquete de Adobe Workfront</p> </td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td>
      <p>Estándar</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraciones de nivel de acceso</p></td> 
   <td> <p>Acceso administrativo a Forms personalizado</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto</p> </td> 
   <td> <p>Permisos de administración de los formularios personalizados</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para añadir un campo calculado que muestre el historial de ediciones de un campo a un formulario personalizado, primero deberá hacer lo siguiente:

* Crear el formulario personalizado
* Añadir el campo cuyo historial desea capturar al formulario personalizado

## Mostrar el historial de ediciones de un campo

1. Vaya a un formulario personalizado en el que desee añadir el campo calculado.

1. Para crear el campo personalizado de texto de una sola línea, por ejemplo, haga lo siguiente:

   1. Haga clic en **Texto de una sola línea**.
   1. Especifique una **Etiqueta** para el campo personalizado. Por ejemplo, puede llamarlo &quot;Instrucciones&quot;.
   1. Haga clic en **Aplicar**.

1. Haga clic en **Calculado** para añadir un campo personalizado calculado al formulario.
1. Especifique una **Etiqueta** para el campo personalizado calculado. Por ejemplo, puede llamarlo &quot;Instrucciones Editar historial&quot;.

   Este es el campo que captura los cambios realizados en el primer campo creado (&quot;Instrucciones&quot;).

1. Haga clic en **Guardar y Cerrar**.
1. Haga clic en el nombre del formulario en el que ahora ha añadido dos campos para volver a abrirlo.
1. Haga clic en el campo personalizado calculado **Instrucciones Editar historial** y, a continuación, copie y pegue lo siguiente en el cuadro **Cálculo**:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recomendado) Pegue el mismo cálculo en el campo **Instrucciones** en el campo calculado en el formulario.
1. Asegúrese de que **Texto** está seleccionado en el campo **Formato** para dar formato de texto al campo personalizado calculado.

   Es la opción predeterminada.

1. Haga clic en **Guardar y Cerrar**.

   Ahora, cuando adjunta el formulario personalizado a un objeto y alguien cambia la información en el campo **Instrucciones**, el campo **Instrucciones Editar historial** muestra el valor más reciente, seguido de la fecha actual entre paréntesis y una barra vertical. Si se realizan más cambios, se añaden a esta información del mismo modo.

   En el cálculo anterior, puede reemplazar *Instrucciones* por el nombre exacto del campo de texto de una sola línea cuyo historial desee rastrear, e **Historial de ediciones de instrucciones** por el nombre exacto del campo calculado.
