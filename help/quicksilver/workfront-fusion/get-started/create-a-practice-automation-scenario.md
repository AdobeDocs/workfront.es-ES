---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crear un escenario de automatización de práctica en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 95%

---

# Crear un escenario de automatización de práctica en [!DNL Adobe Workfront Fusion]

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

Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este artículo explica el proceso de creación de un escenario que busca un proyecto y, a continuación, devuelve todas las tareas asociadas a dicho proyecto.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

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

## Crear un escenario de práctica de automatización

[!DNL Adobe Workfront Fusion] le ayuda a centrarse en tareas importantes mediante la automatización de las repetidas. Crea escenarios que administran automáticamente los datos en varias aplicaciones y servicios.

Cada escenario consta de módulos que guían el modo en que los datos se procesan dentro de una aplicación o se transfieren entre diferentes aplicaciones y servicios. Por ejemplo, puede crear un escenario en Fusion para buscar automáticamente un proyecto de [!DNL Workfront] y enumerar sus tareas. De este modo, Fusion le ahorra tiempo y esfuerzo al gestionar las tareas rutinarias.

Este escenario de práctica explica el proceso de creación de un escenario que busca un proyecto de [!DNL Workfront] y devuelve las tareas del proyecto.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Antes de comenzar

Cree un proyecto con tareas en Workfront que pueda usar para este ejercicio. No es necesario que realice ninguna configuración adicional aparte de añadir tareas al proyecto.

Para obtener información sobre la creación de un proyecto en Workfront, consulte xxx.

### 1. Cree un escenario y asígnele un nombre

1. Inicie sesión en la cuenta de [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   >[!NOTE]
   >
   >Si no ve el panel de navegación izquierdo o sus iconos, haga clic en el icono Menú ![Menu](assets/main-menu-icon-left-nav.png).

1. En el panel [!UICONTROL **Folders**], haga clic en el icono **[!UICONTROL Add folder]** ![](assets/add-folder-icon.png) y, a continuación, escriba un nombre como “Escenarios de práctica” para la primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Create a new scenario]** en la esquina superior derecha de la página.

1. Para este ejercicio, seleccione la aplicación **[!DNL Adobe Workfront]** y luego haga clic en **Buscar**, situado cerca de la parte inferior.


1. Seleccione el nombre del marcador de posición **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y, a continuación, escriba un nombre como “Práctica de escenario 1&quot;.

   ![](assets/name-the-scenario.png)

