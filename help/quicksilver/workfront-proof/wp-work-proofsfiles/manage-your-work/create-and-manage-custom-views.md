---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Crear y administrar vistas personalizadas en  [!DNL Workfront Proof]
description: Puede crear vistas personalizadas de sus archivos y pruebas para enumerar los elementos que desee de la forma en que desea que se muestren. También puede exportar la información en la vista personalizada como un informe (en formato CSV, valor separado por comas, formato de archivo).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2458'
ht-degree: 0%

---

# Crear y administrar vistas personalizadas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Puede crear vistas personalizadas de sus archivos y pruebas para enumerar los elementos que desee de la forma en que desea que se muestren. También puede exportar la información en la vista personalizada como un informe (en formato CSV, valor separado por comas, formato de archivo).

>[!NOTE]
>
>Las vistas personalizadas solo están disponibles en los planes Select y Premium. Póngase en contacto con nuestro equipo de ventas para obtener una cotización.

## Creación de una vista personalizada

Al crear una vista personalizada, puede elegir:

* Si se incluyen pruebas, archivos o ambos
* Qué columnas se muestran
* Por qué columna ordenar
* El criterio de ordenación de la columna (ascendente o descendente)
* Tipos de filtros que se utilizarán para determinar qué información se incluye en la vista

Una vez creada la vista personalizada, está disponible para usar inmediatamente. El nombre de la nueva vista también se incluye en el menú desplegable bajo el encabezado Mis vistas personalizadas (debajo de las vistas Estándar).

Para crear una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.
1. Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Realice una de las siguientes acciones, en función de si desea crear una nueva vista personalizada desde cero o una nueva vista personalizada basada en una vista estándar existente:

   * Para crear una nueva vista personalizada basada en una vista estándar existente: en el menú desplegable, seleccione la vista estándar existente que desee utilizar como base para la nueva vista personalizada. Haga clic en el icono **[!UICONTROL Ver configuración]** y, a continuación, haga clic en **[!UICONTROL Copiar]** a la nueva vista personalizada.

   * ![](assets/proof-custom-view-icon.png)

   * Para crear una nueva vista personalizada desde cero: haga clic en el icono **[!UICONTROL Nueva vista]**.
   * ![](assets/proof-newview.png)

1. En la sección **[!UICONTROL Detalles]**, especifique la siguiente información:

   * **[!UICONTROL Nombre]** (obligatorio): El nombre de la nueva vista. Utilice un nombre único para que los usuarios puedan encontrar fácilmente la vista personalizada en el menú desplegable de Vistas.
   * **[!UICONTROL Elementos]**: seleccione si desea que las pruebas y el archivo, solo las pruebas o solo los archivos se incluyan en la vista. De forma predeterminada, se incluyen tanto las pruebas como los archivos.

