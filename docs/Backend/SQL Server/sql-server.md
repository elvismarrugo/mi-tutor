---
sidebar_position: 0
---

# Fechas en SQL

## Colocar formato fecha en SQL Server

```jsx
    format(l.fecha,'dd/MM/yyyy') as FechaDesembolsoInicial
```

## Concatenar fecha texto en SQL Server

```jsx
    'Texto'+UPPER(convert(varchar,format(FECHA,'MMM yyyy'))) AS 'Texto',
```

## Agregar mes a fecha con formato fecha en SQL Server

```jsx
    format(DATEADD(month,l.periodos,l.fecha),'dd/MM/yyyy') as FechaVencimiento
```