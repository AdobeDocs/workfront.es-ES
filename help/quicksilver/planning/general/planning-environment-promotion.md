---
title: Utilizar la promoción de entorno para Adobe Workfront Planning
description: Puede copiar espacios de trabajo, tipos de registros, campos y vistas de Workfront Planning de un entorno de Workfront a otro mediante las funciones de promoción de entornos. En lugar de reconstruir todo a mano, se monta la configuración en un paquete en el entorno de origen y se instala en el entorno de destino.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 4%
---

# Utilizar la promoción de entorno para Adobe Workfront Planning

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Workfront Planning. Su empresa debe adquirir un paquete de Planning adicional para acceder a Workfront Planning.
>
>La funcionalidad que se describe aquí no está disponible si su organización ha adquirido Workfront Planning como producto independiente.
>
>Para obtener información general sobre Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

Puede copiar espacios de trabajo, tipos de registros, campos y vistas de Workfront Planning de un entorno de Workfront a otro mediante las funciones de promoción de entornos.

En lugar de reconstruir todo a mano, se monta la configuración en un paquete en el entorno de origen y se instala en el entorno de destino.

Utilizar la promoción del entorno con Planning es similar a usarlo para Workfront. Para obtener más información, consulte la sección &quot;Promoción de entorno&quot; en el artículo [Entornos de prueba de Adobe Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md).

## Consideraciones sobre el uso de Promoción de entornos con Planning

* Debe ser administrador de Workfront para usar Promoción de entorno.
* Se importan los siguientes elementos mediante la promoción del entorno:

  * Espacios de trabajo
  * Secciones de Workspace
  * Tipos de registro
  * Campos
  * Vistas
  * Jerarquías
  * Compartir la configuración de todos los objetos
  * Automatizaciones <!--this might not be part of it; Lilit is checking-->
  * Formularios de solicitud
  * Reglas empresariales
  * Objetos conectados
  * Objetos de los que depende el espacio de trabajo o con los que se comparten otros objetos, como grupos, equipos o roles. Se dan los siguientes escenarios:

    * Si ya existe un objeto con el mismo nombre en el entorno de destino, Workfront indica un conflicto y usted decide cómo manejarlo.
    * Si un equipo o un grupo con el que se comparte un objeto no existe en el entorno de destino, la promoción lo crea.
* Para cada objeto, puede hacer lo siguiente:

  * Créela como un objeto nuevo
  * Utilice el objeto existente pero créelo con un nombre nuevo
  * Sobrescribir un objeto existente. La sobrescritura reemplaza la configuración en el destino.

* La instalación puede tardar unos minutos. Puede revertir una instalación desde la página de resultados si es necesario.
* Se recomienda probar el proceso antes de continuar, cuando sea posible. Puede realizar la instalación en una zona protegida o un entorno de vista previa antes de promocionarlo a Producción.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Paquete de flujo de trabajo de Prime o Ultimate con un paquete de planificación de Prime o Ultimate</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación</p></td> 
   <td><p>Estándar de planificación</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>  
   <p>Debe ser administrador del sistema</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en espacios de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Importar la configuración de Planning mediante Promoción de entorno

A continuación se indican los pasos principales para promocionar la configuración de Planning a otro entorno:

