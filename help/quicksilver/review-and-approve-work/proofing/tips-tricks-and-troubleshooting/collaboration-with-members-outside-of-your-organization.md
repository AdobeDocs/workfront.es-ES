---
title: Revisión de las limitaciones de colaboración con personas ajenas a la organización
description: Revisión de las limitaciones de colaboración con personas ajenas a la organización
author: Courtney
draft: Probably
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%
---
# Revisión de las limitaciones de colaboración con personas ajenas a la organización

Existen algunas limitaciones que se deben tener en cuenta al comunicarse con personas ajenas a la organización cuando se añaden a una prueba, específicamente si la persona ajena a la organización tiene acceso a la revisión en un entorno independiente.

## Contactos con la distinción de Miembro

Existen tres tipos de contactos en un entorno de revisión:

* **Usuarios**: los usuarios tienen un inicio de sesión de Workfront Proof en el entorno de su organización.
* **Miembros**: los miembros tienen su propio inicio de sesión de Workfront Proof en el entorno de otra organización (no en la de usted). No puede convertir miembros en usuarios de su entorno.
* **Invitados**: los invitados no tienen su propio inicio de sesión de Workfront Proof en el entorno de su organización, pero usted ha añadido sus detalles a su cuenta (por ejemplo, los revisores invitados en las pruebas). Puede convertir invitados en usuarios.

Dado que los miembros no se pueden convertir en usuarios, su capacidad para etiquetar a las personas en los comentarios de las pruebas está limitada a los usuarios de *su organización original*.

**Ejemplo:** la compañía A invita a un usuario externo a revisar una prueba. Este usuario ya existe en un entorno de prueba independiente, la compañía B.

 

Cuando la compañía A invita al usuario externo a la prueba, el usuario externo se añade a la lista de contactos de la compañía A como miembro. Los revisores del flujo de trabajo de prueba de la compañía A pueden etiquetar al usuario externo en los comentarios de prueba porque ahora se encuentran en el directorio de contactos de la compañía A.

 

El usuario externo no puede etiquetar usuarios de la compañía A aunque estén en el mismo flujo de trabajo de prueba, ya que los usuarios de la compañía A no se han añadido como contactos a la compañía B.

 

El usuario externo de la compañía B puede etiquetar a otros usuarios de la compañía B si están en el flujo de trabajo de prueba o si tienen permiso para compartir la prueba con nuevos usuarios porque esos usuarios existen como contactos en la compañía B.
