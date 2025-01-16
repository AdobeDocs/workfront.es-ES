---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: El editor de escenarios en  [!DNL Adobe] Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1172'
ht-degree: 93%

---

# El editor de escenarios en [!DNL Adobe Workfront Fusion]

El editor de escenarios permite crear y editar escenarios en una interfaz visual.

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Editor de escenarios en Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/navigate-workfront-fusion/scenario-editor.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

![](assets/scenario-editor.jpg)

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abra el editor de escenarios:

1. Haga clic en **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

1. Si desea crear un escenario, haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   O

   Si desea editar un escenario existente, haga clic en él.

   En el editor de escenarios que se muestra, puede hacer todo lo que se indica en la tabla siguiente. Para obtener más información, consulte [Creación de un escenario en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Cuando termine de editar un escenario (o en cualquier momento mientras lo está editando), haga clic en el icono [!UICONTROL Guardar]. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Después de guardar el escenario, dispondrá de una nueva versión en el menú de tres puntos en caso de que necesite acceder a ella en el futuro. Las versiones de escenarios guardadas anteriormente solo están disponibles durante 60 días.

## Acciones del editor de escenarios disponibles

En el editor de escenarios están disponibles las acciones siguientes:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Añadir el primer módulo</td>
     <td> <p>Haga clic en el icono de signo de interrogación. <img src="assets/question-mark-full-size.png"></p> <p> A continuación, busque y haga clic en la aplicación o el servicio con el que desea empezar. Si ha seleccionado alguna aplicación en el paso 2, aparecerá aquí para facilitar el acceso (y en la sección <strong>[!UICONTROL Favorites]</strong> en la parte inferior de la pantalla).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Añadir un módulo</td>
     <td>Pase el ratón sobre un módulo, haga clic en el icono de signo más que aparece a la derecha y, a continuación, haga clic en el módulo que desee en el menú que aparece.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Especifique cuándo y con qué frecuencia se ejecutará el escenario</td>  
      <td> <p>Haga clic en el icono de reloj. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configuración de una ruta</td>   
     <td> <p>Haga clic en el icono de [!UICONTROL wrench] <img src="assets/wrench-icon.gif"> entre los dos módulos y utilice cualquiera de las siguientes opciones:</p>    
       <ul>
         <li><strong>[!UICONTROL Set up a filter]</strong>: Controle qué paquetes se utilizan en determinados puntos del escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Unlink]</strong>: quita una ruta.</li>     
         <li><strong>[!UICONTROL Add a router]</strong>: añade un enrutador entre módulos. </li>     
         <li><strong>[!UICONTROL Add a module]</strong>: añade un módulo nuevo entre módulos.</li>     
         <li><strong>[!UICONTROL Add a note]</strong>: añade una nota a la ruta.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Eliminación de un módulo</td>   
     <td>Haga clic con el botón derecho en el módulo y, a continuación, haga clic en <strong>[!UICONTROL Delete module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Ver un registro de los eventos que se producen en un escenario</td>     
     <td> 
       <p>Publique un escenario. Cuando el escenario termine de ejecutarse, el registro aparecerá en la esquina inferior derecha del [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Según el escenario, el registro puede contener información sobre la dificultad de cada fase y los errores encontrados durante la ejecución del escenario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Establecer la configuración del escenario</td>   
     <td>Haga clic en el icono [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Esta configuración está dirigida principalmente a usuarios avanzados.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Escribir o ver notas sobre el escenario</td>   
     <td>Haga clic en el icono [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alinear automáticamente del diseño de los módulos </td>   
     <td>Haga clic en el icono [!UICONTROL Auto-align]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Ver una animación que muestra cómo fluyen los datos a través del escenario</td>   <td>Haga clic en el icono [!UICONTROL Explain Flow]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exportar el escenario al equipo como modelo</td>   
     <td>Haga clic en el menú [!UICONTROL More] <img src="assets/more-icon.png"> y, a continuación, en [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importar un modelo de escenario desde el equipo</td>   
     <td>Haga clic en el menú [!UICONTROL More] <img src="assets/more-icon.png"> y, a continuación, en [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurar una versión anterior del escenario</td>   
     <td>Consulte el artículo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurar una versión de escenario en [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Establecer la configuración de [!UICONTROL Flow Control]</td>   
     <td> <p>Haga clic en el icono [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Puede configurar una tarea para que se repita un número determinado de veces, convertir una matriz en una serie de paquetes y combinar varios paquetes en uno solo. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Control de flujo en [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Mejorar el escenario con herramientas avanzadas</td>   
     <td>Haga clic en el icono [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Puede crear activadores, acciones, agregadores y transformadores. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Usar herramientas de análisis de texto</td>   
     <td>Haga clic en el icono [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Puede recuperar elementos del código de HTML, buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda, buscar y reemplazar texto y realizar un “raspado” de datos de un sitio web. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Acceder a las aplicaciones y servicios más utilizados</td>   
     <td> Haga clic en un icono de la sección <strong>[!UICONTROL Favorites]</strong> en la parte inferior de la pantalla. Los iconos se muestran en esta sección automáticamente cuando se añaden aplicaciones y servicios al escenario. También se puede hacer clic en el icono Añadir <img src="assets/add-icon.gif"> para añadir aplicaciones y servicios a esta área manualmente.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Realizar una ejecución de prueba del escenario</td>   
     <td>Haga clic en <strong>[!UICONTROL Run once]</strong> para comprobar que el escenario se ejecuta del modo previsto antes de activarlo. Una vez activado, el escenario se ejecutará según su programación. Si no todo funciona del modo previsto, puede visitar nuestra sección de gestión de errores para aprender a gestionarlos.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Utilizar Devtool para depurar el escenario</td>   
     <td>Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Escenarios de depuración con el Devtool de [!DNL Adobe Workfront Fusion]</a>.
</td> 
   </tr> 
<tr>
<td>Comprobar el estado del escenario</td>
<td>Los escenarios pueden estar activos o inactivos. Puede cambiar el estado del escenario haciendo clic en el botón Activar/Desactivar en el detalle del escenario.

Consulte los siguientes artículos para obtener más información.
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Activar o desactivar un escenario en Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Detalles del escenario en Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Cambiar la programación del escenario</td>
<td>Los escenarios activos se ejecutan según un horario. De forma predeterminada, un escenario se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia se ejecuta un escenario activado. Los escenarios de fusión pueden programarse para que se ejecuten incluso cada 5 minutos.

Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Programar un escenario en Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Cambiar el nombre del escenario</td>
<td>Para cambiar el nombre de un escenario, ábralo, haga clic en el nombre del escenario en la esquina superior izquierda y edítelo. Pulse Intro o haga clic fuera del campo editado para guardar el nombre del escenario.</td>
</tr>
<tr>
<td>Seleccionar el primer paquete</td>
<td>Algunos módulos de activación le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.

Para obtener más información, consulte <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Elegir dónde se inicia un módulo de activación en Adobe Workfront Fusion</a>.</td>
</tr>
<tr>
<td>Configuración del número de paquetes devueltos</td>
<td>Los módulos, de forma predeterminada, siempre devuelven solo dos paquetes. Esto se puede cambiar en la configuración del módulo en el campo [!UICONTROL Maximum number of returned bundles].</td>
</tr>
<tr>
<td>Configuración avanzada de escenarios</td>
<td>[!DNL Adobe Workfront Fusion] le ofrece la posibilidad de configurar otros ajustes avanzados.

Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">El panel de ajustes de escenarios en Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
