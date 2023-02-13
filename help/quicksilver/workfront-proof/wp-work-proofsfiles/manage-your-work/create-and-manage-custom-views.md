---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Crear y administrar vistas personalizadas en [!DNL Workfront Proof]
description: Puede crear vistas personalizadas de sus archivos y pruebas para enumerar los elementos que desee de la forma en que desea que se muestren. También puede exportar la información en la vista personalizada como un informe (en CSV, valores separados por comas, formato de archivo).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2457'
ht-degree: 1%

---

# Crear y administrar vistas personalizadas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Puede crear vistas personalizadas de sus archivos y pruebas para enumerar los elementos que desee de la forma en que desea que se muestren. También puede exportar la información en la vista personalizada como un informe (en CSV, valores separados por comas, formato de archivo).

>[!NOTE]
>
>Las vistas personalizadas solo están disponibles en los planes Select y Premium. Póngase en contacto con nuestro equipo de ventas para obtener un presupuesto.

## Creación de una vista personalizada

Al crear una vista personalizada, puede elegir:

* Si se incluyen pruebas, archivos o ambos
* Qué columnas se muestran
* Qué columna ordenar por
* El orden de la columna (ascendente o descendente)
* Qué tipos de filtros utilizar para determinar qué información se incluye en la vista

Una vez creada la vista personalizada, está disponible para su uso inmediato. El nombre de la nueva vista también se incluye en el menú desplegable bajo el encabezado Mis vistas personalizadas (debajo de las vistas Estándar).

Para crear una vista personalizada:

1. Vaya a la **[!UICONTROL Vistas]** página.
1. Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Realice una de las siguientes acciones, en función de si desea crear una nueva vista personalizada desde cero o crear una nueva vista personalizada basada en una vista estándar existente:

   * Para crear una nueva vista personalizada basada en una vista estándar existente: En el menú desplegable, seleccione la vista estándar existente que desee utilizar como base para la nueva vista personalizada. Haga clic en el **[!UICONTROL Configuración de vista]** y, a continuación, haga clic en **[!UICONTROL Copiar]** a la nueva vista personalizada.

   * ![](assets/proof-custom-view-icon.png)

   * Para crear una nueva vista personalizada desde cero: Haga clic en el **[!UICONTROL Nueva vista]** icono.
   * ![](assets/proof-newview.png)

1. En el **[!UICONTROL Detalles]** especifique la siguiente información:

   * **[!UICONTROL Nombre]** (obligatorio): Nombre de la nueva vista. Utilice un nombre único para que los usuarios puedan encontrar fácilmente la vista personalizada en el menú desplegable de las Vistas.
   * **[!UICONTROL Elementos]**: Seleccione si desea que las pruebas y el archivo, solo las pruebas o los archivos solo se incluyan en la vista. De forma predeterminada, se incluyen pruebas y archivos.

