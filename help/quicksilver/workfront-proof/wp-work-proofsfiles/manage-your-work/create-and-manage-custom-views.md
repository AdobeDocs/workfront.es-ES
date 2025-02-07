---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Crear y administrar vistas personalizadas en [!DNL Workfront Proof]
description: Es posible crear vistas personalizadas de los archivos y pruebas para enumerar los elementos que quiera de la forma en que desee que se muestren. También es posible exportar la información en vista personalizada como informe (en formato de archivo CSV con valores separados por comas).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 98%

---

# Creación y administración de vistas personalizadas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Es posible crear vistas personalizadas de los archivos y pruebas para enumerar los elementos que quiera de la forma en que desee que se muestren. También es posible exportar la información en vista personalizada como informe (en formato de archivo CSV con valores separados por comas).

>[!NOTE]
>
>Las vistas personalizadas solo están disponibles en los planes Select y Premium. Póngase en contacto con nuestro equipo de ventas para obtener una cotización.

## Creación de vistas personalizadas

Al crear una vista personalizada, se puede elegir:

* Si se incluirán pruebas, archivos o ambos
* Qué columnas se mostrarán
* Por qué columna ordenar
* El criterio de ordenación de la columna (ascendente o descendente)
* Qué tipos de filtros se utilizarán para determinar qué información se incluirá en la vista

Una vez creada la vista personalizada, estará disponible para su uso inmediato. El nombre de la nueva vista también se incluirá en el menú desplegable situado bajo el encabezado Mis vistas personalizadas (debajo de las vistas estándar).