1. En la sección **[!UICONTROL Columnas]**, determine qué columnas desea incluir en la vista personalizada.

   1. Haga clic en el icono de flecha derecha.
   1. ![](assets/proof-view-rightarrow.png)

   1. Haga doble clic en el nombre de la columna seleccionada.
   1. Debe seleccionar al menos una columna y se puede agregar una columna solo una vez.
   1. Seleccione una columna del área **[!UICONTROL Columnas disponibles]** que desee incluir en la nueva vista.
   1. Las columnas se mueven de la lista **[!UICONTROL Columnas disponibles]** a la lista **[!UICONTROL Columnas seleccionadas]**.

   1. Puede seleccionar entre las columnas estándar o elegir Campos personalizados y Motivos de decisión para que sean columnas en la vista personalizada. (Si los tiene configurados en su cuenta, aparecen en el área de la lista estándar de Columnas disponibles ).
   1. Columnas estándar que puede incluir

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nombre de etapa activo</strong></td>   
      <td>Nombre de la etapa activa en el flujo de trabajo automatizado.</td>  
      </tr>  
      <tr>   
      <td><strong>Comentarios</strong></td>   
      <td>El número de comentarios recibidos.</td>
      </tr>  
      <tr>   
      <td><strong>Contador</strong></td>
      <td>Muestra un número de la prueba que se ha cargado en su cuenta (debe tener activada la opción de contador de pruebas en Configuración de la cuenta).</td>
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
      <td><strong>[!UICONTROL Fecha de incorporación a la prueba]</strong></td>
      <td>La fecha en la que se le añadió a la prueba. </td>
      </tr>
      <tr>
      <td><strong>Fecha límite</strong></td>
      <td>El plazo para toda la prueba.</td>
      </tr>
      <tr>
      <td><strong>Decisiones</strong></td>
      <td>El número de decisiones tomadas del número esperado (p. ej. 0 de 1, 1 de 1, etc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Descargas]</strong></td>
      <td>El número de veces que se ha descargado el archivo original.</td>
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
      <td>La fecha y hora de la última decisión tomada.</td>
      </tr>
      <tr>
      <td><strong>Mi fecha límite</strong></td>
      <td>Su propia fecha límite en las pruebas en las que se le añade explícitamente como revisor/aprobador (si se aplica).</td>
      </tr>
      <tr>
      <td><strong>Propietario</strong></td>
      <td>El propietario del artículo.</td>
      </tr>
      <tr>
      <td><strong>País del propietario</strong></td>
      <td>El país registrado en el sistema para el propietario de la prueba. </td>
      </tr>
      <tr>
      <td><strong>Prueba principal</strong></td>
      <td>Nombre de la prueba principal.</td>
      </tr>
      <tr>
      <td><strong>Progreso</strong></td>
      <td><p>Barra de progreso. Muestra las pruebas que aún no se han iniciado, abierto, comentado o tomado una decisión sobre ellas.</p><p>Esta información no está ordenada según.</p></td>
      </tr>
      <tr>
      <td><strong>Nombre de revisión</strong></td>
      <td>Nombre de la prueba.</td>
      </tr>
      <tr>
      <td><strong>Tipo de prueba</strong></td>
      <td><p>El tipo de prueba: archivo estático, página web estática, web interactiva (.zip upload), página web interactiva (https), vídeo, audio y otro. </p><p>Las pruebas combinadas se identifican como "Tipo de prueba combinado". Tipo de archivo de la prueba.</p></td>
      </tr>
      <tr>
      <td><strong>Tamaño de archivo (MB)</strong></td>
      <td><p>Tamaño de archivo de la prueba en relación con la cuota de uso de disco.</p><p>Esta información se proporciona para la versión actual de la prueba. Si no hay ninguna versión actual, es para la más reciente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Plazo de fase activo</strong></p></td>
      <td>Plazo de las fases del flujo de trabajo automatizado.</td>
      </tr>
      <tr>
      <td><strong>Nombre del escenario</strong></td>
      <td>Nombre de cada fase del flujo de trabajo automatizado. Esto incluye las etapas anteriores, las etapas activas y las etapas futuras.</td>
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
      <td>Las etiquetas adjuntas al elemento.</td>
      </tr>
      <tr>
      <td><strong>Próximos nombres de fase</strong></td>
      <td> Nombre de cada fase que aún no se ha iniciado en el flujo de trabajo automatizado. </td>
      </tr>
      <tr>
      <td><strong>Contador de versiones</strong></td>
      <td> Número de versiones del elemento. </td>
      </tr>
      <tr>
      <td><strong>Número de versión de revisión</strong></td>
      <td><i>Número de versión de la revisión.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Opcional) Realice una de las acciones siguientes para mover la columna al área de **[!UICONTROL Columnas seleccionadas]** para que se incluya en la nueva vista:

      * Reordene las columnas de la lista **[!UICONTROL Columnas seleccionadas]**.
      * El orden en que se muestran las columnas en la lista **[!UICONTROL Columnas seleccionadas]** determina el orden en que se muestran las columnas en la vista personalizada.
      * Las columnas están visibles en la lista **[!UICONTROL Columnas seleccionadas]** en el orden en que las agregó desde la lista **[!UICONTROL Columnas disponibles]**.

      * Para reordenar una columna en la lista **[!UICONTROL Columnas seleccionadas]**, seleccione el nombre de la columna y arrástrela hacia arriba o hacia abajo en la lista.

      * Elimine una columna de la lista **[!UICONTROL Columnas seleccionadas]**, haciendo clic en el nombre de la columna seleccionada y, a continuación, haciendo clic en la flecha **[!UICONTROL Izquierda]**. También puede hacer doble clic en el nombre de la columna seleccionada (la columna se mueve de nuevo a la lista **[!UICONTROL Columnas disponibles]**).

      * Las columnas solo se pueden agregar una vez. Por ejemplo, si mueve la columna Comentarios de la lista [!UICONTROL Available] a [!UICONTROL Selected columns], el nombre de esta columna desaparecerá de la lista [!UICONTROL Available columns].