1. En el **[!UICONTROL Columnas]** , determine qué columnas desea incluir en la vista personalizada.

   1. Haga clic en el icono de flecha derecha .
   1. ![](assets/proof-view-rightarrow.png)

   1. Haga doble clic en el nombre de la columna seleccionada.
   1. Debe seleccionar al menos una columna y esta solo se puede agregar una vez.
   1. Seleccione una columna de la **[!UICONTROL Columnas disponibles]** área que desea incluir en la nueva vista.
   1. Las columnas se mueven desde el **[!UICONTROL Columnas disponibles]** a **[!UICONTROL Columnas seleccionadas]** lista.

   1. Puede seleccionar entre las columnas estándar o elegir los campos personalizados y los motivos de decisión como columnas en la vista personalizada. (Si los ha configurado en su cuenta, aparecerán en el área de la lista estándar de columnas disponibles ).
   1. Columnas estándar que puede incluir

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nombre del escenario activo</strong></td>   
      <td>Nombre del paso activo en el flujo de trabajo automatizado.</td>  
      </tr>  
      <tr>   
      <td><strong>Comentarios</strong></td>   
      <td>Número de observaciones recibidas.</td>
      </tr>  
      <tr>   
      <td><strong>Contador</strong></td>
      <td>Muestra una serie de pruebas que se han cargado en la cuenta (tiene que tener una opción de contador de prueba habilitada en Configuración de cuenta).</td>
      </tr>
      <tr>
      <td><strong>Creación</strong></td>
      <td>La fecha y hora en que se creó el elemento.</td>
      </tr>
      <tr>
      <td><strong>Creador</strong></td>
      <td>El usuario que creó el elemento.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Fecha añadida a la prueba]</strong></td>
      <td>La fecha en la que se agregó a la prueba. </td>
      </tr>
      <tr>
      <td><strong>Fecha límite</strong></td>
      <td>Plazo para toda la prueba.</td>
      </tr>
      <tr>
      <td><strong>Decisiones</strong></td>
      <td>El número de decisiones tomadas del número previsto (por ejemplo, 0 de 1, 1 de 1, etc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Descargas]</strong></td>
      <td>Número de veces que se ha descargado el archivo original.</td>
      </tr>
      <tr>
      <td><strong>Nombre de archivo</strong></td>
      <td>Nombre del archivo o prueba.</td>
      </tr>
      <tr>
      <td><strong>Carpeta</strong></td>
      <td>La carpeta que contiene el elemento.</td>
      </tr>
      <tr>
      <td><strong>Última actividad</strong></td>
      <td>La fecha y hora de la última actividad del elemento.</td>
      </tr>
      <tr>
      <td><strong>Última decisión sobre</strong></td>
      <td>La fecha y hora de la última decisión adoptada.</td>
      </tr>
      <tr>
      <td><strong>Mi fecha límite</strong></td>
      <td>Su propia fecha límite en las pruebas en las que se le agrega explícitamente como revisor/aprobador (si se aplica).</td>
      </tr>
      <tr>
      <td><strong>Propietario</strong></td>
      <td>El propietario del artículo.</td>
      </tr>
      <tr>
      <td><strong>País propietario</strong></td>
      <td>El país inscrito en el sistema para el propietario de la prueba. </td>
      </tr>
      <tr>
      <td><strong>Prueba principal</strong></td>
      <td>Nombre de la prueba principal.</td>
      </tr>
      <tr>
      <td><strong>Progreso</strong></td>
      <td><p>Barra de progreso. Muestra pruebas que aún no están iniciadas, abiertas, comentadas o decididas.</p><p>Esta información no está ordenada.</p></td>
      </tr>
      <tr>
      <td><strong>Nombre de revisión</strong></td>
      <td>Nombre de la prueba.</td>
      </tr>
      <tr>
      <td><strong>Tipo de prueba</strong></td>
      <td><p>Tipo de prueba: Archivo estático, página web estática, web interactiva (carga .zip), página web interactiva (https), vídeo, audio y otros. </p><p>Las pruebas combinadas se identifican como "Tipo de prueba combinado". Tipo de archivo de la prueba.</p></td>
      </tr>
      <tr>
      <td><strong>Tamaño del archivo (MB)</strong></td>
      <td><p>Tamaño de archivo de la prueba en relación con la cuota de uso del disco.</p><p>Esta información se proporciona para la versión actual de la prueba. Si no hay ninguna versión actual, es para la versión más reciente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Plazo de etapa activa</strong></p></td>
      <td>Plazo de etapas en el flujo de trabajo automatizado.</td>
      </tr>
      <tr>
      <td><strong>Nombre del escenario</strong></td>
      <td>Nombre de cada fase del flujo de trabajo automatizado. Esto incluye etapas pasadas, etapas activas y etapas futuras.</td>
      </tr>
      <tr>
      <td><strong>Estado</strong></td>
      <td>Activo, Bloqueado, Borrador o Enviado.</td>
      </tr>
      <tr>
      <td><strong>Estado</strong></td>
      <td>Pendiente, cambios necesarios, aprobado con cambios, aprobado o no relevante.</td>
      </tr>
      <tr>
      <td><strong>Etiquetas</strong></td>
      <td>Cualquier etiqueta adjunta al elemento.</td>
      </tr>
      <tr>
      <td><strong>Próximos nombres de escenario</strong></td>
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

   1. (Opcional) Realice una de las siguientes acciones para mover la columna a la **[!UICONTROL Columnas seleccionadas]** para que se incluya en la nueva vista:

      * Reordenar las columnas en la variable **[!UICONTROL Columnas seleccionadas]** lista.
      * El orden en el que se muestran las columnas en la variable **[!UICONTROL Columnas seleccionadas]** determina el orden en que se muestran las columnas en la vista personalizada.
      * Las columnas se pueden ver en la sección **[!UICONTROL Columnas seleccionadas]** en el orden en el que las agregó desde la **[!UICONTROL Columnas disponibles]** lista.

      * Para reordenar una columna en el **[!UICONTROL Columnas seleccionadas]** , seleccione el nombre de la columna y arrástrela hacia arriba o hacia abajo en la lista.

      * Elimine una columna de la función **[!UICONTROL Columnas seleccionadas]** , haga clic en el nombre de la columna seleccionada y, a continuación, haga clic en la **[!UICONTROL Left]** flecha. También puede hacer doble clic en el nombre de la columna seleccionada (la columna se mueve de nuevo al **[!UICONTROL Columnas disponibles]** ).

      * Una columna solo se puede agregar una vez. Por ejemplo, si mueve la columna Comentarios de [!UICONTROL Disponible] a [!UICONTROL Columnas seleccionadas] , el nombre de esta columna desaparecerá de [!UICONTROL Columnas disponibles] lista.

