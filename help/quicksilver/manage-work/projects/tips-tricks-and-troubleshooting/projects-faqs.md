---
title: Preguntas frecuentes sobre proyectos
description: Preguntas frecuentes sobre proyectos
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Preguntas frecuentes sobre proyectos

A continuación se presentan las preguntas más frecuentes sobre los proyectos.

## ¿Por qué falta Insertar tarea arriba/abajo cuando hago clic con el botón derecho en una tarea de la lista de tareas?

### Respuesta

Para utilizar las opciones de inserción, la lista de tareas debe ordenarse por número. Para ordenar la columna por número, haga clic en **#** en el encabezado de columna a la izquierda de **Nombre de la tarea** para que la tarea pase por número.

## ¿Cuál es la fecha de finalización real?

### Respuesta

La fecha de finalización real representa la fecha y la hora en que se completa el trabajo. Para obtener más información, consulte [Descripción general de la fecha de finalización real del proyecto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## ¿Por qué falta el botón sangría/sangría?

### Respuesta

Para utilizar el botón sangría/ sangría, asegúrese de que las tareas se ordenan por número de tarea y no se aplican agrupamientos.

## ¿Por qué no puedo cambiar el estado del proyecto a Completado?

Recibo el siguiente mensaje de error cuando intento marcar la finalización de mi proyecto:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Respuesta

No puede cambiar el estado de un proyecto para completarlo si tiene cualquiera de las siguientes opciones en el proyecto:

* Tareas o problemas incompletos
* Tarea o problemas en estado de aprobación pendiente

## ¿Por qué no puedo cambiar el estado del proyecto de Completado a Actual?

### Respuesta

Si el proyecto tiene el modo de finalización establecido en automático, una vez que se hayan completado todas las tareas y problemas, el estado del proyecto pasa automáticamente a estar completado y no se puede modificar a ningún otro estado. El modo de finalización del proyecto debe configurarse como Manual para poder convertir un proyecto completo en Actual. Para obtener más información, consulte [El estado del proyecto no cambiará de Completo a Actual](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## ¿Por qué no puedo agregar un proyecto a un Portfolio, aunque tengo los permisos correctos para hacerlo?

Aunque tengo los permisos correctos, falta el botón Agregar proyectos en la pestaña Proyectos del Portfolio.

### Respuesta

Esto se debe a que el estado del Portfolio es inactivo. Para cambiar el estado del Portfolio:

1. Haga clic en **Detalles del Portfolio > Información general**.
1. Cambie el **Estado** a **Activo.**

1. Haga clic en **Guardar**.\
   La variable **Agregar proyectos** ahora debe ser visible en la variable **Proyectos** pestaña .

## ¿Qué acceso recibe un Administrador de recursos cuando se agrega a un proyecto?

### Respuesta

Los administradores de recursos reciben automáticamente el acceso Administrar a los proyectos. Al eliminar el usuario de la función Administrador de recursos , no se elimina su acceso de uso compartido Administrar .

## ¿Por qué cambia el estado del proyecto cuando añado un grupo?

### Respuesta

Los estados del proyecto cambian debido a los estados predeterminados del Grupo. Cuando agrega un grupo a un proyecto, cambia la lista de estados a los estados predeterminados establecidos para el grupo.

Para obtener más información, consulte el artículo [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## ¿Qué es el estado del presupuesto?

### Respuesta

El estado del presupuesto mostrará si el proyecto se ha agregado o no al planificador de capacidades y si se ha completado el cálculo del presupuesto.

Los siguientes son estados presupuestarios:

* No incluido : el proyecto no se agrega al planificador de capacidades.
* Incluido pero no calculado : el proyecto se agrega al Planificador de capacidad, pero se excluye del cálculo del presupuesto.
* Incluido y calculado: el proyecto se añade al planificador de capacidad y se incluye en el cálculo del presupuesto.

## ¿Por qué no puedo compartir un proyecto para el que soy el propietario y en el que tengo permisos de gestión con un equipo? Simplemente no puedo encontrar el equipo en el cuadro de diálogo de uso compartido del proyecto.

### Respuesta

El administrador de Adobe Workfront le restringió a ver solo las empresas, los grupos y los equipos a los que pertenece en su nivel de acceso de . El equipo al que está buscando no es uno de los equipos a los que pertenece.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Para obtener información sobre cómo permitir que un usuario vea todos los equipos del sistema, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
