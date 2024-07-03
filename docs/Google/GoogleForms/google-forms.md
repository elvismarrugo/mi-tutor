---
sidebar_position: 1
---

# Apps Script

## Funciones:

Presiona **tecla del logotipo de Command + Mayús + 4**. El escritorio se oscurecerá mientras seleccionas un área para la captura de pantalla.


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