Para crear una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.
1. Para obtener más información sobre las vistas, consulte [Administrar los elementos de la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Realice una de las siguientes acciones, en función de si desea crear una nueva vista personalizada desde cero o basada en una vista estándar existente:

   * Para crear una nueva vista personalizada basada en una vista estándar existente: en el menú desplegable, seleccione la vista estándar existente que quiera que sea la base de la nueva vista personalizada. Haga clic en el icono **[!UICONTROL Ver configuración]** y, a continuación, haga clic en **[!UICONTROL Copiar]** a la nueva vista personalizada.

   * ![Icono de vista personalizada](assets/proof-custom-view-icon.png)

   * Para crear una nueva vista personalizada desde cero: haga clic en el icono **[!UICONTROL Nueva vista]**.
   * ![Nueva vista](assets/proof-newview.png)

1. En la sección **[!UICONTROL Detalles]**, especifique la siguiente información:

   * **[!UICONTROL Nombre]** (obligatorio): El nombre de la nueva vista. Use un nombre único para que los usuarios puedan encontrar fácilmente la vista personalizada en el menú desplegable de Vistas.
   * **[!UICONTROL Elementos]**: seleccione si desea que las pruebas y el archivo, solo las pruebas o solo los archivos se incluyan en la vista. De forma predeterminada, se incluyen tanto las pruebas como los archivos.

1. En la sección **[!UICONTROL Columnas]**, determine las columnas que quiera incluir en la vista personalizada.

   1. Haga clic en el icono de flecha a la derecha.
   1. ![Flecha derecha](assets/proof-view-rightarrow.png)

   1. Haga doble clic en el nombre de la columna seleccionada.
   1. Es necesario seleccionar al menos una columna y cada columna solo se puede seleccionar una vez.
   1. Seleccione una columna del área **[!UICONTROL Columnas disponibles]** que quiera incluir en la nueva vista.
   1. Las columnas se moverán de la lista **[!UICONTROL Columnas disponibles]** a la lista **[!UICONTROL Columnas seleccionadas]**.

   1. Es posible seleccionar entre las columnas estándar o elegir que Campos personalizados y Motivos de la decisión sean columnas de la vista personalizada. (Si se configuraron en su cuenta, aparecerán en el área de la lista estándar de Columnas disponibles).
   1. Columnas estándar que se pueden incluir

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nombre de la fase activa</strong></td>   
      <td>Nombre de la fase activa del flujo de trabajo automatizado.</td>  
      </tr>  
      <tr>   
      <td><strong>Comentarios</strong></td>   
      <td>El número de comentarios recibidos.</td>
      </tr>  
      <tr>   
      <td><strong>Contador</strong></td>
      <td>Muestra un número de la prueba que se cargó en su cuenta (es necesario tener activada la opción de contador de pruebas en Configuración de la cuenta).</td>
      </tr>
      <tr>
      <td><strong>Creación</strong></td>
      <td>La fecha y la hora de creación del elemento.</td>
      </tr>
      <tr>
      <td><strong>Creador</strong></td>
      <td>El usuario que creó el elemento.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Date added to proof]</strong></td>
      <td>La fecha en la que se le añadió a la prueba. </td>
      </tr>
      <tr>
      <td><strong>Fecha límite</strong></td>
      <td>Fecha límite para toda la prueba.</td>
      </tr>
      <tr>
      <td><strong>Decisiones</strong></td>
      <td>Número de decisiones tomadas respecto al número esperado (por ejemplo: 0 de 1, 1 de 1, etc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Downloads]</strong></td>
      <td>Número de veces que se descargó el archivo original.</td>
      </tr>
      <tr>
      <td><strong>Nombre de archivo</strong></td>
      <td>Nombre del archivo o prueba.</td>
      </tr>
      <tr>
      <td><strong>Carpeta</strong></td>
      <td>Carpeta que contiene el elemento.</td>
      </tr>
      <tr>
      <td><strong>Última actividad</strong></td>
      <td>La fecha y la hora de la última actividad del elemento.</td>
      </tr>
      <tr>
      <td><strong>Última decisión sobre</strong></td>
      <td>La fecha y la hora de la última decisión tomada.</td>
      </tr>
      <tr>
      <td><strong>Mi fecha límite</strong></td>
      <td>Su propia fecha límite en las pruebas en las que se le añadió explícitamente como revisor o aprobador (si se aplica).</td>
      </tr>
      <tr>
      <td><strong>Propietario</strong></td>
      <td>El propietario del elemento.</td>
      </tr>
      <tr>
      <td><strong>País del propietario</strong></td>
      <td>El país registrado en el sistema del propietario de la prueba. </td>
      </tr>
      <tr>
      <td><strong>Prueba principal</strong></td>
      <td>Nombre de la prueba principal.</td>
      </tr>
      <tr>
      <td><strong>Progreso</strong></td>
      <td><p>Barra de progreso. Muestra las pruebas que aún no se han iniciado, abierto, comentado o de las que aún no se ha tomado una decisión.</p><p>Esta información no está ordenada.</p></td>
      </tr>
      <tr>
      <td><strong>Nombre de revisión</strong></td>
      <td>Nombre de la prueba.</td>
      </tr>
      <tr>
      <td><strong>Tipo de prueba</strong></td>
      <td><p>El tipo de prueba: archivo estático, página web estática, web interactiva (carga .zip), página web interactiva (https), vídeo, audio y otros. </p><p>Las pruebas combinadas se identifican como “Tipo de prueba combinada”. Tipo de archivo de la prueba.</p></td>
      </tr>
      <tr>
      <td><strong>Tamaño de archivo (MB)</strong></td>
      <td><p>Tamaño de archivo de la prueba en relación con la cuota de uso de disco.</p><p>Esta información se proporciona para la versión actual de la prueba. Si no hubiera ninguna versión actual, será para la más reciente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Fecha límite de fase activa</strong></p></td>
      <td>Fecha límite de las fases del flujo de trabajo automatizado.</td>
      </tr>
      <tr>
      <td><strong>Nombre de la fase</strong></td>
      <td>Nombre de cada fase del flujo de trabajo automatizado. Esto incluye las fases anteriores, las activas y las futuras.</td>
      </tr>
      <tr>
      <td><strong>Estado</strong></td>
      <td>Activo, Bloqueado, Borrador o Enviado.</td>
      </tr>
      <tr>
      <td><strong>Estado</strong></td>
      <td>Pendiente, Cambios necesarios, Aprobado con cambios, Aprobado o No relevante.</td>
      </tr>
      <tr>
      <td><strong>Etiquetas</strong></td>
      <td>Cualquier etiqueta adjunta al elemento.</td>
      </tr>
      <tr>
      <td><strong>Próximos nombres de fases</strong></td>
      <td> Nombre de cada fase que aún no se ha iniciado en el flujo de trabajo automatizado. </td>
      </tr>
      <tr>
      <td><strong>Contador de versiones</strong></td>
      <td> Número de versiones del elemento. </td>
      </tr>
      <tr>
      <td><strong>Número de versión de prueba</strong></td>
      <td><i>Número de versión de la prueba.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Opcional) Realice una de las acciones siguientes para mover la columna al área de **[!UICONTROL Columnas seleccionadas]** para que se incluya en la nueva vista:

      * Reordene las columnas de la lista **[!UICONTROL Columnas seleccionadas]**.
      * El orden en que se muestran las columnas en la lista **[!UICONTROL Columnas seleccionadas]** determina el orden en que se muestran las columnas en la vista personalizada.
      * Las columnas son visibles en la lista **[!UICONTROL Columnas seleccionadas]** en el orden en que las añadió desde la lista **[!UICONTROL Columnas disponibles]**.

      * Para reordenar una columna en la lista **[!UICONTROL Columnas seleccionadas]**, seleccione el nombre de la columna y arrástrela hacia arriba o hacia abajo en la lista.

      * Elimine una columna de la lista **[!UICONTROL Columnas seleccionadas]**, haga clic en el nombre de la columna seleccionada y, a continuación, en la flecha **[!UICONTROL Izquierda]**. También puede hacer doble clic en el nombre de la columna seleccionada (la columna se mueve de nuevo a la lista **[!UICONTROL Columnas disponibles]**).

      * Una columna sólo puede añadirse una vez. Por ejemplo, si mueve la columna Comentarios de [!UICONTROL Disponibles] a la lista [!UICONTROL Columnas seleccionadas], el nombre de esta columna desaparecerá de la lista [!UICONTROL Columnas disponibles].

