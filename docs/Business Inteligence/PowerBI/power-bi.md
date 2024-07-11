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
        
6. Operador  **IN**. Filtra los datos de una sola tabla, para varios criterios de una misma columna.

        #### **FILTER**
        ```jsx
       Operadores IN = FILTER(Calendario,Calendario[Nombre Dia] IN {"lunes", "martes","miércoles","jueves","viernes"})
        ```

7. Funcion  **IF** función lógica que evalúa una condición y devuelve un valor si la condición es verdadera y otro valor si la condición es falsa.

        #### **FILTER**
        ```jsx
     Semestre = IF(Calendario[Mes Num]<=6, "Sem1", "Sem2")
        ```        