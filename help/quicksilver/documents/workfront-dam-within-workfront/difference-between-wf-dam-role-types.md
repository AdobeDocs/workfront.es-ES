---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Tipos de funciones de licencias de Adobe Workfront frente a tipos de funciones DAM de Adobe Workfront
description: Los administradores de Adobe Workfront utilizan niveles de acceso para determinar qué pueden hacer los usuarios en una aplicación.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Tipos de funciones de licencias de Adobe Workfront frente a tipos de funciones DAM de Adobe Workfront

Los administradores de Adobe Workfront utilizan niveles de acceso para determinar qué pueden hacer los usuarios en una aplicación.

* En Workfront, las licencias determinan el nivel de acceso de un usuario.
* En Workfront DAM, los tipos de funciones definen el acceso de los usuarios a los recursos en DAM.

Dado que los tipos de licencia y los tipos de rol no son intercambiables, tener un nivel de acceso en una aplicación no implica tener acceso en la otra aplicación. Por ejemplo, a un usuario con una licencia de trabajo en Workfront no se le asigna automáticamente una función de colaborador dentro de Workfront DAM.

## Tipos de licencia de Workfront

Como administrador de Workfront, puede definir el nivel de acceso que tienen los usuarios asignando tipos de licencia. Cada licencia viene con un conjunto de funciones de acceso predeterminadas que puede modificar antes de asignar la licencia al usuario. 

Las licencias se utilizan para determinar lo que un usuario puede ver y hacer en Workfront. Hay cinco tipos de licencias disponibles en Workfront:

* Plan
* Trabajo
* Revisar
* Solicitud
* Externo

Consulte [Resumen de licencias heredadas](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) para obtener una descripción de los diferentes tipos de licencias en Workfront.

## Tipos de roles DAM de Workfront

Como administrador de Workfront DAM Workfront, puede asignar tipos de funciones a los usuarios para definir el acceso que tienen a los recursos. Además, los tipos de funciones especifican las áreas de DAM en las que los usuarios pueden trabajar.

Los tipos de funciones funcionan junto con los Grupos al establecer los derechos de acceso de los usuarios. Los grupos controlan el acceso que los usuarios tienen a las carpetas y a los propios recursos. Los tipos de funciones determinan las acciones que los usuarios pueden realizar con los recursos. Todos los usuarios de DAM deben estar asociados con al menos un grupo. Para obtener más información sobre los tipos de funciones y la configuración de acceso, consulte la Ayuda de Workfront DAM.

Hay cuatro tipos de funciones diferentes disponibles en Workfront DAM:

### Brand Portal

Los usuarios con este tipo de función solo tienen acceso al portal de Brand Connect en DAM. En el portal, los usuarios pueden ver y descargar los recursos para los que tienen permisos.

Los usuarios de Brand Portal pueden colaborar con otros creando y compartiendo Lightboxes.

### Usuario normal

Los usuarios con este tipo de función pueden ver y descargar recursos desde Workfront DAM y el portal de Brand Connect.

Los usuarios normales también pueden colaborar con otros creando y compartiendo Lightboxes.

### Colaborador

Los usuarios con este tipo de función tienen acceso a Workfront DAM y a Brand Connect Portal.

Los colaboradores pueden ver, descargar, cargar, editar, mover y eliminar recursos y carpetas a los que tienen acceso. Además, los colaboradores pueden colaborar con otros usuarios creando y compartiendo Lightboxes. 

### Administrador

Los administradores de Workfront tienen acceso a todo lo que hay en el portal de Brand Connect y en Workfront DAM, incluidos los recursos que han caducado o que están inactivos.

Para tener acceso de administrador, los usuarios con el tipo de función Administrador deben estar en el grupo Administrador.
