---
name: clean-el-traffic-csv
description: Limpia una exportación de CSV de tráfico de Experience League/Adobe Analytics sin procesar a páginas solo de Workfront, ordenadas por Vistas de página. Se utiliza cuando el usuario proporciona un CSV de tráfico de páginas de Experience League (columnas como "URL genérica de página", "Visitantes únicos", "Visitas", "Vistas de página") y solicita limpiarlo, filtrarlo o procesarlo, o menciona las hojas de cálculo de "seguimiento de documentación" o "artículos más vistos".
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# Limpiar CSV del tráfico de Experience League

Convierte una exportación sin procesar de tabla de forma libre de Adobe Analytics del tráfico de páginas de Experience League en un CSV limpio, solo para Workfront, deduplicado y ordenado por Vistas de página, sobrescribiendo el archivo original y también guardando una copia con fecha en el escritorio.

## Formas de entrada

La entrada puede ser una de las dos formas:

1. **Exportación sin procesar**: comienza con las líneas de comentarios de metadatos (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"`, etc.), seguidas de una tabla de desglose jerárquico (por ejemplo, `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → filas de URL individuales). La celda literal `Page URL Generic (v33)` (o una etiqueta `Page URL Generic ...` similar) aparece a mitad de camino, en la segunda columna.
2. **CSV ya limpio**: la primera fila ya es un encabezado sin formato como `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, sin filas de metadatos ni columnas iniciales adicionales.

Detecte qué forma tiene antes de empezar: si la fila 1 es una fila de encabezado sin formato que coincide con la forma 2, vaya directamente al paso 2 (no habrá disponible ningún intervalo de fechas, por lo que omita el paso 7 a menos que el usuario proporcione un intervalo de fechas por separado).

## Flujo de trabajo

### Paso 0: Capture el intervalo de fechas (solo exportación sin procesar, antes de eliminar nada)

Busque la línea de metadatos cerca de la parte superior que coincide con `# Date: <range>` (p. ej. `"# Date: Jul 1, 2026 - Jul 31, 2026"`). Registro `<range>` (p. ej. `Jul 1, 2026 - Jul 31, 2026`): se necesita más adelante en el paso 7. Haga esto antes de eliminar filas.

### Paso 1: Reduzca la exportación sin procesar a una tabla sin formato (solo exportación sin procesar)

1. Busque la fila que contiene la celda `Page URL Generic (...)` (se encuentra en la segunda columna de la exportación estándar).
2. Elimine todas las filas por encima de esa fila, incluidas las líneas de comentarios de metadatos y las filas de subtotal `Solution (v2)` / `workfront`.
3. Elimine todas las columnas a la izquierda de la celda `Page URL Generic` (en la exportación estándar, se trata solo de la columna A).
4. En esa misma fila (ahora fila de encabezado), reemplace los valores numéricos de subtotal a la derecha de `Page URL Generic (...)` por los encabezados literales, en orden: `Unique Visitors`, `Visits`, `Page Views`. Deje la celda `Page URL Generic (...)` sin cambiar.

Resultado: un CSV sin formato con el encabezado `Page URL Generic (v33),Unique Visitors,Visits,Page Views` seguido de una fila por URL.

### Paso 2: Mantener solo filas de Workfront

Para cada fila de datos, compruebe si la dirección URL contiene la subcadena literal `/workfront/` (barra diagonal en ambos lados). El prefijo de configuración regional no importa (`/en/`, `/zh-hans/`, etc.; permanezcan todos mientras coincida el segmento de producto).

- Elimine la fila si la dirección URL **no** contiene `/workfront/` como segmento de ruta de acceso; esto elimina otros productos como `workfront-fusion`, `workfront-learn`, `proofhqpapi`, etc. (una subcadena como `tutorials-workfront` cuenta **no**; la coincidencia debe ser el segmento exacto `/workfront/`).
- De lo contrario, mantenga la fila.

### Paso 3: Recortar la dirección URL

Para cada fila superviviente, busque `/using` en la dirección URL y guarde solamente la parte del `/` que lo sigue en adelante (incluyendo), descartando todo lo anterior a `/using` e incluido.

Ejemplo: `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

Si no se encuentra `/using` en la dirección URL de una fila de Workfront, deje esa dirección URL sin cambiar y márquela para el usuario en lugar de adivinar.

### Paso 4: Eliminar fragmentos/sufijos de consulta

Si la dirección URL recortada contiene `#` o `?`, elimine ese carácter y todo lo que haya después.

Ejemplo: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Paso 5: Combinar duplicados

Después del recorte, varias filas ahora pueden compartir la misma dirección URL (por ejemplo, dos filas de configuración regional diferentes que se contraen en la misma ruta). Combine todas las filas con una dirección URL idéntica en una fila, sumando `Unique Visitors`, `Visits` y `Page Views` de forma independiente.

Ejemplo: `/home,2,2,3` y `/home,5,6,7` → `/home,7,8,10`

### Paso 6: Ordenar por Vistas de página

Ordene todas las filas de datos por `Page Views` en orden descendente (primero el más grande). La fila de encabezado permanece fija en la parte superior, sobre los datos ordenados.

### Paso 7: Añada la fila de intervalo de fechas (solo exportación sin procesar, si se captura en el paso 0)

Antes de insertarlo, elimine todas las comas del intervalo de fechas capturado (por ejemplo, `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`); el intervalo sin procesar tiene comas que, de lo contrario, se malinterpretarían como separadores de columnas CSV en esa fila.

Inserte una fila nueva en la parte superior, encima de la fila de encabezado, que contenga únicamente el intervalo de fechas sin comas.

Orden de fila final: fila de intervalo de fechas → fila de encabezado → filas de datos ordenadas.

### Paso 8: Guardar

Sobrescriba el archivo de entrada original con el resultado limpiado.

### Paso 9: guardar una copia con fecha en el escritorio (solo exportación sin procesar, si se capturó un intervalo de fecha en el paso 0)

Cree una versión con nombre de archivo seguro del intervalo de fechas: elimine las comas y reemplace cualquiera de `\ / : * ? " < > |` por `-` (estos caracteres no son válidos en los nombres de archivo de Windows y podrían aparecer en un intervalo de fechas según la configuración regional o el formato de exportación).

Guarde una copia adicional del CSV limpiado (el mismo contenido que en el paso 8) en el escritorio del usuario actual, con el nombre:

`Documentation tracking report <filename-safe date range>.csv`

Ejemplo: un intervalo capturado de `Apr 1, 2026 - Apr 30, 2026` se convierte en `Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`.

Omita este paso para un CSV ya limpio (forma 2) a menos que el usuario proporcione un intervalo de fechas por separado.

## Fuera de ámbito

Publicar o compartir el CSV limpiado (por ejemplo, en Slack) es un paso independiente que aún no se ha definido. No intente adjuntar ni cargar el archivo en ningún lugar como parte de esta aptitud.

## Implementación (exportación en bruto)

Para una exportación sin procesar, ejecute los pasos del 0 al 8 con este script de PowerShell probado en lugar de editar filas a mano; es más rápido y menos propenso a errores en archivos con cientos de filas. Sustituya la ruta de acceso del archivo real de `$path`.

Antes de ejecutar, compruebe si el archivo está bloqueado (por ejemplo, abierto en Excel): si `Set-Content` falla y &quot;otro proceso lo está utilizando&quot;, pídale al usuario que lo cierre y vuelva a ejecutar el archivo.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

Para un CSV ya limpio (forma de entrada 2), omita la reubicación del encabezado, la lógica de intervalo de fechas y el paso 9: ejecute los pasos 2-6 y 8 en el encabezado o las filas existentes tal cual.
