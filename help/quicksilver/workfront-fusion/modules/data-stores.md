---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Almacenes de datos en [!DNL Adobe Workfront Fusion]
description: Un almacén de datos, similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: e71f276eb510497c026a70400afc754d5f57b60b
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Almacenes de datos en [!DNL Adobe Workfront Fusion]

Un almacén de datos, similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Creación de un almacén de datos en [!DNL Workfront Fusion]

* [Configuración del almacén de datos](#set-up-the-data-store)
* [Configuración de la estructura de datos](#set-up-the-data-structure)

### Configuración del almacén de datos

Para poder usar un almacén de datos en un módulo, debe crear el almacén de datos en [!DNL Workfront Fusion].

>[!NOTE]
>
>Su organización tiene un número limitado de almacenes de datos disponibles. Si intenta crear más almacenes de datos de los que tiene disponibles, [!DNL Workfront] devuelve un valor [!UICONTROL Se alcanzó el máximo de tiendas] error.
>
>Para obtener más información, consulte [Error de número máximo de tiendas alcanzado](#maximum-stores-reached-error) en este artículo.

1. Inicie sesión en su [!DNL Workfront Fusion] cuenta.
1. Clic **[!UICONTROL Almacenes de datos]** en el panel de navegación izquierdo.
1. Clic **[!UICONTROL Añadir almacén de datos]** en la esquina superior derecha de la pantalla.
1. Introduzca la configuración del nuevo almacén de datos.

   Un título en negrita en un campo de una [!DNL Workfront Fusion] module indica una configuración requerida.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nombre del almacén de datos] </td> 
      <td> <p>Escriba un nombre para el almacén de datos. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Estructura de datos]</p> </td> 
      <td> <p>Una estructura de datos es una lista de las columnas de una tabla. Esta lista indica el nombre de columna y el tipo de datos.</p> <p>Realice una de las siguientes acciones:</p> 
       <ul> 
        <li style="font-weight: bold;">Seleccione una estructura de datos que ya se haya creado</li> 
        <li> <p style="font-weight: bold;">Añadir una nueva estructura de datos</p> <p>Clic <strong>[!UICONTROL Agregar]</strong> para crear una nueva estructura de datos.</p> <p>Para obtener más información, consulte la <a href="#set-up-the-data-structure" class="MCXref xref">Configuración de la estructura de datos</a> de este artículo.</p> </li> 
        <li style="font-weight: bold;"> <p>Deje el campo vacío.</p> <p style="font-weight: normal;">Si no selecciona ni añade una estructura de datos, la base de datos solo contendrá la clave principal. Este tipo de base de datos es útil si sólo desea guardar claves y sólo le interesa saber si existe o no una clave específica en la base de datos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Tamaño de almacenamiento de datos en MB]</p> </td> 
      <td> <p>Asigne el tamaño del almacén de datos desde el almacenamiento de datos interno total.</p> <p>Nota: El importe reservado se puede cambiar en cualquier momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configuración de la estructura de datos

1. Al crear o editar un almacén de datos, haga clic en **[!UICONTROL Añadir]**.
1. En el **[!UICONTROL Añadir estructura de datos]** que se muestra, configure los campos siguientes:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nombre de estructura de datos]</td> 
      <td> <p> Introduzca un nombre para la nueva estructura de datos.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Especificación]</p> </td> 
      <td> <p>Realice una de las siguientes acciones para configurar las columnas del almacén de datos.</p> 
       <ul> 
        <li> <p>Clic <strong>[!UICONTROL Agregar elemento]</strong> para especificar las propiedades de una columna manualmente.</p> <p>Introduzca el <strong>[!UICONTROL Nombre]</strong> y <strong>[!UICONTROL Tipo]</strong> para la columna del almacén de datos y defina las propiedades correspondientes.</p> </li> 
        <li> <p>Clic <strong>[!UICONTROL Generator]</strong> para determinar las columnas a partir de los datos de ejemplo proporcionados.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
          <p>Por ejemplo, los siguientes datos de ejemplo de JSON crean tres columnas: nombre, edad y número de teléfono. Número de teléfono es una colección de números de teléfono móviles y de teléfono fijo.</p> 
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
          <p>A continuación, puede agregar valores al almacén de datos manualmente o utilizando [!DNL Workfront Fusion] módulos de almacén de datos.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estricto] </td> 
      <td> <p>Active esta opción para asegurarse de que la carga útil coincida con las estructuras de datos. Se rechazarán las cargas que contengan elementos adicionales no especificados en la estructura de datos.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Editar un almacén de datos existente

