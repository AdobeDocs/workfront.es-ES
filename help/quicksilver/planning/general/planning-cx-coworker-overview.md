---
title: Información general sobre Adobe Workfront Planning CX Coworker
description: Puede utilizar CX Coworker en Workfront Planning para realizar acciones similares a los registros y otros objetos de Planning que normalmente realizaría en la interfaz. Los comandos del usuario y la ejecución por parte de la IA de esos comandos funcionan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 17%
---

# Información general sobre Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

CX Coworker es una interfaz conversacional en la que se describe un objetivo en lenguaje sencillo y, a continuación, se planifica, ejecuta y valida el trabajo en los sistemas de Workfront Planning y otros sistemas de Adobe conectados antes de devolverlo para su aprobación.

El CX Coworker conserva todo lo que hace el asistente de IA hoy en día, a la vez que agrega funcionalidades integrales más potentes tanto en una nueva experiencia de pantalla completa como en el carril derecho de Workfront.

Funciona dentro de los controles de acceso de nivel de producto existentes en su organización, por lo que los usuarios solo pueden realizar acciones para las que ya están permitidos en Workfront, con acceso de solo lectura de forma predeterminada y acceso de escritura controlado por los administradores de Workfront.

>[!IMPORTANT]
>
>CX Coworker no está disponible actualmente para organizaciones de atención médica, finanzas u otros sectores con datos confidenciales. Estas organizaciones disponen de un asistente de IA.
>
>Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


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
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p>
O
<p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td>  
   <p>El administrador debe hacer lo siguiente para permitir el acceso a CX Coworker en Planning:</p>
   <ul>
   <li><p>Agregue un tipo de licencia de flujo de trabajo y de Planning a su nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning</p></li>
   <li><p>Anule la selección de Deshabilitar el panel CX Coworker en la configuración de Workfront de su nivel de acceso. Está seleccionada de forma predeterminada.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Configuración del sistema</p></td> 
   <td>   <p>El administrador de Workfront debe seleccionar las herramientas MCP de solo lectura y de solo escritura en el área Preferencias del sistema de Configuración. Las herramientas MCP de solo lectura están seleccionadas de forma predeterminada.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para CX Coworker

* CX Coworker debe estar habilitado para su organización antes de que esté disponible para los usuarios de su empresa.

  Para obtener más información, consulte [Información general de CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Una vez que Workfront ha habilitado el agente para la instancia de Workfront, estará disponible para el administrador principal de Workfront y podrá habilitarlo para su organización. Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* El administrador de Workfront también debe habilitar CX Coworker en su nivel de acceso. Para obtener más información, vea [Crear y modificar niveles de acceso](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* CX Coworker trabaja con información y objetos que se encuentran en Workfront o Workfront Planning y a los que tiene permiso para acceder. En el carril derecho de Planning, el panel Compañero de trabajo funciona en el contexto del espacio de trabajo, el tipo de registro o la página de registro que ha abierto.

* Las acciones que realiza CX Coworker en el área de Planning se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront. Para obtener más información, consulte los siguientes artículos:

  * [Información general sobre los permisos de uso compartido en Planificación de Workfront de Adobe](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Información general sobre el tipo de licencia al usar Planificación de Workfront de Adobe](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por CX Coworker en nombre del usuario se rastrean en el panel del historial del registro.

* Las acciones realizadas por CX Coworker son permanentes y podrían ser irreversibles. Por ejemplo, no se puede deshacer la eliminación de un campo. Revise todas las acciones propuestas por CX Coworker antes de aceptarlas.

* Al crear, actualizar o eliminar un objeto a través de CX Coworker, CX Coworker muestra las acciones deseadas y solicita confirmación. A continuación, puede confirmar o cancelar las acciones.

## Funcionalidad disponible actualmente para CX Coworker

Actualmente, CX Coworker está disponible en el área de Planning de Workfront y utiliza un conjunto de habilidades para acceder y manipular la información de los objetos de Planning. Para obtener más información, consulte [Aptitudes de CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Puede utilizar CX Coworker para realizar las siguientes acciones:

* Búsqueda de registros. Puede buscar por la información contenida en cualquier campo de registro.
* Crear registros. Una vez creado el registro, se muestra un ID con un vínculo al nuevo registro. Puede especificar los campos que desea actualizar durante el proceso de creación, como fechas o descripciones.
* Cree registros basados en un documento que haya cargado. Workfront admite los siguientes formatos de documento para CX Coworker:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT y la mayoría de los formatos de imagen
* Actualizar los campos de los registros que ve en la pantalla
* Eliminar, duplicar o restaurar registros
* Vincular registros a otros registros
* Ver el historial de cambios de un registro


## Busque CX Coworker en Workfront Planning

Puede localizar CX Coworker en las siguientes áreas de Workfront Planning:

* La barra de navegación principal, en la esquina superior derecha de la pantalla.
* Dentro del área de detalles de un registro cuando lo abre en una nueva pestaña.

## Acceda a CX Coworker en el área de planificación


1. Inicie sesión en Workfront, luego haga clic en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **Planificación**.

   Se abre el área de Planning.

   Busque el **icono de IA** ![icono de IA](assets/ai-icon.png) en la esquina superior derecha de la página o continúe con los pasos a continuación.

1. Haga clic en una **tarjeta del espacio de trabajo**.

1. Haga clic en **tarjeta de tipo de registro**.

1. Haga clic en un **registro** para abrir la página **Detalles** del registro y, a continuación, haga clic en abrir en

1. Haga clic en el **icono de CX Coworker** en la esquina superior derecha de la pantalla.

1. En el espacio proporcionado, empiece a escribir comandos para CX Coworker y, a continuación, haga clic en Entrar cuando haya terminado.

   ![Panel de CX Coworker con el cuadro de comandos vacío](assets/cx-coworker-right-rail.png)

   Por ejemplo, puede escribir una de las siguientes opciones:

   * Cree un nuevo registro de campaña llamado Rebajas de verano de 2026
   * Actualice el campo de presupuesto en el registro Campaña de verano a 75 000 $
   * Elimine el registro de campaña denominado Promoción antigua
   * Restaurar la campaña que eliminé accidentalmente

   >[!TIP]
   >
   >Asegúrese de que el administrador de Workfront haya habilitado las herramientas MCP de solo escritura en las preferencias del sistema antes de solicitar a CX Coworker que realice acciones de edición en los objetos.

   Se muestra un indicador visual mientras el CX Coworker procesa los comandos, lo que establece las expectativas del tiempo de respuesta.

   Después de recibir una respuesta correcta, siga los vínculos proporcionados u observe los cambios que aparecen a la izquierda.


1. (Opcional) Haga clic en el icono **Expandir pantalla completa** ![Expandir icono de pantalla completa](assets/expand-full-screen-icon.png) para abrir el cuadro de diálogo Colaborador en una pestaña completa del explorador.