1. En la sección **[!UICONTROL Ordenar]**, especifique la siguiente información:

   * **Ordenar por:** Utilice la pestaña [!UICONTROL Ordenar] si desea establecer un orden concreto en el que se enumeran los elementos en su vista personalizada. Si no selecciona una columna para la ordenación, el valor predeterminado es Sin columna, es decir, sin columna de ordenación especial ni orden.
   * Solamente las columnas seleccionadas en la pestaña [!UICONTROL Columnas] se incluyen en la lista desplegable [!UICONTROL Ordenar por columna].
   * **Ascendente o descendente:** seleccione si desea ordenar la columna de forma ascendente o descendente por defecto.

1. Utilice la sección **[!UICONTROL Filtros]** para definir uno o más criterios de selección de elementos que desea incluir en la vista personalizada. Los filtros son especialmente útiles si desea utilizar su vista personalizada como un informe.
1. Para incluir todos los elementos en la vista personalizada, omita la sección **[!UICONTROL Filtros]**.
1. Filtros disponibles:

   * **Campo:** Seleccione el campo para este filtro (Comentarios es el campo predeterminado). La lista Campo contiene todos los campos Estándar (como en la ficha [!UICONTROL Columnas]). La lista no se limita a las columnas seleccionadas para su visualización.
   * **Operador:** Los operadores disponibles para el filtro dependen del tipo de campo seleccionado. Seleccione un operador que muestre la relación entre el campo y el campo de valor. Rellenará esta información más adelante.
   * **Valor:** seleccione o escriba el valor elegido en este campo, según el campo y el operador que haya seleccionado. Según el operador que haya elegido, puede haber un campo valor o dos o ninguno. Consulte los ejemplos siguientes.
   * **Los filtros se aplican utilizando la siguiente lógica:** los criterios de filtrado entre diferentes campos utilizarán el operador AND. Si varios criterios de filtro utilizan el mismo campo, se utilizará el operador OR para el mismo campo.

     Si desea ver solo pruebas con cero comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Igual a
      * Campo de valor: 0

     Si desea ver solamente las pruebas con dos o más comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Mayor o igual que
      * Campo de valor: 2

     Si desea ver solo pruebas con entre 1 y 4 comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Entre
      * Campo de valor (primer campo): 1
      * Campo de valor (segundo campo): 4

        Puede cambiar sin problemas un filtro que haya añadido a su vista personalizada o eliminarlo haciendo clic en el icono de la cruz situado junto al filtro [!UICONTROL configurar] si es necesario.

        Dado que la lista Campo no se limita a las columnas que seleccionó en la pestaña [!UICONTROL Columnas], tenga cuidado al crear un filtro que incluya una columna que no seleccionó para su visualización en la vista personalizada. Por ejemplo, el siguiente filtro para la vista seleccionará todas las pruebas con un valor de contador de versiones igual o superior a 2:

         * Campo = Contador de versión
         * Operador = Mayor o igual que
         * Campo de valor = 2

           >[!NOTE]
           >
           >Puede cambiar sin problemas un filtro que haya añadido a su vista personalizada o eliminarlo haciendo clic en el icono de la cruz situado junto al filtro [!UICONTROL configurar] si es necesario.



