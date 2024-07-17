---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crear un escenario simple en  [!DNL Adobe Workfront Fusion]
description: Aprenda a crear un escenario de automatización sencillo con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo muestra el proceso de creación de un escenario que busca un problema y lo convierte en un proyecto.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# Crear un escenario básico en [!DNL Adobe Workfront Fusion]

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que cree inspecciona los datos de una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Este ejemplo muestra el proceso de creación de un escenario que busca un problema en Workfront y luego lo convierte en un proyecto.

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
1. En el cuadro [!UICONTROL Tipo de registro], seleccione **[!UICONTROL Problema]**. Esto configura el módulo para que solo busque problemas.

   Puede encontrar **[!UICONTROL Problema]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL problema]&quot;.

1. En el cuadro **[!UICONTROL Conjunto de resultados]**, seleccione **[!UICONTROL Primer registro coincidente]**.

   Esto configura el módulo para que devuelva únicamente el primer registro que encuentre que cumpla los criterios.
1. En el área **[!UICONTROL Criterios de búsqueda]**, configure los criterios para devolver el problema específico.

   1. En el primer cuadro bajo [!UICONTROL Criterios de búsqueda], seleccione el campo que desee incluir en la búsqueda. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.

      Puede encontrar **[!UICONTROL Name]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL name]&quot;.
   1. Para el operador, haga clic en la flecha desplegable junto a **Existe** y cambie a [!UICONTROL **Contiene (sin distinción de mayúsculas y minúsculas)**].

      Esto permite que el módulo encuentre proyectos con las palabras elegidas en el nombre, aunque no introduzca el nombre completo o el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas).
   1. En el último campo bajo [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre del problema que está buscando.

1. En la lista **[!UICONTROL Resultados]**, seleccione los campos de los que desea que salga el módulo. Para este ejemplo, seleccione los campos **[!UICONTROL ID]** y **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Buscar problema&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/)

1. Continúe con [Agregar y configurar el segundo módulo](#add-and-configure-the-second-module).

## Adición y configuración del segundo módulo

1. Pase el ratón sobre el círculo parcial a la derecha del del módulo y luego haga clic en **[!UICONTROL Agregar otro módulo]**.
1. Seleccione [!DNL Adobe Workfront] de la lista de aplicaciones y, a continuación, elija el módulo **[!UICONTROL Misc Action]**.

   El módulo de Misc Action permite realizar acciones en Workfront que no tienen un módulo dedicado. En este ejemplo, este módulo se utiliza para convertir el problema en un proyecto.
1. En el campo [!UICONTROL Conexión], seleccione la misma conexión de Workfront que utilizó en el módulo anterior
1. En el campo **[!UICONTROL Tipo de registro]**, seleccione **[!UICONTROL Problema]**, porque la acción que se va a realizar está relacionada con un problema.
1. En el campo **[!UICONTROL Acción]**, seleccione **convertToProject**. Esta es la acción que convertirá el problema seleccionado en un proyecto.
1. Haga clic en el campo **[!UICONTROL ID]**.

   Se abre un panel que le permite seleccionar qué usar como ID del problema que desea convertir en un proyecto. El panel incluye los resultados de cualquier módulo anterior. Dado que seleccionó ID como salida del módulo anterior, ahora está disponible en el panel.

   Este panel se denomina panel de asignación. Para obtener más información sobre el panel de asignación, vea [Asignar información de un módulo a otro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleccione **ID** en el panel de asignación.

   Aparece un bloque de ID en el campo ID. Muestra el número del módulo desde el que está asignado y el campo asignado.

   ![Id. de mapa](assets/map-id.png)

1. (Opcional) En la sección Proyecto, busque el campo ID de propietario, empiece a escribir su nombre en el campo y, a continuación, selecciónelo cuando aparezca. Esto le establecerá como propietario del proyecto y facilitará la búsqueda en Workfront.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del módulo.

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Convertir en proyecto&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

1. Continuar a [Probar el escenario](#test-the-scenario).

## Prueba del escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

En este caso, una prueba que se realice correctamente buscaría el problema y lo convertiría en un proyecto.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo para poder ver información sobre el paquete de datos que ha procesado el módulo, incluidos los datos extraídos del problema que ha devuelto el módulo.

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada (el problema) y la salida (el proyecto convertido).

   Para obtener más información sobre los datos de las burbujas de inspección, consulte:

   * Para obtener información general, vea [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, vea [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

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

Dado que este escenario busca un problema específico, no es necesario activarlo. La activación de un escenario hace que se ejecute en una programación o cuando se produce una acción específica en una aplicación. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activar o desactivar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
