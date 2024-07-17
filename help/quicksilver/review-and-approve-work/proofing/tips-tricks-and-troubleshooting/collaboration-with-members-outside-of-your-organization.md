---
title: Corrección de las limitaciones de colaboración con personas ajenas a la organización
description: Corrección de las limitaciones de colaboración con personas ajenas a la organización
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Corrección de las limitaciones de colaboración con personas ajenas a la organización

Existen algunas limitaciones que se deben tener en cuenta al comunicarse con personas fuera de la organización cuando se añaden a una prueba, específicamente si la persona fuera de la organización tiene acceso a la prueba en un entorno independiente.

## Contactos con la distinción de Miembro

Existen tres tipos de contactos en un entorno de prueba:

* **Usuarios**: Los usuarios tienen un inicio de sesión de Workfront Proof en el entorno de su organización.
* **Miembros**: Los miembros tienen su propio inicio de sesión de Workfront Proof en el entorno de otra organización (no el suyo propio). No puede convertir miembros en usuarios de su entorno.
* **Invitados**: Los invitados no tienen su propio inicio de sesión de Workfront Proof en el entorno de su organización, pero usted ha agregado sus detalles a su cuenta (por ejemplo, los revisores invitados en las pruebas). Puede convertir invitados en usuarios.

Dado que los miembros no se pueden convertir en usuarios, su capacidad para etiquetar a las personas en los comentarios de las pruebas está limitada a los usuarios de *su organización original*.

**Ejemplo:** La compañía A invita a un usuario externo a revisar una revisión. Este usuario ya existe en un entorno de prueba independiente, Empresa B.

 

Cuando la Empresa A invita al usuario externo a la prueba, el usuario externo se añade a la lista de contactos de la Empresa A como Miembro. Los revisores del flujo de trabajo de prueba de la compañía A pueden etiquetar al usuario externo en los comentarios de prueba porque ahora se encuentran en el directorio de contactos de la compañía A.

 

El usuario externo no puede etiquetar usuarios de la compañía A aunque estén en el mismo flujo de trabajo de prueba, ya que los usuarios de la compañía A no se han agregado como contactos a la compañía B.

 

El usuario externo de la compañía B puede etiquetar a otros usuarios de la compañía B si están en el flujo de trabajo de prueba o si tienen permiso para compartir la prueba con nuevos usuarios porque esos usuarios existen como contactos en la compañía B.
