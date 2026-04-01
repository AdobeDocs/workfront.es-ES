---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Mensajes de confirmación de Git

Aplicar siempre esta regla. Cuando redacte o genere un mensaje de confirmación de Git (por ejemplo, en el cuadro de confirmación de Control de Source o cuando se le pida en el chat del agente), siga este formato.

## Línea de asunto (solo primera línea)

- Alrededor de **50 caracteres o menos**.
- Resuma el cambio en **estado de ánimo imperativo** (por ejemplo, &quot;Agregar...&quot;, &quot;Corregir...&quot;, &quot;Refactorizar...&quot;).

## Línea en blanco

Deje una **línea en blanco** después del asunto antes del cuerpo.

## Cuerpo (descripción detallada)

- Ajustar líneas a **72 caracteres** aproximadamente (incluyendo el prefijo y el espacio de la viñeta).
- Utilice **líneas de viñetas** para la explicación. Cada viñeta debe comenzar exactamente con una de:
   - **📖** — usar cuando el cambio **agregue** algo nuevo: nuevos archivos, nuevas secciones, nuevas características, nuevos encabezados, nuevas líneas u otro contenido de tipo &quot;greenfield&quot;.
   - **✏️** — usar cuando el cambio **modifique** trabajo existente: edita las líneas existentes, actualiza las secciones existentes, refactoriza el código existente o cambia el contenido actual.

Aplique **📖** o **✏️** a cada viñeta de cuerpo para que quede claro qué se introdujo y qué se alteró.

## Plantilla

Rellene los marcadores de posición (no deje corchetes angulares en el mensaje final):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Ejemplo

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
