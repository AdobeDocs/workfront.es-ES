---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Creación de un escenario en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 94%

---

# Crear un escenario en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Flujo de trabajo para crear un escenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Las siguientes tareas explican cómo crear un escenario de [!DNL Adobe Workfront Fusion].

Para encontrar un ejercicio práctico que le guíe en la creación de un escenario de automatización, consulte [Crear un escenario de automatización de práctica en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Para encontrar un ejercicio práctico que le guíe en la creación de un escenario de integración con los datos que proporcionamos, consulte [Crear un escenario de integración de prácticas en Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Para crear un escenario a partir de una plantilla, consulte [Crear escenarios con [!DNL Adobe Workfront Fusion] plantillas](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Plan de Adobe Workfront</td>  
      <td>Cualquiera</td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront</td>  
      <td>
        Nuevo: Estándar<br>
        O<br>
        Actual: Trabajo o superior
      </td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront Fusion</td>  
      <td> 
        Actual: no se requiere licencia de Workfront Fusion.<br>
        O<br>
        Heredado: cualquiera
      </td>  
    </tr>  
    <tr>  
      <td>Producto</td>  
      <td> 
        Nuevo: Plan Select or Prime Workfront: su organización debe adquirir Adobe Workfront Fusion.<br>
        Plan Ultimate Workfront: Workfront Fusion está incluido.<br>
        O<br>
        Actual: su organización debe adquirir Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Empezar a crear un escenario

1. Haga clic en **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

1. Haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.
1. En la pantalla que aparece (el editor de escenarios), si está creando un nuevo escenario, haga clic en **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y escriba un nombre para el escenario.
1. Continúe en [Añadir un módulo en un escenario](#add-a-module-in-a-scenario).

## Adición de un módulo en un escenario

1. Para añadir el primer módulo al escenario, haga clic en el icono de signo de interrogación. ![](assets/question-mark-icon.gif)

   O

   Para añadir módulos adicionales al escenario, haga clic en el controlador situado en la parte derecha del módulo que desea que siga.

1. En el cuadro que aparece, busque y haga clic en la aplicación o el servicio con el que desee comenzar.

   Todas las aplicaciones seleccionadas anteriormente se muestran en el cuadro para facilitar el acceso y en la sección **[!UICONTROL Favoritos]** de la parte inferior de la pantalla.

   Si hace clic en **[!UICONTROL Añadir otro módulo]**, los módulos que se muestran dependen del lugar del escenario en el que añada el módulo. Algunos módulos solo se pueden colocar entre otros módulos y otros solo al inicio del escenario.

   >[!TIP]
   >
   >Los dos tipos más comunes de módulos son acciones y activadores. Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. En la lista de módulos que se muestra, haga clic en el primer módulo que desee añadir al escenario.

   Los módulos que se muestran dependen de dónde desee añadir un módulo en su escenario. Algunos módulos solo se pueden colocar entre otros módulos y otros solo al inicio del escenario.

   Los dos tipos más comunes de módulos son acciones y activadores. Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. Continúe en [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Los módulos de Workfront Fusion que se conectan a una aplicación (como [!DNL Workfront], [!DNL Salesforce] o [!DNL Jira)]) cuentan con el campo [!UICONTROL Conexión]. Aquí puede especificar la conexión que desea que utilice este módulo para conectarse a la aplicación. Puede seleccionar una conexión existente en la lista desplegable o crear una nueva conexión.

Cuando selecciona o crea una conexión para una aplicación en un escenario concreto, otros módulos para esa aplicación utilizan automáticamente la misma conexión, a menos que seleccione una diferente al configurar los módulos posteriores.

Para más información, consulte [Información general sobre conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Para crear una conexión dentro de un módulo [!DNL Workfront Fusion]:

1. Haga clic en **[!UICONTROL Añadir]** para abrir el cuadro **[!UICONTROL Crear una conexión]**.
1. (Opcional) Cambie el **[!UICONTROL nombre de conexión]** predeterminado.
1. (Condicional) Si la aplicación requiere configuraciones avanzadas de conexión, como un ID, clave o [!UICONTROL secreto], ingrese esa información.

   Es posible que deba haga clic en **[!UICONTROL Mostrar configuraciones avanzadas]** para ver los campos donde puede ingresar este tipo de información.

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana de inicio de sesión que aparece, introduzca sus credenciales para iniciar sesión en la aplicación si aún no lo ha hecho.
1. (Condicional) Si aparece el botón **[!UICONTROL Permitir]**, examine las acciones que podrá realizar el conector y, a continuación, haga clic en el botón para conectar la aplicación a [!DNL Workfront Fusion].
1. Continúe en [Configuración del módulo](#configure-the-module).


## Configuración del módulo

1. En los campos que se encuentran debajo del campo Conexión, configure los ajustes del módulo y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Estos ajustes son diferentes para cada módulo. El título en negrita indica una configuración requerida.

   >[!TIP]
   >
   >A medida que trabaja en su escenario, puede hacer clic en el módulo para mostrar este cuadro de configuración en cualquier momento.
   >
   >
   >Si ve un círculo negro en un módulo, aún no ha terminado de configurar sus opciones. Haga clic en el módulo para abrirlo y continuar configurando.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Si va a añadir el primer módulo al escenario, seleccione una opción para indicar dónde desea que comience el escenario cada vez que se ejecute.

   ![](assets/choose-where-start-350x194.png)

1. Repita los pasos de las secciones [Añadir un módulo a un escenario](#add-a-module-in-a-scenario) y [Configuración del módulo](#configure-the-module) para añadir otros módulos al escenario.

1. (Opcional) Copie y pegue un módulo o grupo de módulos.

   Para obtener más información, consulte [Copiar módulos o escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continúe con [Configurar y trabajar con su escenario](#configure-and-work-with-your-scenario).

## Configurar y trabajar con su escenario

1. Realice cualquiera de las siguientes acciones para configurar su escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Especifique cuándo y con qué frecuencia se ejecutará el escenario</td> 
      <td> <p>Haga clic en el icono de reloj. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de una ruta</td> 
      <td> <p>Haga clic en el icono de llave inglesa <img src="assets/wrench-icon.gif"> entre los dos módulos y utilice cualquiera de las siguientes opciones. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Set up a filter]</strong>: controle qué paquetes se utilizan en determinados puntos del escenario.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: quita una ruta.</li> 
        <li><strong>[!UICONTROL Add a router]</strong>: añade un enrutador entre módulos. </li> 
        <li><strong>[!UICONTROL Add a module]</strong>: añade un módulo nuevo entre módulos.</li> 
        <li><strong>[!UICONTROL Add a note]</strong>: añade una nota a la ruta.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Establecer la configuración del escenario</td> 
      <td>Haga clic en el icono [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Esta configuración está dirigida principalmente a usuarios avanzados. Para obtener más información, consulte el <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">panel Ajustes de escenario en [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de control de flujo</td> 
      <td> <p>Haga clic en el icono [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Puede configurar una tarea para que se repita un número determinado de veces, convertir una matriz en una serie de paquetes y combinar varios paquetes en uno solo. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Control de flujo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mejorar el escenario con herramientas avanzadas</td> 
      <td>Haga clic en el icono [!DNL Tools]. <img src="assets/tools-icon.gif"> Puede crear activadores, acciones, agregadores y transformadores. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herramientas de análisis de texto de usuario</td> 
      <td>Haga clic en el icono [!DNL Text parser]<img src="assets/text-parser-icon.gif"> Puede recuperar elementos del código de HTML, buscar y extraer elementos de cadena que coincidan con un patrón de búsqueda, buscar y reemplazar texto y realizar un “raspado” de datos de un sitio web. Para obtener más información, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Herramientas</a>.</td> 
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
      <td> <p>Haga clic en la flecha <img src="assets/exit-editing-arrow.png"> de [!UICONTROL Exit editing] en el editor de escenarios para ver la página de detalles de Escenario. El registro se muestra en la parte inferior de la ventana o en la esquina inferior derecha. Contiene información sobre cada fase y los errores encontrados durante la ejecución del escenario.</p> <p>Para volver a trabajar con su escenario en [!DNL scenario editor], haga clic en cualquier lugar de la página de detalles Escenario.</p> <p>Para obtener más información acerca de la página de detalles del escenario, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalles del escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceder a las aplicaciones y servicios más utilizados</td> 
      <td> Haga clic en un icono de la sección <strong>[!UICONTROL Favorites]</strong> en la parte inferior de la pantalla. Los iconos se muestran en esta sección automáticamente cuando se añaden aplicaciones y servicios al escenario. También puede hacer clic en el icono [!UICONTROL Add] <img src="assets/add-icon.gif"> para añadir aplicaciones y servicios a esta área de forma manual.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver una animación que muestra cómo fluyen los datos a través del escenario</td> 
      <td>Haga clic en el icono <img src="assets/explain-flow-airplane-icon.gif"> de [!UICONTROL Explain flow].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinear automáticamente del diseño de los módulos </td> 
      <td>Haga clic en el icono [!UICONTROL Auto-align] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Escribir o ver notas sobre el escenario</td> 
      <td>Haga clic en el icono de [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminación de un módulo</td> 
      <td>Haga clic con el botón derecho del ratón en el módulo y, a continuación, haga clic en <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para probar el escenario, haga clic en **[!UICONTROL Ejecutar una vez]**.

   Es importante verificar que el escenario se ejecuta como espera antes de activarlo. Una vez activado, el escenario se ejecutará según su programación. Si todo no funciona según lo esperado, consulte [Control de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Cuando termine de editar el escenario (o en cualquier momento mientras lo está editando), haga clic en el icono [!UICONTROL Guardar] en la parte inferior de la ventana ![](assets/save-icon.gif).

Para obtener información acerca de cómo activar un escenario, consulte [Activar o desactivar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

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
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl + Mayús + S</td> 
   <td><span style="font-weight: normal;">Cmd + Mayús + S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Run Once]</td> 
   <td>Ctrl + Mayús + Intro</td> 
   <td><span style="font-weight: normal;">Cmd + Mayús + Entrar</span> </td> 
  </tr> 
 </tbody> 
</table>
