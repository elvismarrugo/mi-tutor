---
sidebar_position: 0
---

# Fechas en SQL

## Colocar formato fecha en SQL Server

```jsx
    format(l.fecha,'dd/MM/yyyy') as FechaDesembolsoInicial
```

## Agregar mes a fecha con formato fecha en SQL Server

```jsx
    format(DATEADD(month,l.periodos,l.fecha),'dd/MM/yyyy') as FechaVencimiento
```