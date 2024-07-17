---
content-type: reference
product-area: reporting
keywords: auditoría, seguimiento, personalizado, campo
navigation-topic: calculate-custom-data-reports
title: "Ejemplo de campo personalizado calculado: mostrar el historial de edición de un campo"
description: Si los usuarios actualizan los campos personalizados de forma regular y desea capturar un registro de todos los cambios realizados en un campo, así como una fecha en la que se produzcan los cambios, puede capturar esta información en un campo personalizado calculado.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Ejemplo de campo personalizado calculado: mostrar el historial de edición de un campo

Si los usuarios actualizan los campos personalizados de forma regular y desea capturar un registro de todos los cambios realizados en un campo, así como una fecha en la que se produzcan los cambios, puede capturar esta información en un campo personalizado calculado.

El siguiente ejemplo muestra cómo generar el campo calculado *Instrucciones Editar historial* para capturar todos los cambios realizados en un campo de texto de una sola línea denominado *Instrucciones*.

>[!TIP]
>
>Puede seguir este ejemplo para todos los tipos de campos personalizados, no solo para los campos de texto de una sola línea.

Esto hace lo siguiente: 

* Limita el campo *Instrucciones Editar historial* a los últimos 2000 caracteres para permanecer dentro del límite de la base de datos de Workfront.
* Comprueba si el valor actual del campo *Instructions* coincide con la parte frontal del valor *Instructions Edit History*; supone que está en blanco y, en caso contrario, hace lo siguiente: 

   * Si coinciden, deja el *Historial de edición de instrucciones* tal cual;
   * Si no coinciden, reemplaza el *Historial de edición de instrucciones* por el valor más reciente del campo *Instrucciones*, seguido de la fecha actual entre paréntesis, una barra vertical y las *Instrucciones anteriores Editar historial*, que conservan los valores anteriores y la fecha en que se escribieron.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso administrativo a Forms personalizado</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Administrar permisos en los formularios personalizados </p> <p>Para obtener más información, vea <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartir un formulario personalizado</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Para agregar un campo calculado que muestre el historial de edición de un campo a un formulario personalizado, primero debe:

* Creación del formulario personalizado
* Agregue el campo cuyo historial desee capturar al formulario personalizado

## Mostrar el historial de edición de un campo

1. Vaya a un formulario personalizado en el que desee agregar el campo calculado.

1. Para crear el campo personalizado de texto de una sola línea, por ejemplo, haga lo siguiente:

   1. Haga clic en **Campo de texto de una línea**.
   1. Especifique una **Etiqueta** para el campo personalizado, como *Instrucciones*.
   1. Haga clic en **Aplicar**.

1. Seleccione **Agregar un campo** y después seleccione **Calculado** para agregar un campo personalizado calculado al formulario.
1. Especifique una **Etiqueta** para el campo personalizado calculado, como *Instrucciones Editar historial*.

   Este es el campo que capturará cualquier cambio realizado en el primer campo que creó (*Instrucciones*).

1. Haga clic en **Guardar + Cerrar**.
1. Haga clic en el nombre del formulario en el que ahora ha añadido dos campos para volver a abrirlo.
1. Haga clic en el campo personalizado calculado *Instrucciones Editar historial,* y, a continuación, copie y pegue lo siguiente en el cuadro Cálculo:
1. En el campo **Cálculo**, especifique el siguiente cálculo para el campo personalizado:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recomendado) Pegue el mismo cálculo en el campo **Instructions** del campo calculado en el formulario.
1. Asegúrese de que  **Texto** está seleccionado en el campo **Formato** para dar formato de texto al campo personalizado calculado.

   Esta es la opción predeterminada.

1. Haga clic en **Guardar+Cerrar**.

   Ahora, cuando adjunta el formulario personalizado a un objeto y alguien cambia la información en el campo *Instrucciones*, el campo *Instrucciones Editar historial&quot; muestra el valor más reciente, seguido de la fecha actual entre paréntesis y una barra vertical. Si se realizan más cambios, se añaden a esta información del mismo modo.

   En el cálculo anterior, puede reemplazar *Instrucciones* con el nombre exacto del campo de texto de una sola línea cuyo historial desee rastrear, y *Instrucciones Editar historial* con el nombre exacto del campo calculado.