1. En el **[!UICONTROL Ordenar]** especifique la siguiente información:

   * **Ordenar por:** Utilice la variable [!UICONTROL Ordenar] si desea definir un orden concreto en el que se muestran los elementos en la vista personalizada. Si no selecciona una columna para ordenarla, el valor predeterminado es Sin columna, es decir, sin ordenar u ordenar columnas especiales.
   * Solo las columnas seleccionadas en la variable [!UICONTROL Columnas] se incluyen en la [!UICONTROL Ordenar por columna] lista desplegable.
   * **Ascendente o Descendente:** Seleccione si desea ordenar la columna de forma ascendente o descendente de forma predeterminada.

1. Utilice la variable **[!UICONTROL Filtros]** para definir uno o más criterios de selección de elementos que se incluirán en la vista personalizada. Los filtros son especialmente útiles si desea utilizar la vista personalizada como un informe.
1. Para incluir todos los elementos en la vista personalizada, omita el **[!UICONTROL Filtros]** para obtener más información.
1. Filtros disponibles:

   * **Campo:** Seleccione el campo para este filtro (Comentarios es el campo predeterminado). La lista Campo contiene todos los campos Estándar (como en la [!UICONTROL Columnas] ). La lista no se limita a las columnas seleccionadas para su visualización.
   * **Operador:** Los operadores disponibles para el filtro dependen del tipo de campo seleccionado. Seleccione un Operator que muestre la relación entre el Campo y el campo de valor. Rellene esta información más adelante.
   * **Valor:** Seleccione o introduzca el valor elegido en este campo, según el campo y el operador seleccionado. Según el Operador que elija, puede haber un campo Valor, dos o ninguno. Consulte los ejemplos siguientes.
   * **Los filtros se aplican mediante la siguiente lógica:** Los criterios de filtro entre diferentes campos utilizan el operador AND. Varios criterios de filtro que utilizan el mismo campo utilizan el operador OR para el mismo campo.

      Si desea ver solo pruebas con cero comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Es igual a
      * Campo Valor: 0

      Si desea ver solo pruebas con dos o más comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Bueno o igual a
      * Campo Valor: 2

      Si desea ver solo pruebas con entre 1 y 4 comentarios, seleccione los siguientes valores:

      * Campo: Comentarios
      * Operador: Entre
      * Campo de valor (primer campo): 1
      * Campo de valor (segundo campo): 4

         Puede cambiar un filtro que haya agregado a la vista personalizada sin problemas o eliminarlo haciendo clic en el icono de cruz situado junto al [!UICONTROL configuración] filtrar si es necesario.

         Porque la lista Campo no está limitada a las columnas seleccionadas en la [!UICONTROL Columnas] , tenga cuidado al crear un filtro que incluya una columna que no haya seleccionado para mostrar en la vista personalizada. Por ejemplo, el siguiente filtro para la vista seleccionará todas las pruebas con un valor de contador de versión igual o superior a 2:

         * Campo = contador de versión
         * Operador = Bueno o igual a
         * Campo de valor = 2

            >[!NOTE]
            >
            >Puede cambiar un filtro que haya agregado a la vista personalizada sin problemas o eliminarlo haciendo clic en el icono de cruz situado junto al [!UICONTROL configuración] filtrar si es necesario.





