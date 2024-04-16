---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Creación de un escenario en Adobe Workfront Fusion
description: Las siguientes tareas explican cómo crear un [!DNL Adobe Workfront Fusion] escenario.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# Creación de un escenario en [!DNL Adobe Workfront Fusion]

Las siguientes tareas explican cómo crear un [!DNL Adobe Workfront Fusion] escenario.

Para ver un ejercicio práctico que le guíe en la creación de un escenario de automatización, consulte [Cree un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Para ver un ejercicio práctico que le guíe a través de la creación de un escenario de integración con los datos que proporcionamos, consulte [Creación de un escenario de integración de prácticas en Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Para crear un escenario a partir de una plantilla, consulte [Creación de escenarios con [!DNL Adobe Workfront Fusion] templates](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p><p>[!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Empezar a crear un escenario

1. Clic **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

1. Clic **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.
1. En la pantalla que aparece (el editor de escenarios), si está creando un nuevo escenario, haga clic en **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y escriba un nombre para el escenario.
1. Continúe en a [Adición de un módulo en un escenario](#add-a-module-in-a-scenario).

## Adición de un módulo en un escenario

1. Para agregar el primer módulo al escenario, haga clic en el icono de signo de interrogación. ![](assets/question-mark-icon.gif)

   O

   Para agregar módulos adicionales al escenario, haga clic en el controlador situado en la parte derecha del módulo que desea que siga.

1. En el cuadro que aparece, busque y haga clic en la aplicación o el servicio con el que desee comenzar.

   Todas las aplicaciones seleccionadas anteriormente se muestran en el cuadro para facilitar el acceso y en el **[!UICONTROL Favoritos]** en la parte inferior de la pantalla.

   Si hace clic **[!UICONTROL Añadir otro módulo]**, los módulos que se muestran dependen de dónde en el escenario esté agregando el módulo. Algunos módulos solo se pueden colocar entre otros módulos y otros solo al principio del escenario.

   >[!TIP]
   >
   >Los dos tipos más comunes de módulos son acciones y déclencheur. Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. En la lista de módulos que se muestra, haga clic en el primer módulo que desee agregar al escenario.

   Los módulos que se muestran dependen de dónde desee agregar un módulo en su escenario. Algunos módulos solo se pueden colocar entre otros módulos y otros solo al principio del escenario.

   Los dos tipos más comunes de módulos son acciones y déclencheur. Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. Continúe en a [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Módulos de Workfront Fusion que se conectan a una aplicación (como [!DNL Workfront], [!DNL Salesforce], o [!DNL Jira)] incluir el [!UICONTROL Conexión] field. Aquí puede especificar la conexión que desea que utilice este módulo para conectarse a la aplicación. Puede seleccionar una conexión existente en la lista desplegable o crear una nueva conexión.

Cuando selecciona o crea una conexión para una aplicación en un escenario concreto, otros módulos para esa aplicación utilizan automáticamente la misma conexión a menos que seleccione una diferente al configurar los módulos posteriores.

Para obtener más información, consulte [Información general sobre Conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Para crear una conexión dentro de un [!DNL Workfront Fusion] módulo:

1. Clic **[!UICONTROL Añadir]** para abrir **[!UICONTROL Crear una conexión]** cuadro.
1. (Opcional) Cambiar el valor predeterminado **[!UICONTROL Nombre de conexión]**.
1. (Condicional) Si la aplicación requiere una configuración de conexión avanzada, como un ID, una clave o [!UICONTROL secreto], introduzca esa información.

   Es posible que tenga que hacer clic en **[!UICONTROL Mostrar configuración avanzada]** para mostrar los campos donde puede introducir este tipo de información.

1. Clic **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que aparece, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si **[!UICONTROL Permitir]** , examine las acciones que podrá realizar el conector y haga clic en el botón para conectar la aplicación [!DNL Workfront Fusion].
1. Continúe en a [Configuración del módulo](#configure-the-module).


## Configuración del módulo

1. En los campos situados debajo del campo Conexión, configure las opciones del módulo y, a continuación, haga clic en **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Estos ajustes son diferentes para cada módulo. Un título en negrita indica una configuración requerida.

   >[!TIP]
   >
   >A medida que trabaje en su escenario, puede hacer clic en el módulo para mostrar este cuadro de configuración en cualquier momento.
   >
   >
   >Si ve un círculo negro en un módulo, aún no ha terminado de configurar sus opciones. Haga clic en el módulo para abrirlo y continuar configurando.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Si va a agregar el primer módulo al escenario, seleccione una opción para indicar dónde desea que comience el escenario cada vez que se ejecute.

   ![](assets/choose-where-start-350x194.png)

1. Repita los pasos de las secciones [Adición de un módulo en un escenario](#add-a-module-in-a-scenario) y [Configuración del módulo](#configure-the-module) para agregar otros módulos al escenario.

1. (Opcional) Copie y pegue un módulo o grupo de módulos.

   Para obtener más información, consulte [Copia de módulos o escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continúe en a [Configurar y trabajar con su escenario](#configure-and-work-with-your-scenario).

## Configurar y trabajar con su escenario

1. Realice cualquiera de las siguientes acciones para configurar su escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Especifique cuándo y con qué frecuencia se ejecutará el escenario</td> 
      <td> <p>Haga clic en el icono de reloj. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programar un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurar una ruta</td> 
      <td> <p>Haga clic en el icono de llave inglesa <img src="assets/wrench-icon.gif"> entre los dos módulos y utilice cualquiera de las siguientes opciones. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adición de un filtro a un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Configurar un filtro]</strong>: Controle qué paquetes se utilizan en determinados puntos del escenario.</li> 
        <li><strong>[!UICONTROL Desvincular]</strong>: elimina una ruta.</li> 
        <li><strong>[!UICONTROL Agregar un enrutador]</strong>: agrega un enrutador entre módulos. </li> 
        <li><strong>[!UICONTROL Agregar un módulo]</strong>: añade un nuevo módulo entre módulos.</li> 
        <li><strong>[!UICONTROL Agregar nota]</strong>: añade una nota a la ruta.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de los escenarios</td> 
      <td>Haga clic en el icono [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Esta configuración está dirigida principalmente a usuarios avanzados. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">El panel de configuración de escenario en [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de control de flujo</td> 
      <td> <p>Haga clic en el icono [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Puede configurar una tarea para que se repita un número determinado de veces, convertir una matriz en una serie de paquetes y combinar varios paquetes en uno solo. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Control de flujo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mejore el escenario con herramientas avanzadas</td> 
      <td>Haga clic en [!DNL Tools] icono. <img src="assets/tools-icon.gif"> Puede crear déclencheur, acciones, agregadores y transformadores. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herramientas de análisis de texto de usuario</td> 
      <td>Haga clic en [!DNL Text parser] icono <img src="assets/text-parser-icon.gif">. Puede recuperar elementos del código del HTML, buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda, buscar y reemplazar texto y "crear secuencias de comandos" de datos de un sitio web. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Realice cualquiera de las siguientes acciones para trabajar con su escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ver un registro de los eventos que se producen cuando se ejecuta el escenario</td> 
      <td> <p>Haga clic en la flecha de [!UICONTROL Exit editing] <img src="assets/exit-editing-arrow.png"> en el editor de escenarios para ver la página de detalles de Escenario. El registro se muestra en la parte inferior de la ventana o en la esquina inferior derecha. Contiene información sobre cada fase y los errores encontrados durante la ejecución del escenario.</p> <p>Para volver a trabajar con su escenario en [!DNL scenario editor], haga clic en cualquier lugar de la página de detalles de Escenario.</p> <p>Para obtener más información sobre la página de detalles de Escenario, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalles del escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceda a sus aplicaciones y servicios más utilizados</td> 
      <td> Haga clic en un icono de la <strong>[!UICONTROL Favoritos]</strong> en la parte inferior de la pantalla. Los iconos se muestran en esta sección automáticamente cuando agrega aplicaciones y servicios a su escenario. También puede hacer clic en el icono [!UICONTROL Add] <img src="assets/add-icon.gif"> para agregar aplicaciones y servicios a esta área manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver una animación que muestra cómo fluyen los datos a través del escenario</td> 
      <td>Haga clic en el icono [!UICONTROL Explicar flujo] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alineación automática del diseño de los módulos </td> 
      <td>Haga clic en el icono [!UICONTROL Alinear automáticamente] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Escriba o vea notas sobre el escenario</td> 
      <td>Haga clic en el icono [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminación de un módulo</td> 
      <td>Haga clic con el botón derecho en el módulo y luego haga clic en <strong>[!UICONTROL Eliminar módulo]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para probar el escenario, haga clic en **[!UICONTROL Ejecutar una vez]**.

   Es importante verificar que el escenario se ejecuta como espera antes de activarlo. Una vez activado, el escenario se ejecutará según su programación. Si todo no funciona como se espera, consulte [Tratamiento de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Cuando termine de editar el escenario (o en cualquier momento mientras lo esté editando), haga clic en [!UICONTROL Guardar] en la parte inferior de la ventana ![](assets/save-icon.gif).

Para obtener información sobre cómo activar un escenario, consulte [Activación o desactivación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Métodos abreviados del teclado para escenarios de Workfront Fusion

Puede utilizar los siguientes métodos abreviados del teclado al crear o editar un escenario:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Acción</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guardar] </td> 
   <td>Ctrl + Mayús + S</td> 
   <td><span style="font-weight: normal;">Cmd + Mayús + S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ejecutar una vez]</td> 
   <td>Ctrl + Mayús + Intro</td> 
   <td><span style="font-weight: normal;">Cmd + Mayús + Intro</span> </td> 
  </tr> 
 </tbody> 
</table>
