---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: El editor de escenarios de [!DNL Adobe] Workfront Fusion
description: El editor de escenarios permite crear y editar escenarios en una interfaz visual.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# El editor de escenarios de [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abra el editor de escenarios:

1. Haga clic en **[!UICONTROL Situaciones]** ![](assets/scenarios-icon.png) en el panel izquierdo.

1. Si desea crear un escenario, haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   O

   Si desea editar un escenario existente, haga clic en el escenario.

1. (Condicional) Si está creando un nuevo escenario, en **[!UICONTROL Qué servicios desea integrar]**, seleccione las aplicaciones con las que desee trabajar en el escenario y, a continuación, haga clic en **[!UICONTROL Continuar]**.

   O

   Haga clic en **[!UICONTROL Omitir]** si desea elegir las aplicaciones desde el editor de escenarios.

   En el editor de situaciones que se muestra, puede hacer todo lo que se enumera en la siguiente tabla. Para obtener más información, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Cuando termine de editar un escenario (o en cualquier momento mientras esté editando), haga clic en el botón [!UICONTROL Guardar] icono. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Después de guardar el escenario, habrá una nueva versión disponible en el menú de tres puntos en caso de que necesite acceder a ella en el futuro. Las versiones de escenarios guardadas anteriormente solo están disponibles durante 60 días.

## Acciones disponibles del editor de escenarios

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Añadir el primer módulo</td>
     <td> <p>Haga clic en el icono del signo de interrogación. <img src="assets/question-mark-full-size.png"></p> <p> A continuación, busque y haga clic en la aplicación o el servicio con el que desea comenzar. Si seleccionó alguna aplicación en el paso 2, esta aparecerá aquí para facilitar el acceso (y en la <strong>[!UICONTROL Favoritos]</strong> en la parte inferior de la pantalla).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Añadir un módulo</td>
     <td>Pase el ratón sobre un módulo, haga clic en el icono de signo más que aparece a la derecha y, a continuación, haga clic en el módulo que desee en el menú que aparece.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Especifique cuándo y con qué frecuencia se ejecutará el escenario</td>  
      <td> <p>Haga clic en el icono del reloj. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programar un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configuración de una ruta</td>   
     <td> <p>Haga clic en el icono [!UICONTROL llave inglesa] <img src="assets/wrench-icon.gif"> entre los dos módulos y utilice cualquiera de las siguientes opciones:</p>    
       <ul>
         <li><strong>[!UICONTROL Configurar un filtro]</strong>: Controle qué paquetes se utilizan en determinados puntos del escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Desvincular]</strong>: Quita una ruta.</li>     
         <li><strong>[!UICONTROL Agregar un enrutador]</strong>: Agrega un router entre módulos. </li>     
         <li><strong>[!UICONTROL Agregar un módulo]</strong>: Agrega un nuevo módulo entre módulos.</li>     
         <li><strong>[!UICONTROL Agregar una nota]</strong>: Agrega una nota a la ruta.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Eliminación de un módulo</td>   
     <td>Haga clic con el botón derecho en el módulo y, a continuación, haga clic en <strong>[!UICONTROL Eliminar módulo]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Ver un registro de los eventos que se producen es un escenario</td>     
     <td> 
       <p>Ejecute un escenario. Cuando el escenario termina de ejecutarse, el registro aparece en la esquina inferior derecha del [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Según el escenario, el registro puede contener información sobre la dificultad de cada fase y los errores encontrados durante la ejecución del escenario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configurar las opciones de escenario</td>   
     <td>Haga clic en el icono [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Estos ajustes están pensados principalmente para usuarios avanzados.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Escriba o vea notas sobre el escenario</td>   
     <td>Haga clic en el icono [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alinear automáticamente el diseño de los módulos </td>   
     <td>Haga clic en el icono [!UICONTROL Alinear automáticamente]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Ver una animación que muestra cómo fluyen los datos a través del escenario</td>   <td>Haga clic en el icono [!UICONTROL Explicar flujo]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exportar el escenario al equipo como un modelo</td>   
     <td>Haga clic en el menú [!UICONTROL Más] <img src="assets/more-icon.png">y, a continuación, haga clic en [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importar un modelo de escenario desde el equipo</td>   
     <td>Haga clic en el menú [!UICONTROL Más] <img src="assets/more-icon.png">y, a continuación, haga clic en [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurar una versión anterior del escenario</td>   
     <td>Consulte el artículo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurar una versión de escenario en [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configuración de la configuración de [!UICONTROL Flow Control]</td>   
     <td> <p>Haga clic en el icono [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Puede configurar una tarea para que se repita un número determinado de veces, convertir una matriz en una serie de paquetes y combinar varios paquetes en un solo paquete. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Control de flujo en [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Mejorar el escenario con herramientas avanzadas</td>   
     <td>Haga clic en el icono [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Puede crear déclencheur, acciones, agregadores y transformadores. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Uso de herramientas de análisis de texto</td>   
     <td>Haga clic en el icono [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Puede recuperar elementos del código del HTML, buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda, buscar y reemplazar texto y crear secuencias de comandos de datos de un sitio web. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Acceda a las aplicaciones y servicios más utilizados</td>   
     <td> Haga clic en un icono de <strong>[!UICONTROL Favoritos]</strong> en la parte inferior de la pantalla. Los iconos se muestran en esta sección automáticamente al agregar aplicaciones y servicios al escenario. También puede hacer clic en el icono Añadir <img src="assets/add-icon.gif"> para agregar aplicaciones y servicios a esta área manualmente.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Ejecutar la prueba</td>   
     <td>Haga clic en <strong>[!UICONTROL Ejecutar una vez]</strong> para comprobar que el escenario se ejecuta tal como espera antes de activarlo. Una vez activado, el escenario se ejecutará según su programación. Si todo no se ejecuta según lo esperado, puede visitar nuestra sección de administración de errores para aprender a manejar los errores.</td> 
   </tr> 
</tbody>
