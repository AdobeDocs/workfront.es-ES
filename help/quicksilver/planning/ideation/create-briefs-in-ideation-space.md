---
title: Creación de informes en el espacio de ideación
description: Este artículo describe cómo puede crear ideas y estrategias en el espacio de ideación para crear informes. Puede exportar los informes de ideación finalizados a un archivo o a Workfront Planning para crear o actualizar registros.
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 2%

---


# Creación de informes en el espacio de ideación

<!-- add to TOC and miniTOC-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible como parte del programa **Beta** del espacio de ideación. </span>

<span class="preview">Para obtener más información, consulte [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Con el Espacio de ideas, una nueva funcionalidad de Adobe Workfront Planning, puede convertir informes en registros de Planning. Los informes exportados crean registros nuevos o actualizan los existentes.

Este artículo describe cómo puede crear ideas y estrategias en el espacio de ideación para crear informes. Para crear o actualizar registros, exporte los informes de ideación finalizados a un archivo o a Workfront Planning.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<ul> 
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Productos adicionales</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workflow</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> 
   <ul>
   <li><p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   </li>
   <li><p>La configuración Deshabilitar espacio de ideación en su nivel de acceso debe estar deseleccionada</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Permisos de contribución o superiores al espacio de trabajo y tipo de registro donde desee agregar registros </p>
      <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
      <p>Ver permisos de objetos de Workfront para agregarlos a informes <!--not sure if this is available--></p>
      <p>Permisos de editor en el espacio de ideación para crear informes</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Funciones de usuario de Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Cualquier función de usuario de GenStudio para acceder a campañas, productos y personas</li>
   <li>GenStudio System Manager para acceder a las activaciones <!--and Events--></li></ul>
   Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funciones de usuario y permisos</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Creación de informes de espacio de ideación

1. Comience en Workfront Planning y cree o edite un registro utilizando el espacio de ideación.

   Para obtener más información, consulte [Crear registros de Planning a partir de informes del espacio de ideación](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
1. Cuando se abra **Espacio de ideas**, use el símbolo del sistema proporcionado para describir el tipo de informe que desea crear.

   Por ejemplo, escriba &quot;Crear una campaña de regreso a la escuela para estudiantes de K-12 que se ejecute durante el mes de agosto, para padres y maestros en los Estados Unidos&quot;.  Para que el informe sea lo más completo posible, indique la mayor cantidad de información disponible sobre qué tipo de campaña, la cronología, las partes interesadas y otros detalles.

1. Haga clic en **Comenzar a idear**.

   Una vez abierto, el agente de espacio de ideación sigue los siguientes pasos:

   1. **Ingesta y síntesis de datos**: extrae información relevante de orígenes conectados. Por ejemplo:

      * Tipos de registro existentes o el tipo de registro existente desde el que comenzó.
      * Documentos recientes que puede haber cargado en el espacio de ideación.
      * Información web que coincide con los criterios de solicitud.

        >[!TIP]
        >
        >La configuración de búsqueda web debe estar activada para que AI pueda buscar información en la web.\
        >Para obtener más información, consulte la sección [Configurar el espacio de ideación](#configure-the-ideation-space)en este artículo.
        >
   1. **Definición de audiencia**: Identifica o recomienda parámetros de audiencia de destino basados en patrones históricos
   1. **Marco de estrategia**: estructura la narrativa estratégica de la campaña
   1. **Ideación de concepto y mensajería**: genera opciones de mensaje inicial y direcciones de concepto creativo
   1. **Entrega de generación y planificación de resúmenes**: genera un informe estructurado que se reenvía al espacio de trabajo de Workfront Planning

      Cuando el agente de ideación finaliza el proceso de recopilación de toda la información, se producen las siguientes cosas:

      * Se crean cinco tarjetas, organizadas por información relevante y similar.

        Las tarjetas se titulan utilizando varios pasos en la creación del registro solicitado, para facilitar el reconocimiento.

        Por ejemplo, se les podría poner el nombre:

        * Plan
        * Cronología
        * Segmentos
        * Mecánica
        * Mensajes

      Los títulos de las tarjetas son personalizados para cada tarjeta de la ideación.

      * Las tarjetas se colocan dentro del mismo marco indicando que este es el resultado de una ideación.

      * Se crea un informe que se muestra en una imagen de vista previa en la esquina inferior izquierda del espacio de ideación. <!--add screen shot??-->

      El informe contiene campos sugeridos que el sistema considera pertinentes para las ideas que está explorando.

1. (Opcional) Haga clic en el icono **Ayuda** ![](assets/more-information-icon.png) en la esquina superior derecha para obtener una lista de métodos abreviados de teclado que le ayudarán a desplazarse por el espacio de ideación.

1. (Opcional) Haga clic en **Fuentes** en la parte inferior de cada tarjeta para saber de dónde se recopiló la información.

   La información se puede importar desde Workfront Planning o desde la Web.
1. (Opcional) Use los iconos de los pulgares hacia arriba o hacia abajo de una tarjeta para proporcionar comentarios.<!--is this still available??-->
1. Haga clic en una tarjeta o en el marco que contiene todas las tarjetas y, a continuación, haga clic en **Agregar al informe** para agregar su información al informe.

   Workfront hace coincidir cada fragmento de información con el campo que encuentra con mayor probabilidad de almacenarla.

   Por ejemplo, las líneas de tiempo se agregan a los campos de tipo fecha y las descripciones a los campos de tipo párrafo.
   1. (Condicional) Haga clic en una tarjeta y, a continuación, haga clic en **Preguntar a AI a ...** para obtener ideas sobre el siguiente paso, antes de agregar la información al resumen. Las respuestas se encuentran en el contexto de la información de cada tarjeta.
   1. Haga clic en el icono **Agregar documentos** ![Agregar documentos](assets/add-documents-in-ideation-space.png) en la esquina superior izquierda del espacio de ideación para cargar documentos en el espacio. Puede agregar nuevos documentos o documentos que ya haya agregado al espacio anteriormente.

      >[!TIP]
      >
      >La configuración Documents debe estar activada para poder acceder a los documentos y cargarlos en el espacio.
      >Para obtener más información, consulte la sección [Configurar el espacio de ideación](#configure-the-ideation-space) en este artículo.
      > 
   1. Haga clic en el icono **Agregar tarjeta de taxonomía WF** ![Agregar desde Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> y seleccione un tipo de registro conectado y, a continuación, un registro de cada tipo para agregar la información de ese registro al tipo de registro seleccionado.

      Se creará una tarjeta para el registro seleccionado para añadirlo al espacio. El tipo de registro se muestra en la esquina superior izquierda de la tarjeta del registro.
   1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y luego en **Ver en Workfront**.

      La página de detalles del registro se abre en otra ficha del explorador de Workfront Planning.
   1. (Opcional) Seleccione el marco de ideación o una tarjeta, haga clic en el icono Eliminar y, a continuación, haga clic en Eliminar para confirmar. La tarjeta se eliminará del espacio de ideación.

      Al eliminar las tarjetas correspondientes a un documento almacenado o a un registro, los elementos se quitan del espacio de ideación, pero permanecen en sus aplicaciones respectivas.

1. (Opcional) Use el cuadro **Preguntar cualquier cosa** en la esquina inferior derecha en cualquier momento para refinar su idea.

   Por ejemplo, escriba `regenerate` para que una tarjeta específica rehaga esa tarjeta usando un contexto actualizado. El espacio de ideación vuelve a ejecutar sus pasos de razonamiento (buscar, sintetizar, citar) y actualiza las tarjetas afectadas.

1. (Opcional) En el cuadro **Preguntar cualquier cosa**, haga una nueva pregunta para comenzar una nueva ideación.

   Se genera un nuevo conjunto de tarjetas, después de que el espacio vuelva a ejecutar sus pasos de razonamiento.

1. (Opcional) Haga clic en uno de los conectores morados de cualquier conjunto de tarjetas de ideación y, a continuación, haga clic en el icono **Copiar a la barra de mensajes** para volver a ejecutar el razonamiento de ideación.

   ![Copiar al icono de la barra de mensajes](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Opcional) Haga clic en los iconos **Deshacer** o **Rehacer** ![Deshacer y rehacer](assets/undo-redo-icons.png) de la parte superior de la página para cancelar o revertir una acción.
1. Aleja para ver la imagen completa: tu objetivo original de la campaña, todas las tarjetas de concepto generadas por IA con citas, documentos adicionales, los registros reales de Workfront Planning que has extraído (productos, personalidades, etc.). La tarjeta de resumen **Brief** de la esquina inferior izquierda lo reúne todo.

1. Haga clic en la imagen de vista previa breve en la esquina inferior izquierda, revise la información y, a continuación, haga clic en una de las siguientes opciones:

   * **Exportar a archivo**. Puede exportar las instrucciones a los siguientes tipos de archivo:

     * PDF
     * Palabra
     * PowerPoint (con o sin plantilla)
   * **Exportar a Workfront Planning**. La exportación sobrescribe todos los datos de campo existentes en el registro de Workfront Planning.

   De este modo, se termina de crear el registro con la información adicional y se agrega al tipo de registro seleccionado originalmente.

   Para obtener más información acerca de la actualización de registros de Planning mediante informes, vea la sección &quot;ConsideracionesConsideraciones acerca del uso del espacio de ideación para crear registros&quot; en el artículo [Crear registros de Planning a partir de informes del espacio de ideación](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configuración del espacio de ideación

Existen controles para el espacio de ideación que configuran lo que se ve en la pantalla y le ayudan a desplazarse por el espacio.

1. Haga clic en el icono **Configuración** ![Configuración](assets/setting-icon.png) para controlar de dónde extrae información AI y, a continuación, elija entre los siguientes **tipos de Source**:

   * **Documentos**: documentos cargados en el espacio seleccionado
   * **Búsqueda web**: investigación web externa
   * **CJA** — Adobe Customer Journey Analytics

1. Haga clic en **Guardar**.

1. Haga clic en el icono **Ayuda** ![Icono de Ayuda](assets/more-information-icon.png) para revisar los métodos abreviados de teclado que puede usar para desplazarse por el espacio de ideación o seleccionar un valor de zoom diferente.

   Elija entre los siguientes niveles de zoom:

   * Zoom al 100 %
   * Zoom de 200%
   * Ajustar al tamaño

   También puede utilizar uno de los siguientes métodos abreviados para desplazarse por la página:

   | Acción | Método abreviado |
   |---|---|
   | Acercar/alejar | Ctrl/⌘ + / − |
   | Ajustar para ajustar/ajustar la selección | — |
   | Zoom hasta el cursor | Ctrl/⌘ + desplazamiento |
   | Panorámica del lienzo | Mantener espacio + arrastrar |
   | Mostrar u ocultar cuadrícula de puntos | G |

1. Haga clic en el icono Buscar para buscar elementos en el espacio de ideación y, a continuación, haga clic en cuando se muestre en la lista para desplazarse a él.