1. Continúe con el apartado siguiente [Conectar el primer módulo](#2-connect-the-first-module).

### 2. Conectar el primer módulo

Ahora debe establecer una conexión autenticada con la cuenta de [!DNL Workfront]. Cada módulo que añada a un escenario debe tener una conexión con su aplicación.

1. En el cuadro de **[!DNL Workfront]**, en **[!UICONTROL Connection]**, haga clic en **[!UICONTROL Add]**, escriba un nombre para la conexión, como “Cuenta de Workfront de Olivia”, y haga clic en **[!UICONTROL Continue]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. El siguiente proceso es específico de [!DNL Workfront], pero se parece al de muchas aplicaciones:

   1. Escriba su dominio de [!DNL Workfront] y haga clic en **[!UICONTROL Continuar]**.
   1. Inicie sesión en [!DNL Workfront].
   1. Examine el acceso que [!DNL Workfront Fusion] está solicitando y luego haga clic en **[!UICONTROL Permitir acceso]**.

   Si necesita ayuda, consulte [Información general sobre las conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configurar el primer módulo

Después de conectar [!DNL Workfront Fusion] a su cuenta de [!DNL Workfront], puede especificar un proyecto de [!DNL Workfront] al que tenga acceso y los datos que desea que procese el primer módulo.

1. En el cuadro [!UICONTROL Tipo de registro], seleccione **[!UICONTROL Proyecto]**. Se configura el módulo para buscar solo proyectos.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL proyecto]&quot;.

1. En el cuadro **[!UICONTROL Conjunto de resultados]**, seleccione **[!UICONTROL Primer registro coincidente]**. Se configura el módulo para que devuelva únicamente el primer registro que encuentre que cumple los criterios. Para este ejemplo, solo necesitamos devolver un registro.
1. En el área **[!UICONTROL Criterios de búsqueda]**, configuraremos un filtro para que devuelva el proyecto específico:

   | Campo | Acción |
   |--------|-------------|
   | Campos de criterios de búsqueda | Seleccione el campo en el que desea buscar los valores. Para este ejemplo, seleccione **[!UICONTROL Nombre]**. |
   | Criterios de búsqueda | En el primer menú desplegable, seleccione **[!UICONTROL Nombre]**. |
   | Operadores básicos | En la segunda lista desplegable, seleccione [!UICONTROL Contiene (sin distinción de mayúsculas y minúsculas)]. Esto permite que el módulo encuentre proyectos con las palabras que elija en el nombre, incluso si no introduce el nombre completo o si introduce el nombre con mayúsculas o minúsculas incorrectas (como, por ejemplo, todo mayúsculas). |
   | Cuadro de texto | Escriba una palabra o frase que sepa que está en el nombre del proyecto que está buscando. |

+++ Expanda para ver un ejemplo en pantalla.
   ![](assets/search-name.png)
+++

1. En la lista **[!UICONTROL Resultados]**, seleccione los campos que desea que el módulo genere. Para este ejemplo, seleccione los campos **[!UICONTROL ID]** y **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede utilizar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]**.

   >[!NOTE]
   >
   >Como no se trata de un módulo de activador, no debe elegir dónde iniciarlo. Si utiliza un módulo de activador, debería seleccionar dónde iniciarlo.
   >
   >
   >Para obtener más información, consulte [Elegir dónde se inicia un módulo de activador en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Buscar proyecto&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continúe con [Añadir y configurar el segundo módulo](#add-and-configure-the-second-module).

### 4. Añadir y configurar el segundo módulo

1. Haga clic en el círculo parcial a la derecha del del módulo para **[!UICONTROL Añadir otro módulo]**.
1. Seleccione [!DNL Workfront] en la lista de aplicaciones y después elija el módulo de búsqueda **[!UICONTROL Leer registros relacionados]**.
1. En el cuadro **[!UICONTROL Conexión]**, seleccione la conexión que creó para el módulo anterior. Debe asegurarse de que este módulo utiliza la misma conexión que el módulo anterior.
1. Haga clic en **[!UICONTROL Tipo de registro]** y, a continuación, seleccione **[!UICONTROL Proyecto]**, porque queremos leer registros relacionados con un proyecto.

   >[!TIP]
   >
   >Puedes encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;proyecto&quot;.

1. Haga clic en el campo **[!UICONTROL Id. de registro principal]**. Este campo necesita el identificador de Workfront del proyecto desde el que desea devolver las tareas.

   Al hacer clic en el campo, se abre la lista de variables que puede utilizar en el campo **[!UICONTROL Id. de registro principal]** para identificar el proyecto en Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Haga clic en la variable **[!UICONTROL ID]** para añadirla al campo **[!UICONTROL Id. de registro principal]**. Esto permite que el identificador devuelto por el primer módulo se utilice como identificador del proyecto con el que desea trabajar en el segundo módulo, lo que garantiza que las tareas devueltas pertenezcan a ese proyecto.
1. En el campo **[!UICONTROL Colecciones]**, seleccione **[!UICONTROL Tareas]**. Esto indica que el módulo debe devolver las tareas asociadas con el proyecto elegido.
1. En el campo **[!UICONTROL Outputs]**, seleccione **[!UICONTROL Id]** y **[!UICONTROL Name]**.
1. Haga clic **[!UICONTROL OK]**

   Ahora tiene un escenario de trabajo.

1. Asigne un nombre al segundo módulo, como &quot;Devolver tareas asociadas con el proyecto&quot; y, a continuación, continúe con [Probar el escenario](#test-the-scenario).

## Probar el escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Elegimos que se devolviera 1 proyecto, así como las tareas asociadas con dicho proyecto. Si ejecuta el escenario, eso es lo que debería suceder.

1. Haga clic en **[!UICONTROL Run once]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez termine de ejecutarse el escenario, haga clic en la burbuja situada encima del primer módulo.

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el conjunto de datos que procesó el módulo, incluidos los datos reales extraídos del proyecto que devolvió el módulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada de información y la salida, que es una recopilación de tareas incluidas en el proyecto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Puede obtener más información sobre cómo leer la información de ejecución de escenarios en los siguientes artículos:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Save]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

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

Este escenario de ejemplo no tiene un módulo de activador. Si este fuera un escenario que usaría para datos reales, empezaría con un módulo de activador y lo último que haría es activarlo. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activación o desactivación de un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
