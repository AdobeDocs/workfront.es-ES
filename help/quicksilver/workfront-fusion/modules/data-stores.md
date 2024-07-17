---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Almacenes de datos en  [!DNL Adobe Workfront Fusion]
description: Un almacén de datos, similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 00a969175626d27b70d516921097725fdf818799
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# Almacenes de datos en [!DNL Adobe Workfront Fusion]

Un almacén de datos, similar a una base de datos o tabla simple, puede almacenar datos de escenarios, lo que permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Puede utilizar un almacén de datos para almacenar nuevos datos de varios sistemas durante la sincronización.

Los módulos del almacén de datos permiten realizar las siguientes acciones en los registros del almacén de datos [!DNL Adobe Workfront Fusion]:

* Agregar
* Reemplazar
* Actualizar
* Recuperar
* Eliminar
* Buscar
* Cuenta

Para obtener información sobre el uso de módulos de almacén de datos, consulte [[!UICONTROL Módulos del almacén de datos]](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Para ver un vídeo introductorio a los almacenes de datos de Workfront Fusion, consulte:

* [Almacenes de datos](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Heredado: cualquiera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe adquirir [!DNL Adobe Workfront Fusion].</li><li>Se incluye el plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion].</li></ul>
   <p>O</p>
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Espacio de datos disponible

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

Si su organización está en el nuevo modelo de plan de Workfront (paquetes Select, Prime y Ultimate), el plan de su organización afecta al tamaño y el número de almacenes de datos disponibles en su instancia de Fusion.

### Plan definitivo

Las instancias de Fusion en el paquete Ultimate reciben:

* 100 MB de espacio
* 50 almacenes de datos

### Planes Select y Prime

Las instancias de Fusion en los paquetes Select o Prime reciben:—>

* 100 MB para las primeras 500K operaciones.

* 10 MB por cada operación adicional de 100.000.

  Por ejemplo, una organización con 600 000 operaciones recibe 110 MB.

Su organización puede tener hasta 50 almacenes de datos. El tamaño combinado de estos almacenes de datos no puede superar el tamaño total del almacén de datos de su organización.

## Crear un almacén de datos en [!DNL Workfront Fusion]

* [Configuración del almacén de datos](#set-up-the-data-store)
* [Configuración de la estructura de datos](#set-up-the-data-structure)

### Configuración del almacén de datos

Para poder usar un almacén de datos en un módulo, debe crear el almacén de datos en [!DNL Workfront Fusion].

>[!NOTE]
>
>Su organización tiene un número limitado de almacenes de datos disponibles. Si intenta crear más almacenes de datos de los que tiene disponibles, [!DNL Workfront] devolverá un error [!UICONTROL Se alcanzó el número máximo de almacenes].
>
>Para obtener más información, consulte [Error alcanzado en el número máximo de tiendas](#maximum-stores-reached-error) en este artículo.

1. Inicie sesión en su cuenta de [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Almacenes de datos]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Agregar almacén de datos]** en la esquina superior derecha de la pantalla.
1. Introduzca la configuración del nuevo almacén de datos.

   Un título en negrita en un campo de un módulo [!DNL Workfront Fusion] indica que se requiere una configuración.

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
        <li> <p style="font-weight: bold;">Añadir una nueva estructura de datos</p> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para crear una nueva estructura de datos.</p> <p>Para obtener más información, consulte la sección <a href="#set-up-the-data-structure" class="MCXref xref">Configurar la estructura de datos</a> en este artículo.</p> </li> 
        <li style="font-weight: bold;"> <p>Deje el campo vacío.</p> <p style="font-weight: normal;">Si no selecciona ni añade una estructura de datos, la base de datos solo contendrá la clave principal. Este tipo de base de datos es útil si sólo desea guardar claves y sólo le interesa saber si existe o no una clave específica en la base de datos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Tamaño de almacenamiento de datos en MB]</p> </td> 
      <td> <p>Asigne el tamaño del almacén de datos desde el almacenamiento de datos interno total.</p> <p> El valor predeterminado es 10 MB. Si tiene menos de 10 MB de espacio de almacén de datos sin asignar de su asignación de 95 MB, el tamaño predeterminado es la cantidad de almacenamiento sin asignar.  <p>Nota: El importe reservado se puede cambiar en cualquier momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configuración de la estructura de datos

1. Al crear o editar un almacén de datos, haga clic en **[!UICONTROL Agregar]**.
1. En el cuadro **[!UICONTROL Agregar estructura de datos]** que aparece, configure los campos siguientes:

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
        <li> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong> para especificar manualmente las propiedades de una columna.</p> <p>Escriba <strong>[!UICONTROL Name]</strong> y <strong>[!UICONTROL Type]</strong> para la columna del almacén de datos y defina las propiedades correspondientes.</p> </li> 
        <li> <p>Haga clic en <strong>[!UICONTROL Generator]</strong> para determinar las columnas a partir de los datos de ejemplo proporcionados.</p> 
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
          <p>A continuación, puede agregar valores al almacén de datos manualmente o mediante los módulos del almacén de datos [!DNL Workfront Fusion].</p> 
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

Puede editar las propiedades y el contenido de un almacén de datos existente en el área [!UICONTROL Almacén de datos] de [!DNL Workfront Fusion].

* [Editar las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store)
* [Editar el contenido de un almacén de datos](#edit-the-contents-of-a-data-store)

### Editar las propiedades de un almacén de datos

Las propiedades de un almacén de datos incluyen la estructura de datos que utiliza el almacén de datos, así como el tamaño de éste.

1. Haga clic en **[!UICONTROL Almacén de datos]** ![](assets/data-store-icon.png) en el panel de navegación izquierdo para abrir el área de [!UICONTROL Almacén de datos].
1. Haga clic en **[!UICONTROL Editar]** ![](assets/data-store-edit.png) junto al almacén de datos que desee editar.
1. (Opcional) Si desea cambiar la estructura de datos utilizada por este almacén de datos a otra estructura de datos existente, selecciónela en la lista desplegable **[!UICONTROL Estructura de datos]**.

   O

   (Opcional) Si desea cambiar la estructura de datos usada por este almacén de datos a una estructura de datos completamente nueva, consulte [Configurar la estructura de datos](#set-up-the-data-structure) en este artículo.

1. (Opcional) Cambie el tamaño del almacén de datos introduciendo el nuevo tamaño en el campo **[!UICONTROL Tamaño de almacenamiento de datos en MB]**.
1. Haga clic en **[!UICONTROL Guardar]**.

### Editar el contenido de un almacén de datos

1. Haga clic en el icono **[!UICONTROL Almacén de datos]** ![](assets/data-store-icon.png) del panel de navegación izquierdo para abrir el área [!UICONTROL Almacén de datos].
1. Haga clic en **[!UICONTROL Examinar]** junto al almacén de datos que desea editar.
1. (Opcional) Reordene las columnas arrastrándolas a la ubicación deseada.
1. (Opcional) [!UICONTROL Edite] una sola celda haciendo clic en el icono **[!UICONTROL Editar]** de esa celda y, a continuación, introduciendo el valor deseado.
1. (Opcional) Agregue un nuevo elemento al almacén de datos haciendo clic en **[!UICONTROL Agregar]** y, a continuación, escribiendo la información del nuevo elemento.
1. Haga clic en **[!UICONTROL Guardar]**.

## Resolución de problemas

* [Restauración de datos perdidos de un almacén de datos](#restoring-lost-data-from-a-data-store)
* [Error de falta de espacio](#out-of-space-error)
* [Error de número máximo de tiendas alcanzado](#maximum-stores-reached-error)

### Restauración de datos perdidos de un almacén de datos

Actualmente no hay ninguna herramienta que pueda automatizar la restauración de los datos perdidos.

#### Solución

1. Examine todos los registros de ejecución de escenarios en los que se insertaron elementos en el almacén de datos.

   Para obtener más información sobre el examen de los registros de ejecución, vea [Ver el historial de ejecución de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copie los datos.
1. Vuelva a insertar los datos en el almacén de datos.

   Para obtener información sobre cómo insertar datos en un almacén de datos, consulte [Editar el contenido de un almacén de datos](#edit-the-contents-of-a-data-store) en este artículo.

### Error de [!UICONTROL espacio insuficiente]

Se produce un error de [!UICONTROL espacio insuficiente] porque ya se ha asignado el almacenamiento del almacén de datos asignado a los almacenes de datos creados anteriormente.

#### Solución

1. Edite cualquiera de los almacenes de datos existentes para utilizar menos espacio. Esto libera espacio para el nuevo almacén de datos.

   Para obtener más información, consulte [Editar las propiedades de un almacén de datos](#edit-the-properties-of-a-data-store) en este artículo.

>[!NOTE]
>
>Le recomendamos que no asigne todo su espacio a un único almacén de datos a menos que esté seguro de que no necesitará más almacenes de datos.

### Error [!UICONTROL Se alcanzó el máximo de tiendas]

Se produce el error [!UICONTROL Se alcanzó el número máximo de almacenes] porque su organización ha utilizado todos los almacenes de datos disponibles. Una organización tiene un número de almacenes de datos disponibles que equivale al doble del número de escenarios disponibles. Por lo tanto, el número total de almacenes de datos disponibles depende del plan que haya adquirido.

Por ejemplo, si su organización ha adquirido un plan con 15 escenarios, puede tener hasta 30 almacenes de datos.

#### Solución

Para reducir el número de almacenes de datos existentes, considere la posibilidad de realizar una de las siguientes acciones:

* Combinación de almacenes de datos existentes
* Eliminar almacenes de datos no utilizados
