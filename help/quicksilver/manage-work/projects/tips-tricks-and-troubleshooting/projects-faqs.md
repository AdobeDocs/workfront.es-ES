---
title: Preguntas frecuentes sobre proyectos
description: Este artículo contiene las preguntas más frecuentes sobre los proyectos de Adobe Workfront.
author: Alina
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 96%

---

# Preguntas frecuentes sobre proyectos

Las siguientes son las preguntas más frecuentes sobre los proyectos.

## ¿Por qué falta Insertar tarea arriba/abajo cuando hago clic con el botón derecho en una tarea de la lista de tareas?

### Respuesta

Para utilizar las opciones de inserción, la lista de tareas debe estar ordenada por número. Para ordenar la columna por número, haga clic en **#** en el encabezado de columna a la izquierda de **Nombre de tarea** para reorganizar la tarea por número.

## ¿Cuál es la fecha de finalización efectiva?

### Respuesta

La Fecha de finalización efectiva representa la fecha y la hora en que se completó el trabajo. Para obtener más información, vea [Información general sobre la fecha de finalización efectiva del proyecto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## ¿Por qué falta el botón de sangría/anulación de sangría?

### Respuesta

Para utilizar el botón de sangría/anulación de sangría, asegúrese de que las tareas estén ordenadas por el número de tarea y de que no se hayan aplicado agrupaciones.

## ¿Por qué no puedo cambiar el estado del proyecto a Completado?

Aparece el siguiente mensaje de error cuando intento marcar mi proyecto como completado:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Respuesta

No puede cambiar el estado de un proyecto a completado si tiene alguno de los siguientes elementos en el proyecto:

* Tareas o problemas incompletos
* Tarea o problemas en estado de aprobación pendiente

## ¿Por qué no puedo cambiar el estado del proyecto de Completado a En curso?

### Respuesta

Si el proyecto tiene el modo de finalización establecido en automático, una vez que se hayan completado todas las tareas y problemas, el estado del proyecto cambiará automáticamente a Completado y no podrá modificarlo a ningún otro estado. El modo de finalización del proyecto debe establecerse en Manual para poder convertir un proyecto completado a En curso. Para obtener más información, consulte [El estado del proyecto no cambiará de Completado a En curso](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## ¿Por qué no puedo añadir un Proyecto a un Portafolio aunque tengo los permisos correctos para hacerlo?

Aunque tengo los permisos correctos, el botón Añadir proyectos no aparece en la ficha Proyectos del Portafolio.

### Respuesta

Esto se debe a que el estado del Portafolio es Inactivo. Para cambiar el estado del Portafolio:

1. Haga clic en **Detalles del Portafolio > Información general**.
1. Cambiar el **Estado** a **Activo.**

1. Haga clic en **Guardar**.\
   El botón **Añadir proyectos** ahora debería estar visible en la ficha **Proyectos**.

## ¿Qué acceso recibe un Administrador de recursos cuando se añade a un proyecto?

### Respuesta

Los administradores de recursos reciben automáticamente acceso de administración a los proyectos. Al quitar el usuario de la función Administrador de recursos, no se quita el acceso de Administrar uso compartido.

## ¿Por qué cambia el estado del proyecto cuando añado un grupo?

### Respuesta

Los estados del proyecto cambian debido a los estados predeterminados del Grupo. Al añadir un grupo a un proyecto, se cambia la lista de estados a los estados predeterminados establecidos para el grupo.

Para obtener más información, consulte el artículo [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## ¿Qué es el estado del presupuesto?

### Respuesta

El estado del presupuesto mostrará si el proyecto está añadido actualmente al Planificador de capacidades y si se completó el cálculo del presupuesto.

Los siguientes son estados de presupuesto:

* No incluido: El proyecto no se añade al planificador de capacidades.
* Incluido, pero no calculado: el proyecto se añade al Planificador de capacidades, pero se excluye del cálculo del presupuesto.
* Incluido y calculado: el proyecto se añade al Planificador de capacidades y se incluye en el cálculo del presupuesto.

## ¿Por qué no puedo compartir un proyecto del que soy propietario y tengo permisos de administración con un equipo? No encuentro el equipo en el cuadro de diálogo Uso compartido del proyecto.

### Respuesta

El administrador de Adobe Workfront ha restringido la visualización a solo Compañías, Grupos y Equipos a los que pertenece su nivel de acceso. El equipo que busca no es uno de los equipos a los que pertenece.

![Ver solamente equipos, grupos y empresas a los que pertenecen](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Para obtener información para permitir que un usuario vea todos los equipos del sistema, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