* [Crear un paquete en el entorno de origen](#create-a-package-in-the-source-environment)
* [Preparar el paquete para la instalación](#make-the-package-ready-to-install)
* [Instalación del paquete en el entorno de destino](#install-the-package-in-the-target-environment)
* [Verificar los resultados](#verify-the-results)

Siga las instrucciones de las secciones siguientes para copiar una configuración de Planning entre dos entornos de Workfront.

### Creación de un paquete en el entorno de origen

1. Tenga un entorno de origen en el que la configuración deseada esté implementada.
1. En el entorno de origen, haga clic en el **Menú principal** ![Menú principal](assets/main-menu-shell.png) y, a continuación, vaya a **Configuración** > **Sistema** > **Promoción del entorno**.
La lista **Paquetes de configuración** muestra los paquetes existentes con su estado, entorno de origen y donde se implementaron.
1. Haga clic en **Crear paquete**.

   >[!TIP]
   >
   >Un paquete necesita al menos un objeto para poder ensamblarlo e instalarlo.
1. En la ficha **Detalles del paquete**, escriba un **Nombre** y una **Descripción** para el paquete. El entorno de origen ya se ha rellenado con el entorno actual (origen).
1. En la lista de tipos de objetos de la izquierda, seleccione **Espacio de trabajo de Planning**.
1. Busque el área de trabajo que desea promocionar, seleccione su casilla de verificación y haga clic en **Agregar área de trabajo de Planning**. El área de trabajo aparece en **Contenido del paquete**.

   ![Workspace seleccionado para la promoción de entorno](assets/workspace-selected-for-environment-promotion.png)
1. Haga clic en **Guardar y ensamblar**.

   Workfront ensambla el paquete y agrega una entrada en la ficha **Actualizaciones** del paquete. Puede revisar lo que el paquete incluye en la pestaña Contenido.
1. (Condicional y opcional) Haga clic en **Guardar y cerrar** si desea terminar más tarde.
1. (Opcional) Haga clic en **Contenido** para revisar el contenido del paquete o haga clic en **Implementaciones** para ver si este paquete se ha implementado varias veces.

   Siga preparando el paquete para la instalación.

### Preparar el paquete para la instalación

Antes de instalar el paquete en el entorno de destino, le recomendamos que lo pruebe en un entorno de prueba.

1. Una vez que el paquete haya terminado de compilarse como se describe en la sección anterior, haz clic en **Detalles del paquete**, haz clic en **Editar**, establece el **Estado** en **Pruebas** y, a continuación, haz clic en **Guardar y cerrar**.

   >[!TIP]
   >
   >Después de crear el paquete, su estado se establece en **Draft**. El estado **Activo** no está disponible hasta que haya probado el paquete primero.
1. (Recomendado) Haga clic en **Instalar** y elija uno de los entornos de prueba disponibles para implementarlo allí y probar la configuración.

   >[!TIP]
   >
   >El entorno Producción no está disponible como una de las opciones cuando el estado se establece en **Prueba**.

1. Después de instalarlo en un entorno de prueba, vuelve a hacer clic en **Editar**, establece el **Estado** en **Activo** y, a continuación, haz clic en **Guardar y cerrar**.

   >[!TIP]
   >
   >La instalación del paquete en un entorno de prueba es similar a la instalación en producción, tal como se describe en la siguiente sección.

   Continúe con la siguiente sección para instalar el paquete en el entorno de destino.


### Instalación del paquete en el entorno de destino

1. En la página del paquete, después de verificarla, haga clic en **Instalar**.
1. En la lista **Entorno de destino**, seleccione el entorno en el que implementar (por ejemplo, su entorno de producción) y haga clic en **Continuar**. El destino predeterminado es el entorno actual.
1. En la página **Información del paquete**, confirme el entorno de origen y el entorno en el que está implementando.
1. En la sección **Asignación de objetos**, expanda cada agrupación de objetos, como **Grupo** y **Espacio de trabajo de Planning**, para revisar los objetos.
1. Para cada objeto, revise las columnas **Conflicto** y **Estado** y, a continuación, elija una **acción de implementación** de la lista. Elija entre las siguientes opciones:

   * **Crear nuevo**: Agrega el objeto al destino. Utilícelo cuando no se detecte ninguna colisión.
   * **Usar existente**: asigna el objeto a uno que ya existe en el destino, como un grupo con el mismo nombre.
   * **Crear con nuevo nombre**: Agrega el objeto con un nombre especificado.
   * **Sobrescribir**: reemplaza el objeto existente en el destino por el del paquete.
1. (Opcional) Para cambiar varios objetos a la vez, seleccione sus casillas de verificación, elija una acción en la lista Acción de implementación en la parte superior del grupo y haga clic en Aplicar a los objetos seleccionados. Utilice los filtros encima de la lista, como Mostrar solo errores, para centrarse en objetos específicos.
1. Resuelva los indicadores de error. Si selecciona **Usar** existente para un objeto, también debe seleccionar el objeto al que se asigna.  De lo contrario, el estado muestra un error y **Implementar** permanece no disponible.
1. Haga clic en **Implementar** y luego en **Implementar** para confirmar.

   Workfront muestra una página de instalación con el mensaje **Este paquete se está instalando**. Esto puede tardar unos minutos.

   Cuando finaliza la instalación, la página muestra un mensaje de éxito, el entorno donde se instaló el paquete y una lista de los objetos instalados, con un estado para cada uno, como **Usado existente** o **Instalado (Crear nuevo)**.
1. (Opcional) Haga clic en **Deshacer la instalación**, si es necesario, para revertir la instalación y quitar la configuración del entorno de destino.

   Continúe comprobando los resultados de la instalación.

### Verificar los resultados

1. Vaya al entorno de destino > **Menú principal** > **Planificación** y busque el área de trabajo importada.
1. Abra los tipos de registro y las vistas para confirmar que los campos y el diseño coinciden con el origen. Los registros no se incluyen, por lo que las tablas están vacías.