1. En el **[!UICONTROL Uso compartido]** , seleccione qué usuarios de su cuenta podrán ver la vista personalizada.
1. Las vistas personalizadas son específicas del usuario que las crea. De forma predeterminada, la nueva vista personalizada solo es visible para su creador; sin embargo, puede elegir compartir su vista personalizada eligiendo una de las siguientes opciones:

   * **Solo usted puede ver esta vista personalizada** (predeterminado): Seleccione esta opción si desea que la vista personalizada solo esté disponible para usted.
   * **Todos los usuarios pueden ver esta vista personalizada**: Seleccione esta opción para que la vista personalizada esté disponible para todos los usuarios de la cuenta.
   * **Seleccionar usuarios que puedan ver esta vista personalizada**: Seleccione esta opción para que la vista personalizada solo esté disponible para usuarios específicos.
   * Comience a escribir el nombre o la dirección de correo electrónico del usuario al que desee tener acceso a la vista personalizada y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
   * Si decide no compartir su vista con otros usuarios en este momento, puede hacerlo más adelante editando la vista personalizada.

1. Haga clic en **[!UICONTROL Crear]**.
1. La vista Personalizado se muestra y está disponible en el [!DNL Views] página. Para obtener más información sobre las vistas, consulte [Administrar elementos en el [!DNL Views] Página en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Edición de vistas personalizadas

Puede editar una vista personalizada fácilmente. Para editar una vista personalizada:

1. Vaya a la **[!UICONTROL Vistas]** página.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el [!UICONTROL Vistas] botón (1)
1. Seleccione la vista que desee editar en el menú desplegable.\
   ![](assets/proof-view-edit.png)

1. Haga clic en el **[!UICONTROL Opciones de vista]** y haga clic en **[!UICONTROL Editar vista]**.\
   ![](assets/proof-view-options.png)\
   Se muestra la página Editar vista personalizada .

1. Haga clic en el [!UICONTROL Acciones] para abrir el Navegador. (3)\
   Este botón solo está disponible si incluye la columna Proof name en la vista.
1. Select [!UICONTROL Editar vista] del menú . (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. Se muestra la página Editar vista personalizada .

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Si edita la vista personalizada, las columnas de la lista Columnas seleccionadas se organizarán automáticamente en orden alfabético. Debe reorganizarlas si es necesario antes de actualizar la vista.


## Copia de vistas personalizadas

La función Copiar vista permite realizar fácilmente una copia de una vista personalizada existente. Esto es muy útil, por ejemplo, si desea configurar vistas independientes para todos los diseñadores, siendo cada vista la misma excepto para el propietario de la prueba (diseñador).

Para copiar una vista personalizada:

1. Vaya a la **[!UICONTROL Vistas]** página.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el **[!UICONTROL Vistas]** botón. (1)
1. Seleccione la vista personalizada en la lista. (2)
1. Haga clic en el **[!UICONTROL Acciones]** para abrir el Navegador. (3)\
   Este botón solo está disponible si incluye la columna Proof name en la vista.

1. Select [!UICONTROL Copiar] del menú . (4)\
   ![copy_custom_view.png](assets/copying-custom-view-350x258.png)

1. En la página Copiar vista personalizada , se rellenan todos los ajustes originales. Modifique la vista personalizada según su elección y haga clic en el botón **[!UICONTROL Copiar vista]** botón. Se le dirigirá a su nueva vista inmediatamente.\
   ![](assets/copy-custom-view-page-350x542.png)

## Compartir vistas personalizadas

La función Compartir vista permite compartir una vista con otros usuarios de su cuenta si aún no la ha seleccionado en la sección Compartir de la vista. Cuando comparte una vista personalizada con otros usuarios, esta aparece en sus [!UICONTROL Mis vistas personalizadas] del menú desplegable Vistas.

Para compartir una vista personalizada con otros usuarios:

1. Vaya a la **[!UICONTROL Vistas]** página.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el **[!UICONTROL Vistas]** botón (1)
1. Seleccione la vista personalizada de la lista (2)
1. Haga clic en el **[!UICONTROL Acciones]** para abrir el Navegador. (3)\
   Este botón solo está disponible si incluye la columna Proof name en la vista.

1. Select [!UICONTROL Vista Compartir] del menú (4)
1. Aparecerá la página Editar vista personalizada .
1. En el [!UICONTROL Uso compartido] seleccione los usuarios con los que desea compartir la vista y haga clic en **[!UICONTROL Actualizar vista]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportación de vistas personalizadas a archivos CSV

Para exportar los datos de una vista personalizada a un archivo CSV:

1. Vaya a la **[!UICONTROL Vistas]** página.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el **[!UICONTROL Vistas]** botón. (1)
1. Seleccione la vista personalizada en la lista. (2)
1. Haga clic en el **[!UICONTROL Acciones]** para abrir el Navegador. (3)\
   Este botón solo está disponible si incluye la columna Proof name en la vista.

1. Select [!UICONTROL Exportar a CSV] del menú . (4)\
   ![export_custom_view.png](assets/exporting-custom-view-350x258.png)\
   En una ventana separada del explorador, &quot;Generando informe: 100 %&#39; aparece más el número de registros (el número de elementos incluidos en el informe desde la vista personalizada)

1. (Condicional) Si aparece un mensaje de seguridad que indica que la descarga del informe está bloqueada actualmente, haga clic en para permitir que continúe la descarga.
1. Haga clic en **[!UICONTROL Guardar]** cuando aparece la ventana Descarga de archivos preguntando si desea abrir o guardar el archivo.
1. Seleccione una ubicación en el equipo y guarde el archivo.

## Eliminación de vistas personalizadas

Puede eliminar una vista personalizada fácilmente. Para ello:

1. Vaya a la **[!UICONTROL Vistas]** página.\
   Para obtener más información sobre las vistas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Haga clic en el **[!UICONTROL Vistas]** botón.
1. Seleccione la vista personalizada en la lista
1. Haga clic en el **[!UICONTROL Acciones]** para abrir el Navegador. (3)\
   Este botón solo está disponible si incluye la columna Proof name en la vista.

1. Select [!UICONTROL Eliminar] del menú . (4)\
   ![delete_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Haga clic en **[!UICONTROL Eliminar]** (5) para confirmar que desea eliminar la vista personalizada actual.\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. Se muestra la vista predeterminada Todos los elementos y la vista personalizada eliminada ya no aparece en la **[!UICONTROL Vistas]** menú desplegable.
