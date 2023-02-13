---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Almacenes de datos en [!DNL Adobe Workfront Fusion]
description: Un almacén de datos, similar a una base de datos o a una tabla sencilla, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios o ejecuciones de escenarios individuales. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Almacenes de datos en [!DNL Adobe Workfront Fusion]

Un almacén de datos, similar a una base de datos o a una tabla sencilla, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios o ejecuciones de escenarios individuales. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.

Los módulos del almacén de datos permiten realizar las siguientes acciones en los registros de su [!DNL Adobe Workfront Fusion] almacén de datos:

* Agregar
* Reemplazar
* Actualizar
* Recuperar
* Eliminar
* Buscar
* Cuenta

Para obtener información sobre el uso de módulos de almacén de datos, consulte [[!UICONTROL Almacén de datos] módulos](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Cree un almacén de datos en [!DNL Workfront Fusion]

* [Configuración del almacén de datos](#set-up-the-data-store)
* [Configuración de la estructura de datos](#set-up-the-data-structure)

### Configuración del almacén de datos

Para poder utilizar un almacén de datos en un módulo, debe crear el almacén de datos en [!DNL Workfront Fusion].

>[!NOTE]
>
>Su organización tiene un número limitado de almacenes de datos disponibles. Si intenta crear más almacenes de datos de los que tiene disponibles, [!DNL Workfront] devuelve un valor [!UICONTROL Alcanzado máximo de tiendas] error.
>
>Para obtener más información, consulte [Error máximo alcanzado](#maximum-stores-reached-error) en este artículo.

1. Inicie sesión en su [!DNL Workfront Fusion] cuenta.
1. Haga clic en **[!UICONTROL Almacenes de datos]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Añadir almacén de datos]** en la esquina superior derecha de la pantalla.
1. Introduzca la configuración del nuevo almacén de datos.

   Un título en negrita en un campo de una [!DNL Workfront Fusion] indica una configuración necesaria.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data store name] </td> 
      <td> <p>Introduzca un nombre para el almacén de datos. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data Structure]</p> </td> 
      <td> <p>Una estructura de datos es una lista de las columnas de una tabla. Esta lista indica el nombre de la columna y el tipo de datos.</p> <p>Realice una de las siguientes acciones:</p> 
       <ul> 
        <li style="font-weight: bold;">Seleccionar una estructura de datos que ya se haya creado</li> 
        <li> <p style="font-weight: bold;">Añadir una nueva estructura de datos</p> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para crear una nueva estructura de datos.</p> <p>Para obtener más información, consulte la <a href="#set-up-the-data-structure" class="MCXref xref">Configuración de la estructura de datos</a> en este artículo.</p> </li> 
        <li style="font-weight: bold;"> <p>Deje el campo vacío</p> <p style="font-weight: normal;">Si no selecciona ni agrega una estructura de datos, la base de datos solo contendrá la clave principal. Este tipo de base de datos es útil si desea guardar claves únicamente y está interesado en saber solamente si existe o no una clave específica en la base de datos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Tamaño de almacenamiento de datos en MB]</p> </td> 
      <td> <p>Asigne el tamaño para el almacén de datos desde el almacenamiento de datos interno total.</p> <p>Nota: La cantidad reservada se puede cambiar en cualquier momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configuración de la estructura de datos

1. Al crear o editar un almacén de datos, haga clic en **[!UICONTROL Agregar]**.
1. En el **[!UICONTROL Agregar estructura de datos]** que se muestra, configure los siguientes campos:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nombre de estructura de datos]</td> 
      <td> <p> Introduzca un nombre para la nueva estructura de datos.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Realice una de las siguientes acciones para configurar las columnas del almacén de datos.</p> 
       <ul> 
        <li> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong> para especificar las propiedades de una columna manualmente.</p> <p>Introduzca la variable <strong>[!UICONTROL Name]</strong> y <strong>[!UICONTROL Type]</strong> para la columna almacén de datos y defina las propiedades correspondientes.</p> </li> 
        <li> <p>Haga clic en <strong>[!UICONTROL Generator]</strong> para determinar las columnas a partir de los datos de ejemplo que proporcione.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
          <p>Por ejemplo, los siguientes datos de muestra de JSON crean tres columnas: nombre, edad y número de teléfono. El número de teléfono es una colección de números de teléfono móvil y de línea fija.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>Las columnas vacías en la vista del almacén de datos:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>A continuación, puede agregar valores al almacén de datos manualmente o utilizando la variable [!DNL Workfront Fusion] módulos del almacén de datos.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estricto] </td> 
      <td> <p>Active esta opción para asegurarse de que la carga útil coincide con las estructuras de datos. Las cargas que contienen elementos adicionales no especificados en la estructura de datos se rechazan.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Editar un almacén de datos existente

