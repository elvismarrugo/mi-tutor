---
sidebar_position: 0
---

# Funciones DAX

1. La funcion  **VALUES**. permite crear una tabla con valores unicos.

        #### **VALUES**
        ```jsx
        Fx Values = VALUES(Productos[Nombre Producto])
        ```


2. La funcion  **DISTINCT**. permite crear una tabla con valores unicos, NO trae filas en blanco de las relaciones.

        #### **DISTINCT**
        ```jsx
        Fx Distinct = DISTINCT(BD[Nombre Cliente])
        ```

3. La funcion  **ALL**. permite crear una tabla con valores unicos, pero permite traer mas de una columna

        #### **ALL**
        ```jsx
        Fx ALL = ALL( BD[Nombre Cliente],BD[Sucursal])
        ```

4. La funcion  **ALLEXCEPT**. permite crear una tabla con valores unicos, trae todo menos las columnas en la consulta.

        #### **ALLEXCEPT**
        ```jsx
        Fx ALL = ALLEXCEPT( BD[Nombre Cliente],BD[Sucursal])
        ```

5. La funcion  **SUMMARIZE**. Toma la tabla transaccional(hechos) y agrupa(resume) .

        #### **SUMMARIZE**
        ```jsx
        Fx SUMMARIZE = SUMMARIZE(BD,Vendedores[Nombre Vendedor],Productos[Nombre Producto])
        ```

5. La funcion  **FILTER**. Filtra los datos de una sola tabla, puede usar AND(&&) - OR(||).

        #### **FILTER**
        ```jsx
        Fx Filter = FILTER(BD,
                (BD[Sucursal]="NORTE" && BD[Cod_Depto]="08" ) &&
                (BD[Nombre Linea]="FIT" || BD[Nombre Linea]="HELADOS")
                )
        ```