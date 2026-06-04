---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Información general sobre la delegación de trabajo
description: Cuando planea estar fuera de la oficina por un corto período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/O-G3HS2JWZB36Y-kSloHo6u4--Z3q40fwAgfcEuELi4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 906
ht-degree: 90%

---

# Información general sobre la delegación de trabajo

Cuando planea estar fuera de la oficina por un corto período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.

Por ejemplo, si algunas tareas vencen antes de que regrese pero no tiene tiempo para completarlas antes de que se vaya, puede delegar las tareas a otro usuario para que pueda completarlas a tiempo y no retrasar la finalización del proyecto hasta después de su regreso.

Puede delegar los siguientes objetos en [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tareas que le han asignado
* Problemas que le han asignado
* Aprobaciones de proyectos, tareas o problemas asignadas a usted.

  >[!TIP]
  >
  >   No puede delegar aprobaciones de hojas de horas, documentos o pruebas.


Este artículo contiene información general sobre la delegación de tareas y problemas asignados al usuario.

Para obtener información sobre la delegación de aprobaciones de proyectos, tareas y problemas, consulte [Delegar solicitud de aprobación](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Para obtener información acerca de cómo delegar tareas y problemas, vea [Delegar tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

## Información general sobre la delegación de tareas y problemas

Tenga en cuenta lo siguiente al delegar tareas y problemas:

* Su administrador de [!DNL Workfront] o de grupos debe habilitar las preferencias de delegación en el área de [!UICONTROL Configuración] para poder delegar su trabajo a otras personas.

  Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Solo puede delegar tareas y problemas desde el área de [!UICONTROL Inicio].
* Al delegar trabajo, existen excepciones para los siguientes tipos de licencia:

   * Puede delegar el trabajo a revisores o solicitantes, aunque [!DNL Workfront] no lo recomienda.
   * Los revisores pueden delegar el trabajo a otras personas. No pueden ver elementos de trabajo en su área de [!UICONTROL Inicio]. Solo pueden ver las aprobaciones.
   * Los solicitantes no pueden delegar el trabajo a otras personas. No pueden ver elementos de trabajo en su área de [!UICONTROL Inicio]
* Solo puede delegar las tareas y problemas que le hayan asignado. No puede delegar tareas y problemas asignados a otros usuarios, equipos o funciones.
* Solo puede delegar tareas y problemas que no se hayan completado antes de la fecha de inicio de la delegación.
* Si un elemento de trabajo se completa durante el lapso de tiempo de delegación, el elemento permanece en el área de inicio del delegado y del asignado durante 2 semanas antes de que [!DNL Workfront] lo elimine automáticamente.
* Los usuarios que seleccione como delegados reciben los mismos permisos que los suyos en las tareas y problemas que les delegue. Los permisos deben funcionar dentro de sus niveles de acceso y, a veces, sus niveles de acceso pueden ser inferiores a los suyos.

>[!NOTE]
>
>  En el caso de los elementos asignados una vez iniciada la delegación, el proceso puede demorarse hasta una hora después de que el elemento se haya asignado a [!DNL Workfront] en compartir los elementos recién asignados con la persona delegada.

* Si se le asignan tareas y problemas adicionales durante el tiempo que ha seleccionado para que su trabajo se delegue a otros usuarios, el nuevo trabajo asignado se delegará automáticamente a la misma persona durante el lapso de tiempo que haya seleccionado si las fechas de la tarea o del problema se encuentran dentro de ese lapso de tiempo.
* Varios usuarios pueden seleccionar el mismo usuario como delegado.
* Las tareas y los problemas delegados no se muestran en las herramientas de administración de recursos, como el [!UICONTROL Distribuidor de cargas de trabajo] o el [!UICONTROL Planificador de recursos] para los usuarios delegados.
* Puede ver el trabajo delegado y los nombres delegados en varias áreas de [!DNL Workfront]. Para obtener más información, vea la sección &quot;Buscar trabajo delegado e información de delegados&quot; en el artículo [Delegar tareas y problemas](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Si un usuario solo tiene acceso de visualización de las tareas en su nivel de acceso y usted tiene permisos de administración de las tareas que le delegue, el usuario recibirá permisos de administración de las tareas que usted le delegue. Sin embargo, no podrá realizar las mismas acciones que usted en las tareas delegadas. Debe solicitar al administrador del sistema acceso de edición de las tareas para poder actualizarlas en su ausencia.

* Al detener la delegación no se eliminan los permisos otorgados a los usuarios delegados de las tareas y problemas que les hayan delegado.
* Si un sistema o deshabilita la opción [!UICONTROL Permitir a los usuarios delegar sus tareas y problemas] en el área de [!UICONTROL Configuración], los usuarios delegados actualmente se eliminarán de las tareas y problemas que les hayan delegado anteriormente. Sus permisos para las tareas o problemas no se eliminarán.

## Diferencias y similitudes entre asignaciones y delegaciones

| Acción | Asignaciones | Delegaciones |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un usuario asignado o delegado puede editar o eliminar el elemento de trabajo que le asignen o deleguen | Según permisos y nivel de acceso | Según permisos y nivel de acceso |
| Aparece un usuario asignado o delegado en el encabezado del elemento de trabajo | Sí | Sí |
| Las tareas o problemas asignados o delegados se muestran en el área de Inicio del asignado o delegado | Sí, hasta que finalice el artículo | Sí, solo durante el período de tiempo de la delegación |
| Puede asignar o delegar trabajo a usuarios desde el área de Inicio | Sí | Sí |
| Puede asignar o delegar trabajo a usuarios mediante el Distribuidor de cargas de trabajo | Sí | No |
| Puede asignar o delegar trabajo a usuarios de una lista o desde el encabezado de un elemento de trabajo | Sí | No |
| Cualquier usuario puede asignar o delegar otros usuarios con elementos de trabajo con los que no están asociados | Según permisos y nivel de acceso | No. Solo el asignado puede delegar sus propios elementos. |
| Las horas planificadas, reales o presupuestadas para el trabajo asignado o delegado a un usuario se muestran para ese usuario en las herramientas de administración de recursos | Sí | No |