Puede editar las propiedades y el contenido de un almacén de datos existente en el [!UICONTROL Almacén de datos] área de [!DNL Workfront Fusion].

* [Edición de las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store)
* [Edición del contenido de un almacén de datos](#edit-the-contents-of-a-data-store)

### Edición de las propiedades de un almacén de datos

Las propiedades de un almacén de datos incluyen la estructura de datos que utiliza el almacén de datos, así como el tamaño del almacén de datos.

1. Haga clic en **[!UICONTROL Almacén de datos]** ![](assets/data-store-icon.png) en el panel de navegación izquierdo para abrir el [!UICONTROL Almacén de datos] .
1. Haga clic en **[!UICONTROL Editar]** ![](assets/data-store-edit.png) junto al almacén de datos que desea editar.
1. (Opcional) Si desea cambiar la estructura de datos utilizada por este almacén de datos a otra estructura de datos existente, selecciónela en el **[!UICONTROL Estructura de datos]** lista desplegable.

   O

   (Opcional) Si desea cambiar la estructura de datos utilizada por este almacén de datos a una estructura de datos completamente nueva, consulte [Configuración de la estructura de datos](#set-up-the-data-structure) en este artículo.

1. (Opcional) Cambie el tamaño del almacén de datos introduciendo el nuevo tamaño en la variable **[!UICONTROL Tamaño de almacenamiento de datos en MB]** campo .
1. Haga clic en **[!UICONTROL Guardar]**.

### Edición del contenido de un almacén de datos

1. Haga clic en el **[!UICONTROL Almacén de datos]** icono ![](assets/data-store-icon.png) en el panel de navegación izquierdo para abrir el [!UICONTROL Almacén de datos] .
1. Haga clic en **[!UICONTROL Examinar]** ![](assets/browse-data-store.png) junto al almacén de datos que desea editar.
1. (Opcional) Reordene las columnas arrastrándolas a la ubicación deseada.
1. (Opcional) [!UICONTROL Editar] una celda única haciendo clic en el botón **[!UICONTROL Editar]** icono ![](assets/data-store-edit.png)en esa celda, introduzca el valor deseado.
1. (Opcional) Agregue un nuevo elemento al almacén de datos haciendo clic en **[!UICONTROL Agregar]** y, a continuación, introduciendo la información del nuevo artículo.
1. Haga clic en **[!UICONTROL Guardar]**.

## Resolución de problemas

* [Restauración de datos perdidos de un almacén de datos](#restoring-lost-data-from-a-data-store)
* [Error de falta de espacio](#out-of-space-error)
* [Error máximo alcanzado](#maximum-stores-reached-error)

### Restauración de datos perdidos de un almacén de datos

Actualmente no hay ninguna herramienta que pueda automatizar la restauración de los datos perdidos.

#### Solución alternativa

1. Examine todos los registros de ejecución de escenarios en los que se insertaron elementos en el almacén de datos.

   Para obtener más información sobre cómo examinar los registros de ejecución, consulte [Ver el historial de ejecución de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copie los datos.
1. Vuelva a insertar los datos en el almacén de datos.

   Para obtener información sobre cómo insertar datos en un almacén de datos, consulte [Edición del contenido de un almacén de datos](#edit-the-contents-of-a-data-store) en este artículo.

### [!UICONTROL Sin espacio] error

Un [!UICONTROL Fuera de espacio] se produce un error porque a los almacenes de datos creados anteriormente ya se les ha asignado el almacenamiento del almacén de datos asignado.

#### Solución alternativa

1. Edite cualquiera de los almacenes de datos existentes para utilizar menos espacio. Esto libera espacio para el nuevo almacén de datos.

   Para obtener más información, consulte [Edición de las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store) en este artículo.

>[!NOTE]
>
>Se recomienda no asignar todo el espacio a un único almacén de datos a menos que esté seguro de que no necesitará más almacenes de datos.

### [!UICONTROL Alcanzado máximo de tiendas] error

A [!UICONTROL Alcanzado máximo de tiendas] se produce un error porque su organización ha utilizado todos los almacenes de datos disponibles. Una organización tiene varios almacenes de datos disponibles que equivalen al doble del número de escenarios disponibles. Por lo tanto, el número total de almacenes de datos disponibles depende del plan que haya comprado.

Por ejemplo, si su organización ha adquirido un plan con 15 escenarios, la organización puede tener hasta 30 almacenes de datos.

#### Solución alternativa

Para reducir el número de almacenes de datos existentes, considere la posibilidad de realizar una de las siguientes acciones:

* Combinación de almacenes de datos existentes
* Eliminar almacenes de datos no utilizados
