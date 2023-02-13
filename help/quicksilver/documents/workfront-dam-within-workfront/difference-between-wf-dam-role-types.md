---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Tipos de funciones de licencia de Adobe Workfront frente a tipos de funciones de DAM de Adobe Workfront
description: Los administradores de Adobe Workfront utilizan niveles de acceso para determinar lo que los usuarios pueden hacer en una aplicación.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 2%

---

# Tipos de funciones de licencia de Adobe Workfront frente a tipos de funciones de DAM de Adobe Workfront

Los administradores de Adobe Workfront utilizan niveles de acceso para determinar lo que los usuarios pueden hacer en una aplicación.

* En Workfront, la licencia determina el nivel de acceso de un usuario.
* En Workfront DAM, los tipos de funciones definen el acceso de los usuarios a los recursos en DAM.

Debido a que los tipos de licencia y los tipos de función no son intercambiables, tener un nivel de acceso en una aplicación no implica acceso en la otra aplicación. Por ejemplo, a un usuario con una licencia de trabajo en Workfront no se le asigna automáticamente una función de colaborador dentro de Workfront DAM.

## Tipos de licencia de Workfront

Como administrador de Workfront, puede definir el nivel de acceso que tienen los usuarios asignando tipos de licencia. Cada licencia incluye un conjunto de funciones de acceso predeterminadas que puede modificar antes de asignar la licencia al usuario. 

Las licencias se utilizan para determinar lo que un usuario puede ver y hacer en Workfront. Hay cinco tipos de licencias disponibles en Workfront:

* Plan
* Trabajo
* Revisar
* Solicitud
* Externo

Consulte [Información general sobre las licencias de Adobe Workfront](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) para obtener una descripción de los distintos tipos de licencia en Workfront.

## Tipos de funciones DAM de Workfront

Como administrador de Workfront DAM Workfront, asigna tipos de funciones a los usuarios para definir el acceso que tienen a los recursos. Además, los tipos de funciones especifican las áreas de DAM en las que los usuarios pueden trabajar.

Los tipos de funciones funcionan junto con Grupos al establecer los derechos de acceso de los usuarios. Los grupos controlan el acceso que los usuarios tienen a las carpetas y a los propios recursos. Los tipos de funciones determinan las acciones que los usuarios pueden realizar con los recursos. Todos los usuarios de DAM deben estar asociados con al menos un grupo. Para obtener más información sobre los tipos de funciones y la configuración de acceso, consulte la Ayuda de Workfront DAM.

Hay cuatro tipos de funciones diferentes disponibles en Workfront DAM:

### Brand Portal

Los usuarios con este tipo de rol solo tienen acceso al portal de Brand Connect en DAM. Dentro del portal, los usuarios pueden ver y descargar los recursos a los que tienen permisos.

Los usuarios de Brand Portal pueden colaborar con otros creando y compartiendo lightboxes.

### Usuario normal

Los usuarios con este tipo de función pueden ver y descargar recursos desde Workfront DAM y el portal de Brand Connect.

Los usuarios normales también pueden colaborar con otros creando y compartiendo lightboxes.

### Colaborador

Los usuarios con este tipo de función tienen acceso a Workfront DAM y al portal de Brand Connect.

Los colaboradores pueden ver, descargar, cargar, editar, mover y eliminar recursos y carpetas a los que tienen acceso. Además, los colaboradores pueden colaborar con otros creando y compartiendo lightboxes. 

### Administrador

Los administradores de Workfront tienen acceso a todo lo que hay en el portal de Brand Connect y en Workfront DAM, incluidos los recursos que han caducado o que tienen un estado inactivo.

Para tener acceso de administrador, los usuarios con el tipo de rol Administrador deben estar en el grupo Administrador.