Puede editar las propiedades y el contenido de un almacén de datos existente en la [!UICONTROL Almacén de datos] área de [!DNL Workfront Fusion].

* [Editar las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store)
* [Editar el contenido de un almacén de datos](#edit-the-contents-of-a-data-store)

### Editar las propiedades de un almacén de datos

Las propiedades de un almacén de datos incluyen la estructura de datos que utiliza el almacén de datos, así como el tamaño de éste.

1. Clic **[!UICONTROL Almacén de datos]** ![](assets/data-store-icon.png) en el panel de navegación izquierdo para abrir [!UICONTROL Almacén de datos] área.
1. Clic **[!UICONTROL Editar]** ![](assets/data-store-edit.png) situado junto al almacén de datos que desea editar.
1. (Opcional) Si desea cambiar la estructura de datos utilizada por este almacén de datos a otra estructura de datos existente, selecciónela en el **[!UICONTROL Estructura de datos]** menú desplegable.

   O

   (Opcional) Si desea cambiar la estructura de datos utilizada por este almacén de datos a una estructura de datos completamente nueva, consulte [Configuración de la estructura de datos](#set-up-the-data-structure) en este artículo.

1. (Opcional) Cambie el tamaño del almacén de datos introduciendo el nuevo tamaño en la variable **[!UICONTROL Tamaño de almacenamiento de datos en MB]** field.
1. Haga clic en **[!UICONTROL Guardar]**.

### Editar el contenido de un almacén de datos

1. Haga clic en **[!UICONTROL Almacén de datos]** icono ![](assets/data-store-icon.png) en el panel de navegación izquierdo para abrir [!UICONTROL Almacén de datos] área.
1. Clic **[!UICONTROL Examinar]**  situado junto al almacén de datos que desea editar.
1. (Opcional) Reordene las columnas arrastrándolas a la ubicación deseada.
1. (Opcional) [!UICONTROL Editar] una sola celda haciendo clic en el botón **[!UICONTROL Editar]** en esa celda y, a continuación, introduzca el valor deseado.
1. (Opcional) Agregue un nuevo elemento al almacén de datos haciendo clic en **[!UICONTROL Añadir]**, a continuación, introduzca la información del nuevo elemento.
1. Haga clic en **[!UICONTROL Guardar]**.

## Resolución de problemas

* [Restauración de datos perdidos de un almacén de datos](#restoring-lost-data-from-a-data-store)
* [Error de falta de espacio](#out-of-space-error)
* [Error de número máximo de tiendas alcanzado](#maximum-stores-reached-error)

### Restauración de datos perdidos de un almacén de datos

Actualmente no hay ninguna herramienta que pueda automatizar la restauración de los datos perdidos.

#### Solución alternativa

1. Examine todos los registros de ejecución de escenarios en los que se insertaron elementos en el almacén de datos.

   Para obtener más información sobre el examen de los registros de ejecución, consulte [Visualización del historial de ejecución de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copie los datos.
1. Vuelva a insertar los datos en el almacén de datos.

   Para obtener información sobre cómo insertar datos en un almacén de datos, consulte [Editar el contenido de un almacén de datos](#edit-the-contents-of-a-data-store) en este artículo.

### [!UICONTROL Espacio insuficiente] error

Un [!UICONTROL Espacio insuficiente] Se produce un error porque los almacenes de datos creados anteriormente ya se han asignado al almacenamiento del almacén de datos asignado.

#### Solución alternativa

1. Edite cualquiera de los almacenes de datos existentes para utilizar menos espacio. Esto libera espacio para el nuevo almacén de datos.

   Para obtener más información, consulte [Editar las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store) en este artículo.

>[!NOTE]
>
>Le recomendamos que no asigne todo su espacio a un único almacén de datos a menos que esté seguro de que no necesitará más almacenes de datos.

### [!UICONTROL Se alcanzó el máximo de tiendas] error

A [!UICONTROL Se alcanzó el máximo de tiendas] Este error se produce porque su organización ha utilizado todos sus almacenes de datos disponibles. Una organización tiene un número de almacenes de datos disponibles que equivale al doble del número de escenarios disponibles. Por lo tanto, el número total de almacenes de datos disponibles depende del plan que haya adquirido.

Por ejemplo, si su organización ha adquirido un plan con 15 escenarios, puede tener hasta 30 almacenes de datos.

#### Solución alternativa

Para reducir el número de almacenes de datos existentes, considere la posibilidad de realizar una de las siguientes acciones:

* Combinación de almacenes de datos existentes
* Eliminar almacenes de datos no utilizados
