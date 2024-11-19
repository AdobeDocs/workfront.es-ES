---
title: Información general del asistente de IA
content-type: reference
description: Información general del asistente de IA
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 64ad86e29bf18969f82dbdb54b98ca884d2ec26a
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---

# Información general del asistente de IA

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Está disponible en el entorno de vista previa para todos los clientes y en el entorno de producción para los clientes que han habilitado versiones mensuales. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

El asistente de IA de Workfront le ayuda a realizar su trabajo al ofrecerle información y sugerencias en la aplicación en una conversación en lenguaje natural. El asistente de IA puede ofrecerle una experiencia de trabajo más fluida al

* Resumir elementos o documentos de trabajo
* Buscar instrucciones o material de referencia para los procesos de trabajo
* Generar o comprobar fórmulas para campos calculados

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: no disponible</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: no disponible</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Requisitos previos para el asistente de IA

## Requisitos previos para el asistente de IA

Para habilitar el Asistente de IA para su organización, se deben aplicar **todas** las siguientes opciones:

* Su organización debe haber migrado a Adobe IMS (sistema Identity Management)
* La experiencia unificada de Adobe debe estar habilitada
* Su organización debe tener un plan Select, Prime o Ultimate Workfront
* El Adobe debe tener un acuerdo de IA general de Adobe firmado en el archivo

  Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de generación de IA de Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en este artículo.

## Consideraciones sobre el asistente de IA

* El asistente de IA distingue entre contextos y la página que ha abierto. Por ejemplo, si se introduce &quot;Resumir este proyecto&quot; en el asistente de IA de una página de proyecto, se devuelve un resumen de ese proyecto específico.
* El administrador de Workfront debe habilitar el Asistente de IA para los usuarios de su organización. El asistente de IA se habilita mediante niveles de acceso.

  Para obtener más información, consulte [Habilitar o deshabilitar el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* El Asistente de inteligencia artificial aplicada a la planificación de Workfront tiene características diferentes a las del Asistente de IA de Workfront.

  Para obtener más información sobre el Asistente de IA en Workfront Planning, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Funcionalidad disponible en el asistente de IA

El asistente de IA ofrece actualmente las siguientes funciones:

* Resumir proyectos, tareas, problemas o documentos.

  Para obtener más información, vea [Resumir con el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Proporcionar instrucciones o información de referencia extraída de la documentación de Workfront en Adobe Experience League.

  Para obtener más información, consulte [Obtener ayuda del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

<div class="preview">

* Localizar elementos específicos en Workfront.

  Para obtener más información, vea [Usar el Asistente para IA para trabajar con proyectos, tareas y problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

</div>

* Generar o refinar fórmulas para campos personalizados calculados.

  >[!NOTE]
  >
  >Esta funcionalidad solo está disponible para organizaciones con planes Prime o Ultimate Workfront.

  Para obtener más información, vea [Generar o revisar fórmulas de campos calculados con el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Tipos de objetos disponibles para el asistente de IA

El asistente de IA puede consultar los datos asociados con los siguientes tipos de objetos si el usuario tiene los permisos válidos en Workfront:

* Portafolios
* Programas
* Proyectos
* Tareas
* Problemas
* Formularios personalizados
* Usuarios
* Registros de Workfront Planning


## Acceder al asistente de IA

1. En la parte superior de cualquier página de Workfront, haga clic en el icono Asistente de IA ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Escriba su pregunta o mensaje en el panel situado a la derecha de la pantalla.

   Si no puede escribir en este panel, su organización no tiene un acuerdo de IA general de Adobe firmado en el archivo.

1. Si el asistente de IA no proporciona la respuesta que necesita, perfeccione el mensaje e inténtelo de nuevo.

## Firma del acuerdo de Adobe Gen AI

Si su organización no tiene un acuerdo de IA de generación de Adobe firmado, el Asistente de IA no se puede habilitar para su organización.

Si un usuario intenta utilizar el asistente de IA cuando no se ha firmado el acuerdo de IA de generación de Adobe, verá un mensaje:

* Usuarios: se informa a los usuarios de que el Asistente de IA no se ha habilitado para su organización y de que pueden ponerse en contacto con el administrador de Workfront para solicitarlo para su organización.
* Administradores: se informa a los administradores de que no hay un acuerdo de IA general de Adobe firmado y pueden solicitar que se envíe una copia del acuerdo para su firma.

Para solicitar el acuerdo de Adobe Gen AI:

1. Como administrador de Workfront, haga clic en el icono Asistente de IA ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Empiece a escribir en el panel Ayudante de IA.
1. Cuando aparezca el mensaje del acuerdo de Adobe Gen AI, haga clic en **Revisar acuerdo**.
1. Introduzca el nombre y la dirección de correo electrónico de la persona de su organización que firmará el acuerdo de generación de IA de Adobe.

   El acuerdo se enviará a esta persona para que lo firme. Una vez firmado y devuelto, el Ayudante de IA se habilita para su organización.