1. En la sección **[!UICONTROL Sorting]**, especifique la siguiente información:

   * **Ordenar por:** Utilice la ficha [!UICONTROL Ordenar] si desea establecer un orden determinado en el que los elementos se enumeran en la vista personalizada. Si no selecciona una columna para ordenar, el valor predeterminado es Ninguna columna, es decir, ninguna columna o orden especial.
   * En la lista desplegable [!UICONTROL Ordenar por columna] solo se incluyen las columnas que seleccionó en la ficha [!UICONTROL Columnas].
   * **Ascendente o Descendente:** Seleccione si desea ordenar la columna de forma ascendente o descendente de forma predeterminada.

1. Utilice la sección **[!UICONTROL Filtros]** para definir uno o más criterios de selección de elementos que desea incluir en la vista personalizada. Los filtros son especialmente útiles si desea utilizar la vista personalizada como informe.
1. Para incluir todos los elementos en la vista personalizada, omita la sección **[!UICONTROL Filtros]**.
1. Filtros disponibles:

   * **Campo:** Seleccione el campo para este filtro (Comentarios es el campo predeterminado). La lista Campo contiene todos los campos Estándar (como en la ficha [!UICONTROL Columnas]). La lista no se limita a las columnas seleccionadas para su visualización.
   * **Operador:** Los operadores disponibles para el filtro dependen del tipo de campo seleccionado. Seleccione un Operador que muestre la relación entre el campo Field y el campo value. Rellenará esta información más adelante.
   * **Valor:** Seleccione o escriba el valor elegido en este campo, según el campo y el Operador que haya seleccionado. Según el Operador que haya elegido, puede haber un campo Valor o dos o ninguno. Consulte los ejemplos siguientes.
   * **Los filtros se aplican según la siguiente lógica:** Los criterios de filtro entre los distintos campos utilizarán el operador AND. Si varios criterios de filtro utilizan el mismo campo, se utilizará el operador OR para el mismo campo.

     Si desea ver solo pruebas con cero comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Es igual a
      * Campo de valor: 0

     Si desea ver solo pruebas con dos o más comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Mayor o igual que
      * Campo de valor: 2

     Si desea ver solo pruebas con entre 1 y 4 comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Entre
      * Campo de valor (primer campo): 1
      * Campo de valor (segundo campo): 4

        Puede cambiar un filtro que haya agregado a la vista personalizada sin problemas o eliminarlo haciendo clic en el icono cruzado situado junto al filtro [!UICONTROL setup] si es necesario.

        Dado que la lista Campo no se limita a las columnas seleccionadas en la ficha [!UICONTROL Columnas], tenga cuidado al crear un filtro que incluya una columna que no seleccionó para mostrarla en la vista personalizada. Por ejemplo, el siguiente filtro para la vista seleccionará todas las pruebas con un valor de contador de versión de 2 o más:

         * Campo = Contador de versión
         * Operador = Mayor o igual que
         * Campo de valor = 2

           >[!NOTE]
           >
           >Puede cambiar un filtro que haya agregado a la vista personalizada sin problemas o eliminarlo haciendo clic en el icono cruzado situado junto al filtro [!UICONTROL setup] si es necesario.



1. En la sección **[!UICONTROL Compartir]**, seleccione qué usuarios de su cuenta podrán ver la vista personalizada.
1. Las vistas personalizadas son específicas del usuario que las crea. De forma predeterminada, la nueva vista personalizada solo está visible para su creador; sin embargo, puede elegir compartir la vista personalizada eligiendo una de las siguientes opciones:

   * **Solo usted puede ver esta vista personalizada** (predeterminada): seleccione esta opción si desea que la vista personalizada esté disponible solamente para usted.
   * **Todos los usuarios pueden ver esta vista personalizada**: seleccione esta opción para que la vista personalizada esté disponible para todos los usuarios de su cuenta.
   * **Seleccionar usuarios que pueden ver esta vista personalizada**: seleccione esta opción para que la vista personalizada solo esté disponible para usuarios específicos.
   * Comience a escribir el nombre o la dirección de correo electrónico del usuario al que desea tener acceso a la vista personalizada y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
   * Si decide no compartir la vista con otros usuarios en este momento, puede hacerlo más tarde editando la vista personalizada.

