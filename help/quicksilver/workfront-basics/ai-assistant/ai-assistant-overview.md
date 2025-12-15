---
title: Asistente de IA en Workfront
content-type: reference
description: Obtenga información sobre el Asistente de IA en Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 44db621643c76ab1f2c1b51d5e81cb0d1f827a58
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 8%

---

# Asistente de IA en Workfront

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
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td><p>Nuevo: cualquiera</p>
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos para el asistente de IA

Para habilitar el Asistente de IA para su organización, se deben aplicar **todas** las siguientes opciones:

* Su organización debe haber migrado a Adobe IMS (sistema Identity Management)
* La experiencia unificada de Adobe debe estar habilitada
* Su organización debe tener un plan Select, Prime o Ultimate Workfront
* Adobe debe tener registrado un acuerdo de Adobe Gen AI

  Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en este artículo.

## Consideraciones sobre el asistente de IA

* El asistente de IA distingue entre contextos y la página que ha abierto. Por ejemplo, si se introduce &quot;Resumir este proyecto&quot; en el asistente de IA de una página de proyecto, se devuelve un resumen de ese proyecto específico.
* El administrador de Workfront debe habilitar el Asistente de IA para los usuarios de su organización. El asistente de IA se habilita mediante niveles de acceso.

  Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* El Asistente de inteligencia artificial aplicada a la planificación de Workfront tiene características diferentes a las del Asistente de IA de Workfront.

  Para obtener más información sobre el Asistente de IA en Workfront Planning, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* Actualmente, el asistente de IA solo está disponible en inglés.


## Funcionalidad disponible en el asistente de IA

El asistente de IA ofrece actualmente las siguientes funciones:

* Resumir proyectos, tareas, problemas o documentos.

  Para obtener más información, vea [Resumir con el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Proporcionar instrucciones o información de referencia extraída de la documentación de Workfront en Adobe Experience League.

  Para obtener más información, consulte [Obtener ayuda del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Localizar elementos específicos en Workfront.

  Para obtener más información, vea [Usar el Asistente para IA para trabajar con proyectos, tareas y problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Generar o refinar fórmulas para campos personalizados calculados.

  >[!NOTE]
  >
  >Esta funcionalidad solo está disponible para organizaciones con planes Prime o Ultimate Workfront.

  Para obtener más información, vea [Generar o revisar fórmulas de campos calculados con el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Resumir actualizaciones, documentos cargados y otros cambios importantes sobre sus proyectos en los siguientes lapsos de tiempo: 24 horas, 3 días, 7 días en Prioridades.

Para obtener más información, vea [Ponerse al día con el trabajo en Prioridades](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


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


## Acceso al Asistente de IA

1. En la parte superior de cualquier página de Workfront, haz clic en el icono ![Ayudante de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Escriba su pregunta o mensaje en el panel situado a la derecha de la pantalla.

   Si no puede escribir en este panel, su organización no tiene registrado ningún acuerdo de IA general de Adobe firmado.

1. Si el asistente de IA no proporciona la respuesta que necesita, perfeccione el mensaje e inténtelo de nuevo.

## Firma del acuerdo de Adobe Gen AI

Si su organización no tiene un acuerdo firmado de IA de Adobe Gen en los archivos, el Asistente de IA no se puede habilitar para su organización.

Si un usuario intenta utilizar el asistente de IA cuando no se ha firmado el acuerdo de IA de Adobe Gen, verá un mensaje:

* Usuarios: se informa a los usuarios de que el Asistente de IA no se ha habilitado para su organización y de que pueden ponerse en contacto con el administrador de Workfront para solicitarlo para su organización.
* Administradores: se informa a los administradores de que no hay un acuerdo firmado de Adobe Gen AI y pueden solicitar que se envíe una copia del acuerdo para su firma.

Para solicitar el acuerdo de Adobe Gen AI:

1. Como administrador de Workfront, haga clic en el icono ![Ayudante de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Empiece a escribir en el panel Ayudante de IA.
1. Cuando aparezca el mensaje del acuerdo de Adobe Gen AI, haga clic en **Revisar acuerdo**.
1. Introduzca el nombre y la dirección de correo electrónico de la persona de su organización que firmará el acuerdo de Adobe Gen AI.

   El acuerdo se enviará a esta persona para que lo firme. Una vez firmado y devuelto, Adobe revisa el acuerdo y, a continuación, el asistente de IA está habilitado para su organización.

   >[!NOTE]
   >
   >Conceda un margen de 1 a 3 días laborables tras la firma y la devolución del acuerdo para que Adobe revise y habilite el asistente de IA.

## Sugerencias para crear mensajes en el Asistente de IA

Utilice las siguientes palabras clave en los indicadores para proporcionar contexto y ayudar a localizar la información correcta. Las palabras clave no distinguen entre mayúsculas y minúsculas.

Al escribir el mensaje, incluya la frase `using (keyword)`.

| Palabra clave | Efecto |
|---|---|
| `workfront` | Interactúa con Workfront. |
| `planning` | Interactúa con Workfront Planning. |
| `help` | Devuelve información de la documentación de Experience League. |
| `formula` | Comprueba y devuelve fórmulas para utilizarlas en Planning, Setup o formularios personalizados. |
| `health` | Comprueba el estado del proyecto con el Asesor de estado del proyecto. |
| `summarize` | Resume elementos, como al cargar un archivo o resumir un proyecto. |

>[!NOTE]
>
> No todas las palabras clave están disponibles en todas las áreas.
>
>* La palabra clave `formula` solo está disponible en Planning, Setup y el creador de formularios personalizados.
>* La palabra clave `planning` solo está disponible en Workfront Planning.





