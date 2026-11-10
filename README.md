<p align="center">
  <img src="https://raw.githubusercontent.com/maxicuyo94/mogura-releases/main/mogura.svg" alt="" width="96" height="96">
</p>

<h1 align="center">Mogura</h1>

<p align="center">
  Administrador de bases de datos para Windows: liviano, rápido y en español.<br>
  SQL Server y Azure SQL, PostgreSQL, MySQL y SQLite, en una sola app.
</p>

<p align="center">
  <a href="https://github.com/maxicuyo94/mogura-releases/releases/latest"><b>⬇ Descargar la última versión</b></a>
</p>

---

## Por qué Mogura

- **Liviana.** El instalador pesa unos 7 MB y la app abre al instante, sin Java ni nada extra.
- **Segura con producción.** Las conexiones de producción arrancan en solo lectura. Para escribir hay que habilitarlo con Windows Hello y confirmar. Un `UPDATE` o `DELETE` sin `WHERE` siempre pide confirmación.
- **Con Azure de verdad.** Se conecta a Azure SQL con tu cuenta de Microsoft (Entra ID), desde el navegador o con Azure CLI, y renueva la sesión sola.
- **Con un asistente de IA que no se manda solo.** Explica, arregla y optimiza consultas, pero lo que propone pasa al editor con un botón: nunca se ejecuta por su cuenta.

## Qué podés hacer

### Escribir y ejecutar SQL
- Editor con pestañas que se recuerdan al cerrar, resaltado y **autocompletado según tu esquema**: tablas, columnas, alias y joins por clave foránea.
- **Formatear SQL** con Shift+Alt+F.
- **Variables** `${nombre}` con valor por defecto, listas para elegir y calendario para fechas. Se completan en un panel al costado.
- **Historial** de lo ejecutado (cifrado, porque el SQL puede llevar datos) y **scripts guardados**.
- Se puede **cancelar** una consulta larga, y las filas llegan de a páginas, así que miles de resultados no traban la app.

### Ver y editar resultados
- Grilla que **ordena y filtra** sin volver a consultar, y muestra el tipo de cada columna y las claves.
- **Editar celdas** directamente: Mogura revisa tipo, largo, NULL y claves foráneas antes de guardar, y guarda todo en una transacción.
- **Exportar** a CSV o Excel, o copiar filas como `INSERT`.

### Trabajar con la base
- Árbol de objetos con tablas, vistas, funciones, procedimientos, índices y triggers, con el tamaño de cada tabla.
- **Diagrama del esquema** con las relaciones entre tablas, que se guarda como SVG.
- **Dump** de estructura y datos, de toda la base o de las tablas que elijas, con avance y cancelación.
- **Importar CSV o Excel** a una tabla, emparejando columnas. Arma los `INSERT` para que los revises antes de ejecutarlos.
- **Planilla**: abrí un CSV o un Excel y editalo como en Excel, conservando su formato.

### Asistente de IA (opcional)
- Panel de chat con Ctrl+K: **explicar**, **arreglar** un error u **optimizar** una consulta a partir de su plan de ejecución.
- **Texto gris** mientras escribís, que se acepta con Tab.
- Usa [Claude Code](https://claude.com/claude-code) con tu propia cuenta de Claude, sin claves de API. Solo recibe el esquema que hace falta, nunca tus filas. En producción viene apagado.

### Para todos los días
- Modo claro y oscuro.
- Toda la app en español.
- Se **actualiza sola**: al abrirse avisa si hay una versión nueva.

### Próximamente
Ya están hechas y llegan en la próxima versión:
- **Plan de ejecución visual**: un árbol con lo que va a hacer la base, las filas estimadas y lo que más cuesta, sin ejecutar la consulta.
- **Comparar esquemas** entre dos bases (por ejemplo, desarrollo y producción), con el script de diferencias.

## Instalar

1. Bajá `Mogura_X.Y.Z_x64-setup.exe` de la [última versión](https://github.com/maxicuyo94/mogura-releases/releases/latest).
2. Ejecutalo. No hace falta ser administrador.

Funciona en Windows 10 y 11 de 64 bits. Para el asistente de IA hace falta tener instalado Claude Code.

---

<sub>Este repo solo guarda las versiones publicadas: las apps instaladas consultan acá si hay una nueva (`latest.json` de la última versión).</sub>
