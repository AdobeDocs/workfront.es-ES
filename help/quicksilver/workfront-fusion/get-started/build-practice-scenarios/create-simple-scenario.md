---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crear un escenario básico en  [!DNL Adobe Workfront Fusion]
description: Aprenda a crear un escenario de automatización sencillo con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo lo lleva a través del proceso de creación de un escenario que busca una  [!DNL Workfront] tarea en Workfront y luego la convierte en un proyecto.
author: Becky
feature: Workfront Fusion
exl-id: 06fa7e15-b8dc-4fe1-9703-c160d580ef79
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Crear un escenario básico en [!DNL Adobe Workfront Fusion]

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que cree inspecciona los datos de una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Este ejemplo lo lleva a través del proceso de creación de un escenario que busca una tarea [!DNL Workfront] en Workfront y luego la convierte en un proyecto.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Crear un escenario de práctica

### Empezar a crear el escenario

1. En el área **Escenarios**, haga clic en **Crear un nuevo escenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Se muestra el editor de escenarios, que contiene un módulo vacío en el centro.

   <!--picture?-->

1. Seleccione el nombre del marcador de posición **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y, a continuación, escriba un nombre.
1. Continúe con [Agregue y configure el primer módulo](#add-and-configure-the-first-module) a continuación.

### Adición y configuración del primer módulo

1. Haga clic en el módulo vacío para elegir la aplicación desde la que seleccionará un módulo.

   A la derecha del módulo aparece una lista de aplicaciones.

1. Seleccione **[!DNL Adobe Workfront]**. Si no está visible, haga clic en la barra de búsqueda situada en la parte inferior de la lista, escriba &quot;Workfront&quot; y selecciónela cuando aparezca en la lista.

   La lista cambia para mostrar todos los [!DNL Workfront] módulos que puede usar.

1. Haga clic en el módulo **[!UICONTROL Buscar]**.

   Se abrirá la ventana de configuración del módulo.

1. En el cuadro [!UICONTROL Conexión], seleccione su conexión de Workfront.

   Si no cuenta con una conexión de Workfront, consulte [Crear una conexión con [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. En el cuadro [!UICONTROL Tipo de registro], seleccione **[!UICONTROL Tarea]**. Esto configura el módulo para que busque solo tareas.

   Puede encontrar **[!UICONTROL Tarea]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL tarea]&quot;.

1. En el cuadro **[!UICONTROL Conjunto de resultados]**, seleccione **[!UICONTROL Primer registro coincidente]**.

   Esto configura el módulo para que devuelva únicamente el primer registro que encuentre que cumpla los criterios.
1. En el área **[!UICONTROL Criterios de búsqueda]**, configure los criterios para devolver la tarea específica.

   1. En el primer cuadro bajo [!UICONTROL Criterios de búsqueda], seleccione el campo que desee incluir en la búsqueda. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.

      Puede encontrar **[!UICONTROL Name]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL name]&quot;.
   1. Para el operador, haga clic en la flecha desplegable junto a **Existe** y cambie a [!UICONTROL **Contiene (sin distinción de mayúsculas y minúsculas)**].

      Esto permite que el módulo encuentre proyectos con las palabras elegidas en el nombre, aunque no introduzca el nombre completo o el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas).
   1. En el último campo bajo [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre de la tarea que está buscando.

1. En la lista **[!UICONTROL Resultados]**, seleccione los campos de los que desea que salga el módulo. Para este ejemplo, seleccione los campos **[!UICONTROL ID]** y **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Buscar tarea&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continúe con [Agregar y configurar el segundo módulo](#add-and-configure-the-second-module).

## Adición y configuración del segundo módulo

1. Pase el ratón sobre el círculo parcial a la derecha del del módulo y luego haga clic en **[!UICONTROL Agregar otro módulo]**.
1. Seleccione [!DNL Adobe Workfront] de la lista de aplicaciones y luego elija el módulo **[!UICONTROL Convertir objeto]**.
1. En el campo [!UICONTROL Conexión], seleccione la misma conexión de Workfront que utilizó en el módulo anterior
1. En el campo **[!UICONTROL Tipo de registro]**, seleccione **[!UICONTROL Tarea]**, ya que el módulo convertirá una tarea.
1. En el campo **[!UICONTROL Convertir en]**, seleccione **Proyecto**.
1. Junto al campo ID de tarea, haga clic en el botón de alternancia de asignación para habilitarlo.

   La opción se vuelve azul cuando está habilitada. Esto le permite asignar el ID de tarea del módulo anterior.

   ![Alternar mapa](assets/map-toggle.png)
1. Haga clic en el campo **[!UICONTROL Identificador de tarea]**.

   Se abre un panel que le permite seleccionar qué utilizar como ID de la tarea que desea convertir en proyecto. Dado que ha habilitado la asignación, el panel incluye la salida de cualquier módulo anterior. Ha seleccionado ID como salida del módulo anterior, por lo que ahora está disponible en el panel.

   Este panel se denomina panel de asignación. Para obtener más información sobre el panel de asignación, vea [Asignar información de un módulo a otro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleccione **ID** en el panel de asignación.

   Aparece un bloque de ID en el campo ID. Muestra el número del módulo desde el que está asignado y el campo asignado.

   ![Id. de mapa](assets/map-id.png)

1. Haga clic en el campo **Id. de plantilla**, empiece a escribir el nombre de la plantilla de Workfront que desea usar para este proyecto y, a continuación, selecciónela cuando aparezca en la lista.
1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Convertir en proyecto&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

1. Continuar a [Probar el escenario](#test-the-scenario).

## Prueba del escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

En este caso, una prueba que se realice correctamente buscaría la nueva tarea y la convertiría en un proyecto.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo para poder ver información sobre el paquete de datos que ha procesado el módulo, incluidos los datos extraídos de la tarea que ha devuelto el módulo.

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada (la tarea) y la salida (el proyecto convertido).

   Para obtener más información sobre los datos de las burbujas de inspección, consulte:

   * Para obtener información general, vea [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, vea [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón secundario en un módulo de [!DNL Workfront] y luego haga clic en **[!UICONTROL Agregar una nota]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Puede agregar varias notas para un módulo.
>
>1. Cierre el área **[!UICONTROL Notas]**.
>
>     Después de agregar una nota a un escenario, aparece un punto naranja en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para ver sus notas.
>

## Activación del escenario

El último paso para crear un escenario es activarlo.

Dado que este escenario busca una tarea específica, no es necesario activarla. La activación de un escenario hace que se ejecute en una programación o cuando se produce una acción específica en una aplicación. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activar o desactivar un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Pasos siguientes

* [Agregue un módulo de déclencheur](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
* Agregue un webhook para permitir que el escenario se ejecute cada vez que se ingrese una solicitud.
* Agregue un filtro para asegurarse de que solo determinadas solicitudes se conviertan en proyectos.
* Agregue una función que personalice el nombre del nuevo proyecto.
* Añada la gestión de errores para garantizar que el escenario sea resistente a los errores.