1. En la sección **[!UICONTROL Compartir]**, seleccione qué usuarios de su cuenta podrán ver la vista personalizada.
1. Las vistas personalizadas son específicas del usuario que las crea. Por defecto, la nueva vista personalizada solamente es visible para su creador; sin embargo, puede optar por compartir su vista personalizada eligiendo una de las siguientes opciones:

   * **Solo usted puede ver esta vista personalizada** (predeterminada): seleccione esta opción si desea que la vista personalizada esté disponible solamente para usted.
   * **Todos los usuarios pueden ver esta vista personalizada**: seleccione esta opción para que la vista personalizada esté disponible para todos los usuarios de su cuenta.
   * **Seleccionar usuarios que pueden ver esta vista personalizada**: seleccione esta opción para que la vista personalizada solo esté disponible para usuarios específicos.
   * Comience a escribir el nombre o la dirección de correo electrónico del usuario que desea que tenga acceso a la vista personalizada y, a continuación, haga clic sobre el nombre cuando aparezca en la lista.
   * Si decide no compartir la vista con otros usuarios en este momento, puede hacerlo más tarde editando la vista personalizada.

1. Haga clic en **[!UICONTROL Crear]**.
1. La vista personalizada se muestra y está disponible en la página [!DNL Views]. Para obtener más información sobre las vistas, consulte [Administrar elementos en la [!DNL Views] página en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Edición de vistas personalizadas

Puede editar una vista personalizada fácilmente. Para editar una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el botón [!UICONTROL Vistas] (1)
1. Seleccione la vista que desee editar en el menú desplegable.\
   ![Editar vista](assets/proof-view-edit.png)

1. Haga clic en el botón **[!UICONTROL Opciones de vista]** y luego haga clic en **[!UICONTROL Editar vista]**.\
   ![Ver opciones](assets/proof-view-options.png)\
   Se muestra la página Editar vista personalizada.

1. Haga clic en el menú [!UICONTROL Acciones]. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.
1. Seleccione [!UICONTROL Editar vista] en el menú. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. Se muestra la página Editar vista personalizada.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Si edita la vista personalizada, las columnas de la lista Columnas seleccionadas se ordenarán en orden alfabético automáticamente. Deberá reorganizarlos si es necesario antes de actualizar la vista.


## Copia de vistas personalizadas

La función de vista Copiar permite realizar fácilmente una copia de una vista personalizada existente. Esto es realmente útil, por ejemplo, si desea configurar vistas separadas para todos sus diseñadores, siendo cada vista la misma excepto por el propietario de la prueba (diseñador).

Para copiar una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el botón **[!UICONTROL Vistas]**. (1)
1. Seleccione la vista personalizada de la lista. (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Copiar] en el menú. (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. En la página Copiar vista personalizada, se rellenan todos los ajustes originales. Modifique la vista personalizada según su elección y haga clic en el botón **[!UICONTROL Copiar vista]**. Se le llevará a la nueva vista inmediatamente.\
   ![Copiar vista personalizada](assets/copy-custom-view-page-350x542.png)

## Uso compartido de vistas personalizadas

La función compartir vista permite compartir una vista con otros usuarios de la cuenta si aún no los ha seleccionado en la sección Compartir para la vista. Cuando comparte una vista personalizada con otros usuarios, la vista aparece en su sección [!UICONTROL Mis vistas personalizadas] del menú desplegable Vistas.

Para compartir una vista personalizada con otros usuarios:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el botón **[!UICONTROL Vistas]** (1)
1. Seleccione la vista personalizada de la lista (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Compartir vista] en el menú (4)
1. Aparecerá la página Editar vista personalizada.
1. En la sección [!UICONTROL Compartir] elige los usuarios con los que quieres compartir la vista y haga clic en **[!UICONTROL Actualizar vista]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportación de vistas personalizadas a archivos CSV

Para exportar los datos de una vista personalizada a un archivo CSV:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el botón **[!UICONTROL Vistas]**. (1)
1. Seleccione la vista personalizada de la lista. (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Exportar a CSV] en el menú. (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   En otra ventana del explorador aparece “Generando informe: 100 %” aparece más el número de registros (el número de elementos incluidos en el informe desde su vista personalizada)

1. (Condicional) Si aparece un mensaje de seguridad indicando que la descarga del informe está actualmente bloqueada, haga clic para permitir que la descarga continúe.
1. Haga clic en **[!UICONTROL Guardar]** cuando aparezca la ventana Descarga de archivos preguntándole si desea abrir o guardar el archivo.
1. Seleccione una ubicación en su ordenador y guarde el archivo.

## Eliminación de vistas personalizadas

Puede eliminar una vista personalizada fácilmente. Para ello:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el botón **[!UICONTROL Vistas]**.
1. Seleccione la vista personalizada de la lista
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Eliminar] en el menú. (4)\
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Haga clic en **[!UICONTROL Eliminar]** (5) para confirmar que desea eliminar la vista personalizada actual\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. Se muestra la vista predeterminada todos los elementos y la vista personalizada eliminada ya no aparece en el menú desplegable **[!UICONTROL Vistas]**.
