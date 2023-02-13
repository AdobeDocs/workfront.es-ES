---
title: Registros de auditoría
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede realizar un seguimiento de los cambios de usuario activados en el sistema durante los últimos 90 días mediante registros de auditoría.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# Registros de auditoría

Como administrador de Adobe Workfront, puede realizar un seguimiento de los cambios de usuario activados en el sistema durante los últimos 90 días mediante los registros de auditoría que se describen a continuación.

Para obtener instrucciones sobre cómo ver y filtrar lo que desea ver en estos registros de auditoría, consulte [Ver y exportar registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Información que puede encontrar en un registro de auditoría

Los campos siguientes se registran en cada entrada de registro de auditoría:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fecha y hora</td> 
   <td>Cuando se produjo la acción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Tipo del registro de auditoría, como Nivel de acceso o Formulario personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nombre de usuario</td> 
   <td> <p>Nombre del usuario que realizó la acción.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acción</td> 
   <td> Acción realizada por el usuario, como Cambiar, Crear y Eliminar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objeto</td> 
   <td> Nombre del objeto afectado como resultado de la acción. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Detalles</td> 
   <td>Detalles adicionales sobre la acción. Pase el ratón sobre el texto para leer el mensaje completo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dirección IP</td> 
   <td> <p>Dirección IP del usuario que realizó la acción en el momento de la acción.</p> <p>La dirección IP no está disponible para algunas acciones del sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de registro de auditoría y las acciones que los déclencheur

* [Nivel de acceso](#access-level)
* [Compañía](#company)
* [Condición](#condition)
* [Campo personalizado](#custom-field)
* [Formularios personalizados](#custom-forms)
* [Sección personalizada](#custom-section)
* [tarifa de cambio](#exchange-rate)
* [Grupo](#group)
* [Roles](#job-roles)
* [Intento de inicio de sesión](#login-attempt)
* [Prioridad](#priority)
* [Preferencias de proyecto](#project-preferences)
* [Gravedad](#severity)
* [Estado](#status)
* [Preferencias de tareas y problemas](#tasks-issues-preferences)
* [Usuario](#user)

### Nivel de acceso {#access-level}

El sistema genera una entrada de registro de nivel de acceso cuando un usuario realiza una de las siguientes acciones:

* Crea un nivel de acceso
* Elimina un nivel de acceso
* Cambia un nivel de acceso:

   * Modifica el tipo de licencia
   * Cambia los permisos de Proyectos, Tareas, Problemas, Portfolio, Programas, Informes, Documentos, Usuarios o Plantillas

      >[!NOTE]
      >
      >El sistema no registra ningún cambio en los permisos de Datos financieros ni dentro de los siguientes tipos de acceso: Ver y editar.
      >
      >Por ejemplo, si un usuario cambia el tipo de acceso Planificador de Vista a Editar, el sistema no mostrará la información contenida en el menú desplegable Ajustar la configuración .

### Compañía {#company}

El sistema genera una entrada de registro de auditoría de la empresa cuando un usuario realiza una de las siguientes acciones:

* Crea una empresa
* Cambia una empresa:

   * Cambia el nombre
   * Agrega o elimina miembros
   * Agrega, edita o elimina el valor en su campo Grupo
   * Agrega o edita una tasa de facturación de la empresa para una función de trabajo
   * Elimina una tasa de facturación de la empresa para una función de trabajo
   * Lo establece como la empresa principal para la organización
   * Adjunta o quita un formulario personalizado

* Elimina una empresa

Para obtener más información sobre los estados, consulte [Resumen de los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condición {#condition}

El sistema genera una entrada de registro de auditoría de condiciones cuando un usuario realiza una de las siguientes acciones:

* Crea una condición
* Cambia una condición:

   * Cambia el nombre
   * Cambia el color
   * Lo establece como predeterminado
   * Cambia o elimina la descripción de la condición
   * Oculta o muestra la condición

* Elimina una condición

Para obtener más información sobre la configuración de funciones de trabajo, consulte [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizado {#custom-field}

El sistema genera una entrada de registro de auditoría de campos personalizados cuando un usuario realiza una de las siguientes acciones:

* Crea un campo personalizado
* Cambia un campo personalizado:

   * Cambia el nombre, la etiqueta, las instrucciones o el formato
   * Cambia el tipo de visualización

      Esto solo está disponible si el campo es de uno de los siguientes tipos: línea única, párrafo, lista desplegable, casilla de verificación, botón de radio

   * Cambia el tamaño del campo

      Esto solo está disponible si el campo es de uno de los siguientes tipos: línea única, párrafo, texto con formato

   * Agrega, elimina u oculta una opción de campo
   * Edita una etiqueta o un valor de opción de campo
   * Configura la opción de campo que se va a seleccionar o que no se va a seleccionar de forma predeterminada
   * Configura un campo desplegable para permitir varias selecciones o una sola selección
   * Configura un campo de fecha para mostrar o no la hora del día
   * Edita el hipervínculo o cambia el valor de un campo de texto descriptivo

* Elimina un campo personalizado
* Comparte un campo personalizado

### Formularios personalizados {#custom-forms}

El sistema genera una entrada de registro de auditoría de Forms personalizada cuando un usuario realiza una de las siguientes acciones:

* Crea un formulario personalizado
* Cambia un formulario personalizado:

   * Cambia el nombre o la descripción
   * Habilita o deshabilita está activo
   * Agrega o quita un campo o una sección
   * Para una sección personalizada, cambia una configuración en Configuración adicional
   * Cambia un campo a obligatorio o no obligatorio
   * Cambia un cálculo en un campo personalizado
   * Oculta o muestra la fórmula asociada a un campo calculado en el texto del pase de instrucciones
   * Habilita o deshabilita Actualizar cálculos anteriores
   * Agrega o cambia la lógica de omisión o la lógica de visualización

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Elimina un formulario personalizado
* Comparte un formulario personalizado

### Sección personalizada {#custom-section}

El sistema genera una entrada de registro de auditoría de sección personalizada cuando un usuario realiza una de las siguientes acciones en un formulario personalizado:

* Crea una sección personalizada
* Cambia el nombre o la descripción de una sección personalizada
* Elimina una sección personalizada

Para obtener información sobre las secciones personalizadas en los formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### tarifa de cambio {#exchange-rate}

El sistema genera una entrada de registro de auditoría de tipo de cambio cuando un usuario realiza una de las siguientes acciones:

* Crea un tipo de cambio
* Cambia un tipo de cambio:

   * Agrega una moneda
   * Cambia la tasa de la moneda
   * Establece la moneda como moneda base (predeterminada) para todos los proyectos e informes del sistema

* Elimina un tipo de cambio

Para obtener más información sobre la configuración de las tasas de cambio, consulte [Configurar tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Grupo {#group}

El sistema genera una entrada de registro de auditoría de grupo cuando un usuario realiza una de las siguientes acciones:

* Crea un grupo
* Elimina un grupo
* Cambia un grupo:

   * Agrega o elimina usuarios
   * Agrega o elimina subgrupos

### Roles {#job-roles}

El sistema genera una entrada de registro de auditoría de funciones de trabajo cuando un usuario realiza una de las siguientes acciones:

* Crea una función de trabajo
* Cambia una función de trabajo:

   * Cambia el nombre
   * Agrega, cambia o elimina la descripción
   * Agrega, cambia o elimina el coste por hora (costo/hora)
   * Agrega, cambia o elimina la tasa de facturación (Facturación/Hr.)

* Elimina una función de trabajo

Para obtener más información sobre la configuración de funciones de trabajo, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Intento de inicio de sesión {#login-attempt}

El sistema genera una entrada de registro de auditoría de intento de inicio de sesión cuando un usuario realiza una de las siguientes acciones:

* Inicia sesión, cierra sesión o falla en un intento de inicio de sesión en Workfront (en un explorador y en la aplicación móvil)
* Inicie sesión, cierre la sesión o falle un intento de inicio de sesión en cualquier integración de Workfront (como Workfront para Slack y Workfront para Salesforce)
* Inicia sesión o cierra sesión en la API de Workfront

Los registros de intentos de inicio de sesión no registran cuando un administrador de Workfront utiliza la función Iniciar sesión como .

>[!NOTE]
>
>Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Si necesita más información, consulte con su administrador de red o TI.

### Prioridad {#priority}

El sistema genera una entrada de registro de auditoría de prioridad cuando un usuario realiza una de las siguientes acciones:

* Crea una prioridad
* Cambia una prioridad:

   * Cambia el nombre
   * Cambia el color
   * Lo establece como predeterminado
   * Agrega, cambia o elimina la descripción de la prioridad
   * Oculta o muestra la prioridad

* Elimina una prioridad

Para obtener más información sobre la configuración de prioridades, consulte [Crear y personalizar prioridades](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Preferencias de proyecto {#project-preferences}

El sistema genera una entrada de registro de auditoría Preferencias del proyecto cuando un usuario realiza una de las siguientes acciones:

* Crea un trimestre personalizado
* Cambia las preferencias de un proyecto:

   * Bloquea o desbloquea
   * Cambia una de sus configuraciones
   * La activa, desactiva o edita
   * Edita un cálculo de línea de tiempo

* Elimina un trimestre personalizado

Para obtener más información sobre las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravedad {#severity}

El sistema genera una entrada de registro de auditoría de gravedad cuando un usuario realiza una de las siguientes acciones:

* Crea una gravedad de problema
* Cambia la gravedad del problema:

   * Cambia el nombre
   * Cambia el color
   * Lo establece como predeterminado
   * Cambia o elimina la descripción de la gravedad
   * Oculta o muestra la gravedad

* Elimina una gravedad del problema

Para obtener más información sobre la configuración de funciones de trabajo, consulte [Crear o personalizar grupos de problemas](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Estado {#status}

El sistema genera una entrada de registro de auditoría de estado cuando un usuario realiza una de las siguientes acciones:

* Crea un estado en el nivel de sistema o grupo
* Cambia un estado a nivel de sistema o grupo:

   * Cambia el nombre
   * Lo convierte en un estado predeterminado
   * Bloquea o desbloquea
   * Oculta o desoculta
   * Cambia el color o la descripción

* Elimina un estado en el nivel de sistema o grupo

Para obtener más información sobre los estados, consulte [Resumen de los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferencias de tareas y problemas {#tasks-issues-preferences}

El sistema genera una entrada de registro de auditoría de Preferencias de tareas y problemas cuando un usuario cambia una preferencia de Tareas y problemas de una de las siguientes maneras:

* Bloquea o desbloquea una preferencia
* Cambia la configuración de una preferencia
* Cambia una configuración de acceso para tareas, problemas o solicitudes

Para obtener más información sobre las preferencias de tareas y problemas, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Usuario {#user}

El sistema genera una entrada de registro de auditoría de usuario cuando un usuario realiza una de las siguientes acciones:

* Crea un usuario

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Si necesita más información, consulte con su administrador de red o TI.

* Elimina un usuario
* Cambia el nivel de acceso, la empresa, el equipo o el grupo de un usuario
* Activa un usuario
* Desactiva un usuario
