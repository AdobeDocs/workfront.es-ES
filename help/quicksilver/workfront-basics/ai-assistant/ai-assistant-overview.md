---
title: Asistente de IA en Workfront
content-type: reference
description: Obtenga información sobre el Asistente de IA en Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 2619aa432a8c0b12d0d910df8eb05447fa50f387
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 99%

---

# Asistente de IA en Workfront

El asistente de IA de Workfront le ayuda a realizar su trabajo al ofrecerle información y sugerencias en la aplicación mediante una interacción en lenguaje natural. El asistente de IA puede ofrecerle una experiencia de trabajo más fluida al

* Resumir elementos o documentos de trabajo
* Buscar instrucciones o material de referencia para los procesos de trabajo
* Generar o comprobar fórmulas para campos calculados

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Seleccionar o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos para el asistente de IA

Para habilitar el Asistente de IA para su organización, se deben aplicar **todas** las siguientes opciones:

* Su organización debe haber migrado a Adobe IMS (Identity Management System)
* La experiencia unificada de Adobe debe estar habilitada
* Su organización debe tener un plan Select, Primer o Ultimate de Workfront
* Adobe debe tener un acuerdo firmado en el archivo de Adobe Gen AI

  Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en este artículo.

## Consideraciones sobre el asistente de IA

* El asistente de IA distingue entre los contextos de la página que ha abierto. Por ejemplo, si se introduce “Resumir este proyecto” en el asistente de IA de una página de proyecto, este devuelve un resumen de ese proyecto específico.
* El administrador de Workfront debe habilitar el asistente de IA para los usuarios de su organización. El asistente de IA se habilita mediante niveles de acceso.

  Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* El asistente de IA de Workfront Planning tiene funciones diferentes a las del asistente de IA de Workfront.

  Para obtener más información sobre el asistente de IA en Workfront Planning, consulte [Información general del asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* Actualmente, el asistente de IA solo está disponible en inglés.


## Funcionalidad disponible en el asistente de IA

El asistente de IA ofrece actualmente las siguientes funciones:

* Resumir proyectos, tareas, problemas o documentos.

  Para obtener más información, consulte [Resumir mediante el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Proporcionar instrucciones o información de referencia extraída de la documentación de Workfront en Adobe Experience League.

  Para obtener más información, consulte [Obtener ayuda del asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Localizar elementos específicos en Workfront.

  Para obtener más información, consulte [Usar el asistente de IA para trabajar con proyectos, tareas y problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Generar o refinar fórmulas para campos personalizados calculados.

  >[!NOTE]
  >
  >Esta funcionalidad solo está disponible para organizaciones con planes Prime o Ultimate Workfront.

  Para obtener más información, consulte [Generar o revisar fórmulas de campos calculados con el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Resumir actualizaciones, documentos cargados y otros cambios importantes sobre sus proyectos en los siguientes periodos de tiempo: 24 horas, 3 días, 7 días en Prioridades.

Para obtener más información, consulte [Ponerse al día con el trabajo en Prioridades](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Tipos de objetos disponibles en el asistente de IA

El asistente de IA puede consultar los datos asociados con los siguientes tipos de objetos si el usuario tiene los permisos válidos en Workfront:

* Portafolios
* Programas
* Proyectos
* Tareas
* Problemas
* Formularios personalizados
* Usuarios
* Registros de Workfront Planning


## Acceso al Asistente de IA

1. En la parte superior de cualquier página de Workfront, haga clic en el icono ![Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Escriba su pregunta o indicación en el panel situado a la derecha de la pantalla.

   Si no puede escribir en este panel, significa que su organización no tiene registrado ningún acuerdo de IA generativa de Adobe firmado.

1. Si el asistente de IA no proporciona la respuesta que necesita, mejore su indicación e inténtelo de nuevo.

## Firme el acuerdo de IA generativa de Adobe

Si su organización no tiene un acuerdo de IA generativa de Adobe firmado en los archivos, no se podrá habilitar el asistente de IA para su organización.

Si un usuario intenta utilizar el asistente de IA cuando no se ha firmado el acuerdo de IA generativa de Adobe, aparece el siguiente mensaje:

* Usuarios: se les informa a los usuarios de que el asistente de IA no está habilitado para su organización y de que pueden ponerse en contacto con el administrador de Workfront para solicitarlo para su organización.
* Administradores: se les informa a los administradores de que no hay un acuerdo de la IA generativa de Adobe firmado y que pueden solicitar que se les envíe una copia del acuerdo para su firma.

Para solicitar el acuerdo de la IA generativa de Adobe, haga lo siguiente:

1. Como administrador de Workfront, haga clic en el icono ![Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Empiece a escribir en el panel Asistente de IA.
1. Cuando aparezca el mensaje del acuerdo de la IA generativa de Adobe, haga clic en **Revisar acuerdo**.
1. Introduzca el nombre y la dirección de correo electrónico de la persona de su organización que firmará el acuerdo de la IA generativa de Adobe.

   El acuerdo se envía a esta persona para que lo firme. Una vez firmado y devuelto, Adobe revisa el acuerdo y, a continuación, se habilita el asistente de IA para su organización.

   >[!NOTE]
   >
   >Después de firmar y devolver el acuerdo, espere entre 1 y 3 días hábiles para que Adobe revise y active el Asistente de IA.

## Sugerencias para crear indicaciones en el asistente de IA

Utilice las siguientes palabras clave en las indicaciones para proporcionar contexto y localizar la información correcta. Las palabras clave no distinguen entre mayúsculas y minúsculas.

Al escribir la indicación, incluya la frase `using (keyword)`.

| Palabra clave | Efecto |
| --- | --- | 
| `workfront` | Interactúa con Workfront. |
| `planning` | Interactúa con Workfront Planning. |
| `help` | Devuelve información de la documentación de Experience League. |
| `formula` | Comprueba y devuelve fórmulas para utilizarlas en la planificación, configuración o formularios personalizados. |
| `health` | Comprueba el estado del proyecto con el asesor del estado del proyecto. |
| `summarize` | Resume elementos, como al cargar un archivo o resumir un proyecto. |

>[!NOTE]
>
> No todas las palabras clave están disponibles en todas las áreas.
>
>* La palabra clave `formula` solo está disponible en la planificación, en la configuración y en el creador de formularios personalizados.
>* La palabra clave `planning` solo está disponible desde Workfront Planning.