1. Haga clic en **[!UICONTROL Crear]**.
1. La vista personalizada se muestra y está disponible en la página [!DNL Views]. Para obtener más información sobre las vistas, consulte [Administrar elementos en la [!DNL Views] página en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Edición de vistas personalizadas

Puede editar una vista personalizada fácilmente. Para editar una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haz clic en el botón [!UICONTROL Vistas] (1)
1. Seleccione la vista que desee editar en el menú desplegable.\
   ![](assets/proof-view-edit.png)

1. Haga clic en el botón **[!UICONTROL Opciones de vista]** y luego haga clic en **[!UICONTROL Editar vista]**.\
   ![](assets/proof-view-options.png)\
   Se muestra la página Editar vista personalizada.

1. Haga clic en el menú [!UICONTROL Acciones]. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.
1. Seleccione [!UICONTROL Editar vista] en el menú. (4) \
   ![editando_vista_personalizada_2.png](assets/editing-custom-view-2-350x258.png)

1. Se muestra la página Editar vista personalizada.

![Editar_página_vista_personalizada.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Si edita la vista personalizada, las columnas de la lista Columnas seleccionadas se ordenarán en orden alfabético automáticamente. Deberá reorganizarlos si es necesario antes de actualizar la vista.


## Copia de vistas personalizadas

La función de vista Copiar permite realizar fácilmente una copia de una vista personalizada existente. Esto resulta muy útil, por ejemplo, si desea configurar vistas independientes para todos los diseñadores y cada vista es la misma excepto para el propietario de la prueba (diseñador).

Para copiar una vista personalizada:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haz clic en el botón **[!UICONTROL Vistas]**. (1)
1. Seleccione la vista personalizada de la lista. (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Copiar] en el menú. (4)\
   ![copiar_vista_personalizada.png](assets/copying-custom-view-350x258.png)

1. En la página Copiar vista personalizada, se rellenan todos los ajustes originales. Modifique la vista personalizada según su elección y haga clic en el botón **[!UICONTROL Copiar vista]**. Se le llevará a la nueva vista inmediatamente.\
   ![](assets/copy-custom-view-page-350x542.png)

## Uso compartido de vistas personalizadas

La función Compartir vista permite compartir una vista con otros usuarios de la cuenta si aún no los ha seleccionado en la sección Compartir para la vista. Cuando comparte una vista personalizada con otros usuarios, la vista aparece en su sección [!UICONTROL Mis vistas personalizadas] del menú desplegable Vistas.

Para compartir una vista personalizada con otros usuarios:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haz clic en el botón **[!UICONTROL Vistas]** (1)
1. Seleccione su Vista personalizada de la lista (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Compartir vista] en el menú (4)
1. Aparecerá la página Editar vista personalizada.
1. En la sección [!UICONTROL Compartir], seleccione los usuarios con los que desea compartir la vista y haga clic en **[!UICONTROL Actualizar vista]**.

   ![Editar_página_vista_personalizada__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportación de vistas personalizadas a archivos CSV

Para exportar los datos de una vista personalizada a un archivo CSV:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haz clic en el botón **[!UICONTROL Vistas]**. (1)
1. Seleccione la vista personalizada de la lista. (2)
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Exportar a CSV] en el menú. (4)\
   ![exportar_vista_personalizada.png](assets/exporting-custom-view-350x258.png)\
   En una ventana independiente del explorador, aparecerá &quot;Generando informe: 100 %&quot; más el número de registros (el número de elementos incluidos en el informe desde la vista personalizada)

1. (Condicional) Si aparece un mensaje de seguridad que indica que la descarga del informe está bloqueada actualmente, haga clic en para permitir que continúe la descarga.
1. Haga clic en **[!UICONTROL Guardar]** cuando aparezca la ventana Descarga de archivos preguntándole si desea abrir o guardar el archivo.
1. Seleccione una ubicación en el equipo y guarde el archivo.

## Eliminación de vistas personalizadas

Puede eliminar una vista personalizada fácilmente. Para ello:

1. Vaya a la página **[!UICONTROL Vistas]**.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haz clic en el botón **[!UICONTROL Vistas]**.
1. Seleccione la vista personalizada de la lista
1. Haga clic en el menú **[!UICONTROL Acciones]**. (3)\
   Este botón solo está disponible si incluye la columna Nombre de la prueba en la vista.

1. Seleccione [!UICONTROL Eliminar] en el menú. (4)\
   ![eliminando_vista_personalizada.png](assets/deleting-custom-view-350x258.png)

1. Haga clic en **[!UICONTROL Eliminar]** (5) para confirmar que desea eliminar la vista personalizada actual\
   ![eliminar__1_.png](assets/delete--1--350x187.png)

1. Se mostrará la vista predeterminada Todos los elementos y la vista personalizada eliminada dejará de aparecer en el menú desplegable **[!UICONTROL Vistas]**.
