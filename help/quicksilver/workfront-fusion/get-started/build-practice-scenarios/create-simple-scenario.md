---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Cree un escenario básico en [!DNL Adobe Workfront Fusion]
description: Aprenda a crear un escenario de automatización sencillo con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo muestra el proceso de creación de un escenario que busca un [!DNL Workfront] en Workfront y la convierte en un proyecto.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Cree un escenario básico en [!DNL Adobe Workfront Fusion]

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que cree inspecciona los datos de una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Este ejemplo muestra el proceso de creación de un escenario que busca un [!DNL Workfront] en Workfront y la convierte en un proyecto.

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

1. En el **Escenarios** , haga clic en **Crear un nuevo escenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Se muestra el editor de escenarios, que contiene un módulo vacío en el centro.

   <!--picture?-->

1. Seleccione el **[!UICONTROL Nuevo escenario]** nombre del marcador de posición en la esquina superior izquierda y, a continuación, escriba un nombre.
1. Continuar con [Adición y configuración del primer módulo](#add-and-configure-the-first-module) más abajo.

### Adición y configuración del primer módulo

1. Haga clic en el módulo vacío para elegir la aplicación desde la que seleccionará un módulo.

   A la derecha del módulo aparece una lista de aplicaciones.

1. Seleccionar **[!DNL Adobe Workfront]**. Si no está visible, haga clic en la barra de búsqueda situada en la parte inferior de la lista, escriba &quot;Workfront&quot; y selecciónela cuando aparezca en la lista.

   La lista cambia para mostrar todo [!DNL Workfront] módulos que puede utilizar.

1. Haga clic en **[!UICONTROL Buscar]** módulo.

   Se abrirá la ventana de configuración del módulo.

1. En el [!UICONTROL Conexión] , seleccione la conexión de Workfront.

   Si no tiene una conexión de Workfront, consulte [Cree una conexión con [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. En el [!UICONTROL Tipo de registro] , seleccione **[!UICONTROL Tarea]**. Esto configura el módulo para que busque solo tareas.

   Puede encontrar **[!UICONTROL Tarea]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL tarea].&quot;

1. En el **[!UICONTROL Conjunto de resultados]** , seleccione **[!UICONTROL Primer registro coincidente]**.

   Esto configura el módulo para que devuelva únicamente el primer registro que encuentre que cumpla los criterios.
1. En el **[!UICONTROL Criterios de búsqueda]** , configure los criterios para devolver la tarea específica.

   1. En el primer cuadro debajo de [!UICONTROL Criterios de búsqueda], seleccione el campo que desee incluir en la búsqueda. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.

      Puede encontrar **[!UICONTROL Nombre]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL name].&quot;
   1. Para el operador, haga clic en la flecha desplegable situada junto a **Existe** y cámbielo por [!UICONTROL **Contiene (sin distinción de mayúsculas)**].

      Esto permite que el módulo encuentre proyectos con las palabras elegidas en el nombre, aunque no introduzca el nombre completo o el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas).
   1. En el último campo debajo de [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre de la tarea que está buscando.

1. En el **[!UICONTROL Salidas]** , seleccione los campos de salida que desea que muestre el módulo. Para este ejemplo, seleccione **[!UICONTROL ID]** y **[!UICONTROL Nombre]** campos.

   >[!TIP]
   >
   >Puede utilizar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Clic **[!UICONTROL OK]** para guardar la configuración del módulo.

1. Haga clic con el botón derecho en el módulo y seleccione **[!UICONTROL Cambiar nombre]**, escriba un nombre y describa lo que desea que haga el módulo (por ejemplo, &quot;Buscar tarea&quot;) y haga clic en **[!UICONTROL OK]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continuar con [Adición y configuración del segundo módulo](#add-and-configure-the-second-module).

## Adición y configuración del segundo módulo

1. Pase el ratón sobre el círculo parcial a la derecha del del módulo y haga clic en **[!UICONTROL Añadir otro módulo]**.
1. Seleccionar [!DNL Adobe Workfront] en la lista de aplicaciones, elija el módulo **[!UICONTROL Convertir objeto]**.
1. En el [!UICONTROL Conexión] , seleccione la misma conexión de Workfront que utilizó en el módulo anterior
1. En el **[!UICONTROL Tipo de registro]** , seleccione **[!UICONTROL Tarea]**, porque el módulo convertirá una tarea.
1. En el **[!UICONTROL Convertir a]** , seleccione **Proyecto**.
1. Junto al campo ID de tarea, haga clic en el botón de alternancia de asignación para habilitarlo.

   La opción se vuelve azul cuando está habilitada. Esto le permite asignar el ID de tarea del módulo anterior.

   ![Alternar mapa](assets/map-toggle.png)
1. Haga clic en **[!UICONTROL Identificador de tarea]** field.

   Se abre un panel que le permite seleccionar qué utilizar como ID de la tarea que desea convertir en proyecto. Dado que ha habilitado la asignación, el panel incluye la salida de cualquier módulo anterior. Ha seleccionado ID como salida del módulo anterior, por lo que ahora está disponible en el panel.

   Este panel se denomina panel de asignación. Para obtener más información sobre el panel de asignación, consulte [Asignación de información de un módulo a otro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleccionar **ID** en el panel de asignación.

   Aparece un bloque de ID en el campo ID. Muestra el número del módulo desde el que está asignado y el campo asignado.

   ![ID de mapa](assets/map-id.png)

1. Haga clic en **Identificador de plantilla** , empiece a escribir el nombre de la plantilla de Workfront que desea utilizar para este proyecto y selecciónela cuando aparezca en la lista.
1. Clic **[!UICONTROL OK]** para guardar la configuración del módulo.

1. Haga clic con el botón derecho en el módulo y seleccione **[!UICONTROL Cambiar nombre]** A continuación, escriba un nombre y describa lo que desea que haga el módulo (como &quot;Convertir en proyecto&quot;) y haga clic en **[!UICONTROL OK]**.

1. Continuar a [Prueba del escenario](#test-the-scenario).

## Prueba del escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

En este caso, una prueba que se realice correctamente buscaría la nueva tarea y la convertiría en un proyecto.

1. Clic **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo para poder ver información sobre el paquete de datos que ha procesado el módulo, incluidos los datos extraídos de la tarea que ha devuelto el módulo.

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada (la tarea) y la salida (el proyecto convertido).

   Para obtener más información sobre los datos de las burbujas de inspección, consulte:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información sobre los paquetes procesados, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Entrada [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar el progreso del escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón derecho en [!DNL Workfront] módulo y haga clic en **[!UICONTROL Añadir una nota]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Puede agregar varias notas para un módulo.
>
>1. Cierre el **[!UICONTROL Notas]** área.
>
>     Después de agregar una nota a un escenario, aparece un punto naranja en la etiqueta **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) para ver las notas.
>

## Activación del escenario

El último paso para crear un escenario es activarlo.

Dado que este escenario busca una tarea específica, no es necesario activarla. La activación de un escenario hace que se ejecute en una programación o cuando se produce una acción específica en una aplicación. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre la activación de escenarios, consulte [Activación o desactivación de un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Pasos siguientes

* [Añadir un módulo de déclencheur](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
* Agregue un webhook para permitir que el escenario se ejecute cada vez que se ingrese una solicitud.
* Agregue un filtro para asegurarse de que solo determinadas solicitudes se conviertan en proyectos.
* Agregue una función que personalice el nombre del nuevo proyecto.
* Añada la gestión de errores para garantizar que el escenario sea resistente a los errores.

