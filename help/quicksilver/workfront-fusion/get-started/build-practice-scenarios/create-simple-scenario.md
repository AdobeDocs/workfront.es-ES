---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crear un escenario básico en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 06fa7e15-b8dc-4fe1-9703-c160d580ef79
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1328'
ht-degree: 94%

---

# Crear un escenario básico en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Crear un escenario básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/create-basic-scenario.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que crea ve los datos de una aplicación o servicio y los procesa para proporcionar el resultado deseado.

Este ejemplo le guiará por el proceso de creación de un escenario que busca una tarea de [!DNL Workfront] en Workfront y la convierte en un proyecto.

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

### Empiece a crear el escenario

1. En el área **Escenarios**, haga clic en **Crear un nuevo escenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Se mostrará el editor de escenarios, que contiene un módulo vacío en el centro.

   <!--picture?-->

1. Seleccione el nombre del marcador de posición **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y, a continuación, escriba un nombre.
1. Continúe con [Añadir y configurar el primer módulo](#add-and-configure-the-first-module).

### Añadir y configurar el primer módulo

1. Haga clic en el módulo vacío para elegir la aplicación desde la que seleccionará un módulo.

   A la derecha del módulo aparece una lista de aplicaciones.

1. Seleccionar **[!DNL Adobe Workfront]**. Si no está visible, haga clic en la barra de búsqueda en la parte inferior de la lista, escriba “Workfront” y selecciónela cuando aparezca en la lista.

   La lista cambia para mostrar todos los módulos de [!DNL Workfront] que puede utilizar.

1. Haga clic en el módulo **[!UICONTROL Buscar]**.

   Se abrirá la ventana de configuración del módulo.

1. En el cuadro [!UICONTROL Conexión], seleccione su conexión de Workfront.

   Si no tiene una conexión de Workfront, consulte [Crear una conexión con [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. En el cuadro [!UICONTROL Tipo de registro], seleccione **[!UICONTROL Tarea]**. Esto configura el módulo para que busque solo tareas.

   Puede encontrar **[!UICONTROL Tarea]** en la lista si empieza a escribir la palabra “[!UICONTROL tarea]”.

1. En el cuadro **[!UICONTROL Conjunto de resultados]**, seleccione **[!UICONTROL Primer registro coincidente]**.

   Se configura el módulo para que devuelva únicamente el primer registro que encuentre que cumple los criterios.
1. En el área **[!UICONTROL Criterios de búsqueda]**, configure los criterios para que devuelvan la tarea específica.

   1. En el primer cuadro debajo de [!UICONTROL Criterios de búsqueda], seleccione el campo que desea incluir en la búsqueda. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.

      Puede encontrar **[!UICONTROL Name]** en la lista si empieza a escribir la palabra “[!UICONTROL name]”.
   1. Para el operador, haga clic en la flecha desplegable junto a **Existe** y cambie a [!UICONTROL **Contiene (sin distinción de mayúsculas y minúsculas)**].

      Esto permite que el módulo encuentre proyectos con las palabras que elija en el nombre, incluso si no introduce el nombre completo o si introduce el nombre con mayúsculas o minúsculas incorrectas (como, por ejemplo, todo mayúsculas).
   1. En el último campo debajo de [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre de la tarea que está buscando.

1. En la lista **[!UICONTROL Resultados]**, seleccione los campos de los que desea que salga el módulo. Para este ejemplo, seleccione los campos **[!UICONTROL ID]** y **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para encontrar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón derecho en el módulo, haga clic en **[!UICONTROL Cambiar nombre]** y escriba un nombre que describa lo que desea que haga el módulo (como “Buscar tarea”) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continúe con [Añadir y configurar el segundo módulo](#add-and-configure-the-second-module).

## Añadir y configurar el segundo módulo

1. Pase el puntero por encima del círculo parcial a la derecha del módulo y luego haga clic en **[!UICONTROL Añadir otro módulo]**.
1. Seleccione [!DNL Adobe Workfront] de la lista de aplicaciones y luego elija el módulo **[!UICONTROL Convertir objeto]**.
1. En el campo [!UICONTROL Conexión], seleccione la misma conexión de Workfront que ha utilizado en el módulo anterior.
1. En el campo **[!UICONTROL Tipo de registro]**, seleccione **[!UICONTROL Tarea]**, ya que el módulo convertirá una tarea.
1. En el campo **[!UICONTROL Convertir en]**, seleccione **Proyecto**.
1. Junto al campo Identificador de tarea, haga clic en el conmutador de asignación para habilitarlo.

   El conmutador se vuelve azul cuando está habilitado. Esto le permite asignar el Identificador de tarea del módulo anterior.

   ![Conmutador Asignar](assets/map-toggle.png)
1. Haga clic en el campo **[!UICONTROL Identificador de tarea]**.

   Se abre un panel que le permite seleccionar qué utilizar como identificador de la tarea que desea convertir en proyecto. Dado que ha habilitado la asignación, el panel incluye la salida de cualquier módulo anterior. Ha seleccionado ID como salida del módulo anterior, por lo que ahora está disponible en el panel.

   Este panel se denomina panel de asignación. Para obtener más información sobre el panel de asignación, consulte [Asignar información de un módulo a otro en ](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleccione **ID** en el panel de asignación.

   Aparece un bloque de ID en el campo ID. Muestra el número del módulo desde el que se asigna y el campo que se asigna.

   ![Identificador de asignación](assets/map-id.png)

1. Haga clic en el campo **Identificador de plantilla**, empiece a escribir el nombre de la plantilla de Workfront que desea utilizar para este proyecto y, a continuación, selecciónela cuando aparezca en la lista.
1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como “Convertir en proyecto”) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

1. Continuar para [Probar el escenario](#test-the-scenario).

## Probar el escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

En este caso, una prueba que se realice correctamente buscaría la nueva tarea y la convertiría en un proyecto.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo para poder ver información sobre el paquete de datos que ha procesado el módulo, incluidos los datos extraídos de la tarea que ha devuelto el módulo.

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada (la tarea) y la salida (el proyecto convertido).

   Para obtener más información sobre los datos de las burbujas de inspección, consulte lo siguiente:

   * Para obtener información general, consulte [Flujo de ejecución del escenario en  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, consulte [Ejecución de escenarios, ciclos y fases en  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Se recomienda guardar con frecuencia mientras se perfeccionan y prueban escenarios.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de añadir notas sobre cada módulo.
>
>1. Haga clic con el botón derecho en un módulo de [!DNL Workfront] y luego haga clic en **[!UICONTROL Añadir una nota]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Puede añadir varias notas para un módulo.
>
>1. Cierre el área **[!UICONTROL Notas]**.
>
>     Después de añadir una nota a un escenario, aparece un punto naranja en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para ver sus notas.
>

## Activar el escenario

El último paso para crear un escenario es activarlo.

Dado que este escenario busca una tarea específica, no es necesario activarla. La activación de un escenario hace que se ejecute en una programación o cuando se produce una acción específica en una aplicación. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activación o desactivación de un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programación de un escenario en [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Pasos siguientes

* [Añada un módulo de activador](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
* Añada un webhook para permitir que el escenario se ejecute cada vez que se introduzca una solicitud.
* Añada un filtro para asegurarse de que solo determinadas solicitudes se conviertan en proyectos.
* Añada una función que personalice el nombre del nuevo proyecto.
* Añada la gestión de errores para garantizar que el escenario sea resistente a los errores.
