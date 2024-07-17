---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Editor de escenarios en  [!DNL Adobe] Workfront Fusion
description: El editor de escenarios permite crear y editar escenarios en una interfaz visual.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# Editor de escenarios en [!DNL Adobe Workfront Fusion]

El editor de escenarios permite crear y editar escenarios en una interfaz visual.

![](assets/scenario-editor-350x228.jpg)

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
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abra el editor de escenarios:

1. Haga clic en **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

1. Si desea crear un escenario, haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   O

   Si desea editar un escenario existente, haga clic en el escenario.

   En el editor de escenarios que se muestra, puede hacer todo lo que se indica en la tabla siguiente. Para obtener más información, vea [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Cuando termine de editar un escenario (o en cualquier momento mientras lo está editando), haga clic en el icono [!UICONTROL Guardar]. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Después de guardar el escenario, habrá disponible una nueva versión en el menú de tres puntos por si necesita acceder a ella en el futuro. Las versiones de escenarios guardadas anteriormente solo están disponibles durante 60 días.

## Acciones del editor de escenarios disponibles

Las siguientes acciones están disponibles en el editor de escenarios:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Añadir el primer módulo</td>
     <td> <p>Haga clic en el icono de signo de interrogación. <img src="assets/question-mark-full-size.png"></p> <p> A continuación, busque y haga clic en la aplicación o el servicio con el que desee comenzar. Si seleccionó alguna aplicación en el paso 2, aparecerá aquí para facilitar el acceso (y en la sección <strong>[!UICONTROL Favoritos]</strong> en la parte inferior de la pantalla).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Añadir un módulo</td>
     <td>Pase el ratón sobre un módulo, haga clic en el icono de signo más que aparece a la derecha y, a continuación, haga clic en el módulo que desee en el menú que aparece.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Especifique cuándo y con qué frecuencia se ejecutará el escenario</td>  
      <td> <p>Haga clic en el icono de reloj. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obtener más información, vea <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programar un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configurar una ruta</td>   
     <td> <p>Haga clic en el icono de [!UICONTROL wrench] <img src="assets/wrench-icon.gif"> entre los dos módulos y utilice cualquiera de las siguientes opciones:</p>    
       <ul>
         <li><strong>[!UICONTROL Configurar un filtro]</strong>: Controle qué paquetes se utilizan en determinados puntos del escenario. Para obtener más información, vea <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Agregar un filtro a un escenario en [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Desvincular]</strong>: quita una ruta.</li>     
         <li><strong>[!UICONTROL Agregar un enrutador]</strong>: Agrega un enrutador entre módulos. </li>     
         <li><strong>[!UICONTROL Agregar un módulo]</strong>: Agrega un módulo nuevo entre módulos.</li>     
         <li><strong>[!UICONTROL Agregar una nota]</strong>: Agrega una nota a la ruta.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Eliminación de un módulo</td>   
     <td>Haga clic con el botón secundario en el módulo y, a continuación, haga clic en <strong>[!UICONTROL Delete module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Ver un registro de los eventos que se producen en un escenario</td>     
     <td> 
       <p>Ejecute un escenario. Cuando el escenario termina de ejecutarse, el registro aparece en la esquina inferior derecha del [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Según el escenario, el registro puede contener información sobre la dificultad de cada fase y los errores encontrados durante la ejecución del escenario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configuración de los escenarios</td>   
     <td>Haga clic en el icono [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Esta configuración está dirigida principalmente a usuarios avanzados.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Escriba o vea notas sobre el escenario</td>   
     <td>Haga clic en el icono [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alineación automática del diseño de los módulos </td>   
     <td>Haga clic en el icono [!UICONTROL Alinear automáticamente]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Ver una animación que muestra cómo fluyen los datos a través del escenario</td>   <td>Haga clic en el icono [!UICONTROL Explicar flujo]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exporte el escenario a su equipo como modelo</td>   
     <td>Haga clic en el menú [!UICONTROL Más] <img src="assets/more-icon.png"> y, a continuación, haga clic en [!UICONTROL Exportar modelo].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importar un modelo de escenario desde el equipo</td>   
     <td>Haga clic en el menú [!UICONTROL Más] <img src="assets/more-icon.png"> y, a continuación, haga clic en [!UICONTROL Importar modelo].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurar una versión anterior del escenario</td>   
     <td>Consulte el artículo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurar una versión de escenario en [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configurar opciones de [!UICONTROL Flow Control]</td>   
     <td> <p>Haga clic en el icono [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Puede configurar una tarea para que se repita un número determinado de veces, convertir una matriz en una serie de paquetes y combinar varios paquetes en uno solo. Para obtener más información, vea <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Control de flujo en [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Mejore el escenario con herramientas avanzadas</td>   
     <td>Haga clic en el icono [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Puede crear déclencheur, acciones, agregadores y transformadores. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Uso de herramientas de análisis de texto</td>   
     <td>Haga clic en el icono [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Puede recuperar elementos del código de HTML, buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda, buscar y reemplazar texto y "crear secuencias de comandos" de datos de un sitio web. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Acceda a sus aplicaciones y servicios más utilizados</td>   
     <td> Haga clic en un icono de la sección <strong>[!UICONTROL Favoritos]</strong> en la parte inferior de la pantalla. Los iconos se muestran en esta sección automáticamente cuando agrega aplicaciones y servicios a su escenario. También puede hacer clic en el icono Agregar <img src="assets/add-icon.gif"> para agregar aplicaciones y servicios a esta área manualmente.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Prueba y ejecución del escenario</td>   
     <td>Haga clic en <strong>[!UICONTROL Ejecutar una vez]</strong> para comprobar que el escenario se ejecuta como espera antes de activarlo. Una vez activado, el escenario se ejecutará según su programación. Si todo no funciona como se espera, puede visitar nuestra sección de gestión de errores para aprender a gestionar los errores.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Utilizar Devtool para depurar el escenario</td>   
     <td>Para obtener más información, vea <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Escenarios de depuración con la herramienta de depuración [!DNL Adobe Workfront Fusion]</a>.
</td> 
   </tr> 
<tr>
<td>Comprobar el estado del escenario</td>
<td>Los escenarios pueden estar activos o inactivos. Puede cambiar el estado del escenario haciendo clic en el botón Encendido/Apagado en el detalle del escenario.

Consulte los siguientes artículos para obtener más información:
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Activación o desactivación de un escenario en Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Detalles de los escenarios en Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Cambiar la programación del escenario</td>
<td>Los escenarios activos se ejecutan según una programación. De forma predeterminada, un escenario se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia se ejecuta un escenario activado. Los escenarios de Fusion se pueden programar para que se ejecuten con tanta frecuencia como cada 5 minutos.

Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Programar un escenario en Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Cambie el nombre del escenario</td>
<td>Para cambiar el nombre de un escenario, ábralo, haga clic en el nombre del escenario en la esquina superior izquierda y edítelo. Pulse Entrar o haga clic fuera del campo editado para guardar el nombre del escenario.</td>
</tr>
<tr>
<td>Seleccionar el primer paquete</td>
<td>Algunos módulos de déclencheur le permiten seleccionar el primer paquete desde el que desea que se inicie la recuperación de paquetes.

Para obtener más información, consulte <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Elegir dónde se inicia un módulo de déclencheur en Adobe Workfront Fusion</a>.</td>
</tr>
<tr>
<td>Configuración del número de paquetes devueltos</td>
<td>Los módulos, de forma predeterminada, siempre devuelven solo dos paquetes. Esto se puede cambiar en la configuración del módulo en el campo [!UICONTROL Número máximo de paquetes devueltos].</td>
</tr>
<tr>
<td>Configuración avanzada de escenarios</td>
<td>[!DNL Adobe Workfront Fusion] le ofrece la posibilidad de configurar otras opciones avanzadas.

Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">El panel de configuración de escenarios en Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
