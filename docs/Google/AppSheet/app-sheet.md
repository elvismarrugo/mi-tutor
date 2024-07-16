---
sidebar_position: 1
---

# AppSheet

## Carpetas:

Lo ideal es que todo quede guardado en una misma carpeta y crear un libro por cada tabla para tablas que manejaran muchos registros(dinamicas) y un libro con tablas estaticas.

Tablas maestras
Tablas operaciones

en las tablas de operaciones es recomendado tener IdNombre y Nombre

Complemento Size My Sheet, permite saber cuanto hemos gastado en el libro de googlesheets

Al crear la primera tabla en AppSheet, se debe reubicar en carpeta, Storage - SourcePath, buscar data, seleccionar carpeta y guradar cambios.

La tabla de menu es de solo lectura


El campo IdNombre, debe ser tipo ref y escoger la otra tabla ej Nombre
el campo Nombre, debe ser tipo text y la formula [IdNombre].[Nombre]
La columna Show se debe desmarcar para el campo dual
y la columna Display Name toma el nombre del campo dual


Valid If
SELECT(Operador[Operador], [TipoServicio] = [_THISROW].[TipoServicio])


Suggested values
ORDERBY(Operador[IdOperador],[Operador],false)


Presiona **tecla del logotipo de Command + Mayús + 4**. El escritorio se oscurecerá mientras seleccionas un área para la captura de pantalla.

LOWER([Email]): Convierte a minuscula
UPPER([Operador])  Convierte a Mayuscula


### Traer IDS
```jsx
   function traerIds() {
    var formulario=FormApp.openById
    ("id del form que contiene las preguntas")
    var items=formulario.getItems()
    items.forEach(item=>{
      Logger.log(item.getId().toString())
      Logger.log(item.getTitle())
      Logger.log(item.getType())
    })
  }
```

Si es primera vez se deben otorgar permisos

Esto nos mostrará el id de cada una de las pregunta, el cual está antes de cada pregunta

### Traer datos de la hoja opciones
```jsx
  function actualizarOpciones() {
    var formulario=FormApp.openById
    ("id del form que contiene las preguntas")
    var libro=SpreadsheetApp.getActiveSpreadsheet()
    var hoja=libro.getSheetByName("Opciones")
    var tiposId=hoja.getRange("A2:A").getValues()
    tiposId = tiposId.map(tipoId=>tipoId[0]).filter(tipoId=>tipoId)
    Logger.log(tiposId)
    var qTipoId=formulario.getItemById("id de la pregunta")  
    qTipoId.asListItem().setChoiceValues(tiposId)
  }
```

primera vez pedirá permisos

### Añadir "actualizarOpciones" a activadores "onOpen"  y "onEdit"

Validaciones

Email
```jsx
  "expresion regular": "coincidencias"
  email : "[a-zA-Z0-9_\.\+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-\.]+"
```
Celulares
```jsx
  "expresion regular": "coincidencias"
  celular : "^\d{10}$"
```
