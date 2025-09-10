---
title: Información general sobre tipos de registros centralizados
description: Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Resumen de tipos de registros centralizados

Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning.

## Descripción general de los tipos de registros centralizados

Al implementar Workfront Planning para una organización de varios equipos con flujos de trabajo comunes, es posible que necesite definir una estructura y metadatos coherentes para los tipos de registro clave (como Campañas o Entregables) que se pueden agregar a los espacios de trabajo de cada equipo para capturar y administrar su trabajo.

Además, es posible que necesite el trabajo de cada equipo para llegar a un nivel central.

En un flujo de trabajo de este tipo, puede asegurarse de que los equipos capturan su trabajo de forma coherente y, al mismo tiempo, desbloquean la visibilidad entre equipos, sin necesidad de agregar todo a un espacio de trabajo o a todos los miembros de la organización en cada uno de ellos. Puede utilizar tipos de registros centralizados para conseguirlo.

Para utilizar tipos de registros centralizados, haga lo siguiente:

1. Configure un tipo de registro para que esté centralizado en un espacio de trabajo específico.

   Un administrador de espacio de trabajo puede seleccionar usuarios con una licencia estándar, equipos, grupos, funciones o empresas para agregar un tipo de registro elegido a un espacio de trabajo que administren.

   El tipo de registro original existirá en su espacio de trabajo original, pero será visible desde todos los demás espacios de trabajo.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Agregue un tipo de registro existente de uno existente que se haya configurado como centralizado al espacio de trabajo de un equipo.

   El tipo de registro existe en los siguientes espacios de trabajo:

   * Su espacio de trabajo original, donde se designó como tipo de registro centralizado.
   * El espacio de trabajo del equipo.

   Para obtener más información, vea [Agregar tipos de registros existentes](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   Las secciones siguientes describen consideraciones sobre los tipos de registros centralizados en sus espacios de trabajo originales o después de agregarlos a los espacios de trabajo de un equipo.

## Consideraciones sobre los tipos de registros centralizados en su espacio de trabajo original

El tipo de registro configurado para ser centralizado tiene las siguientes propiedades:

* Toda su información solo se puede editar en el espacio de trabajo original.

* Puede realizar las siguientes acciones en el tipo de registro centralizado desde el espacio de trabajo original de un tipo de registro centralizado:

   * Edítela

     La edición de un tipo de registro centralizado incluye la edición de su aspecto, las funciones entre espacios de trabajo y todos los campos creados en el espacio de trabajo original.
   * Creación de formularios de solicitud
   * Administrar formularios de solicitud

* Sólo puede eliminar un tipo de registro centralizado si no se ha agregado a un área de trabajo de equipo. Una vez añadido al espacio de trabajo de un equipo, al intentar eliminarlo del espacio de trabajo original se genera un error.

  Esto se hace para que el tipo de registro centralizado pueda permanecer en los espacios de trabajo donde ya se ha agregado.
* Los registros que agregue a un tipo de registro centralizado sólo son visibles para los usuarios que tienen permisos de Vista en su espacio de trabajo original.
* Los registros que se agregan del espacio de trabajo del equipo se acumulan y se muestran en el espacio de trabajo original. Todos los miembros del espacio de trabajo original obtienen permisos de visualización.

* Los tipos de registro conectados de un tipo de registro centralizado estarán disponibles para la conexión desde los espacios de trabajo en los que se agregue este tipo de registro.

* Los campos creados para un tipo de registro centralizado desde el espacio de trabajo original son visibles desde todos los espacios de trabajo en los que se ha añadido el tipo de registro.

## Consideraciones sobre los tipos de registros centralizados después de agregarlos al espacio de trabajo de un equipo

* Los colaboradores de Team Workspace obtienen permiso de contribución para el tipo de registro centralizado del área de trabajo de equipo. Pueden agregar y administrar registros en él.

* Los visualizadores de Team Workspace obtienen permiso de visualización para el tipo de registro centralizado en Team Workspace. No pueden agregarlo y administrarlo registros en.

* Los administradores de área de trabajo de equipo pueden realizar las siguientes acciones en el tipo de registro agregado desde un tipo de registro centralizado en el área de trabajo de un equipo:

   * Añadir campos nuevos

     Los campos agregados a un registro centralizado desde un área de trabajo de equipo solo son visibles desde el área de trabajo del equipo.
   * Compartirlo
   * Elimínelo.

     Al eliminar el tipo de registro del espacio de trabajo de un equipo, solo se elimina del espacio de trabajo del equipo. También se eliminan los registros que se le hayan agregado desde el espacio de trabajo del equipo. Esto no elimina el tipo de registro de su espacio de trabajo original ni de ningún otro espacio de trabajo de equipo en el que se haya agregado.

     Esto se hace para que sea posible mantener el tipo de registro centralizado ya agregado en los espacios de trabajo que ya lo están utilizando.

* No puede realizar las siguientes acciones en el tipo de registro agregado desde un tipo de registro centralizado en el espacio de trabajo de un equipo:

   * Edítela

     No se puede editar su aspecto, sus funciones entre espacios de trabajo ni los campos añadidos desde el espacio de trabajo original.
   * Creación de formularios de solicitud
   * Administrar formularios de solicitud

* Los registros añadidos en los espacios de trabajo de un equipo son visibles desde los siguientes espacios de trabajo, si tiene permisos de Vista o superiores en estos espacios de trabajo:

   * Espacio de trabajo del equipo en el que se agregan.
   * Espacio de trabajo original del tipo de registro centralizado.
   * Todos los demás espacios de trabajo en los que se haya añadido el espacio de trabajo centralizado.

* Los siguientes escenarios existen para registros creados en espacios de trabajo de equipos:

   * Si tiene permisos de Administración en el espacio de trabajo original y no tiene permisos en los espacios de trabajo de los equipos, puede ver los registros agregados desde los espacios de trabajo del equipo en el espacio de trabajo original, pero no puede administrarlos desde el espacio de trabajo original.
   * Si tiene permisos de administración en el espacio de trabajo del equipo, puede administrar los registros en el espacio de trabajo original del tipo de registro centralizado o desde el espacio de trabajo en el que se agregaron.

     Puede ver los registros en espacios de trabajo de equipo adicionales en los que el tipo de registro centralizado se agrega sólo si tiene permisos de visualización en dichos espacios de trabajo.

## Acceso a las conexiones

Los tipos de registro conectados al tipo de registro centralizado en el espacio de trabajo original se vuelven visibles para los espacios de trabajo de equipo en los que se agrega el tipo de registro centralizado.

## Comportamiento de API

Al agregar registros a un tipo de registro centralizado desde un área de trabajo de equipo mediante la API de Workfront Planning, el sistema comprueba si el usuario tiene acceso para crear registros en el área de trabajo original del tipo de registro centralizado.

Se dan los siguientes casos:

* Si el usuario tiene acceso, el registro se crea en el espacio de trabajo original de los tipos de registro centralizados.

* Si el usuario no tiene acceso, recibe el error de que no tiene acceso al espacio de trabajo original del tipo de registro centralizado y debe proporcionar el ID del espacio de trabajo donde tiene acceso para crear registros.