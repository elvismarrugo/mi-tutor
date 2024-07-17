---
sidebar_position: 0
---

# Conociendo el software

![alt text](image.png)
![alt text](image-1.png)

| Fila | Columna | Color     | Hexadecimal |
|------|---------|-----------|-------------|
| 1    | 1       | Azul      | #4682B4     |
| 1    | 2       | Verde     | #32CD32     |
| 1    | 3       | Morado    | #9370DB     |
| 1    | 4       | Azul Claro| #87CEFA     |
| 2    | 1       | Azul Claro| #87CEFA     |
| 2    | 2       | Morado    | #9370DB     |
| 2    | 3       | Verde     | #32CD32     |
| 2    | 4       | Azul      | #4682B4     |


## 1. Decks

  #### **1. Decks**
      ```jsx
      La parte mas rellenado es cuando la musica es mas intensa y la mas finita, los bajones de la canción (ausencia de bombos)
      ```

  #### **2. HOT CUES**
      ```jsx
        1. Sirven para hacer referencia a las canciones, tiene 8
        2. Un click coloca un punto, dos click inicia la cancion desde alla
      ```
  #### **3. CUE**
    ```jsx
      Sirve para escuchar el canal por los auriculares  
    ```
  #### **4. LINEA DE TIEMPO PARCIAL**
    ```jsx
      La parte superior corresponde al Deck1 (izquierda)
      La parte inferior corresponde al Deck2 (Derecha)
    ```
      
  #### **5. BPM's: Beats por minuto**
    ```jsx
        Beats= 125 Bombos en cada minuto
        Compas= 4 Bombos
        Frase: 8 compases
    ```
  
  #### **6. Indicador Bombos**
    ```jsx
        5.2 Bars
        Compas = 5
        Bombos = 2
        Segundo bombo del quinto compas
        9.1 Bars
        Inicio Frase 8 Compases = 1 Frase
        Inicio frase coincide con un compas
    ```
  #### **7. Estructura musica en carpetas menor a 200 archivos **
    ```jsx
        * Año
        * Genero
        * Trimestre
        * Bases - Cantadas - Melodias
    ```
   #### **8. Mezcla **
    ```jsx
        Final de una cancion1 con principio de cancion2
        Cancion1:Primer bombo despues de un bajon - Hot Cue corte A
        Cancion2:Primer bombo despues de un bajon antes de la primera subida

    ```
  #### **9. Equalizacion **
    ```jsx
        Agudos: frecuencia alta notas agudas
        Medios: Melodia o voz del cantante
        Bajos: Bombo, frecuencia baja, La suma de las dos debe ser 100: 
          0% + 100%, 50% + 50%, 25% + 75%
    ```
  #### **10. Mezcla basica **
  ```jsx
      ajusto bpm en ambas canciones
      Cancion Saliente: quitar protagonismo
        inicio
          agudos: 100%
          medios: 100%
          graves: 100%
          volumen: 100%
      Cancion entrante: dar protagonismo
        inicio:
          agudos: 75%
          medios: 75%
          graves: 0%
          volumen: 0%
        entrada
          subo volumen hasta llegar al 100%
          subo agudos y medios hasta llegar al 100%
          en cambio de frase invierto los graves
          quito agudos y medios de cancion saliente
          meter efecto
  ```
#### **11. Mezcla al subidon **
    ```jsx
        ajusto bpm en ambas canciones
        mezclar las canciones en el bajon, para que ambas esten mezcladas al subidon
        mezclar segundo bajon de la cancion saliente con el primero de la cancion entrante
        Beat Jump Rekordbox
        colocamos el cursor en la primera cancion en el primer bombo del segundo bajon y le damos hacia 3 bloques de 32 bombos con beat jump:3 veces al 32
        hot cue y marcamos corte A
        colocamos el cursor en la segunda cancion en el primer bombo del primer bajon y le damos hacia 3 bloques de 32 bombos con beat jump:3 veces al 32
        hot cue y marcamos corte A
        cuando se unan se baja un poco el grave de una de las canciones
    ```
#### **12. Quitar cancion saliente **
    ```jsx
      1. Siguiente bajon de la cancion entrante, se baja el volumen
      2. Ambas en el subido, y se baja subitamente el volumen la de la saliente no se tocan los equalizadores
      3. no hacer nada, cuanda ambas estan por acabar
      4. con efectos, ejemplo filterm, izq(grave), der(agudo)
      5. bajar volumen y equalizadores
    ```
#### **13. Auriculares **
    ```jsx
      1. Conectar salida phones, cualquiera gama media
      2. Si el mixing esta en CUE y este esta activado sonara el canal
      3. Si el mixing esta en MASTER escucharemos lo mismo del publico
      4. Si esta en la mitad se escucharan ambos      
    ```
#### **14. Cuadrar a mano **
    ```jsx
      1. El pitch hacia abajo aumenta los bpm
      2. El pitch hacia arriba disminuye los bpm
      3. Se aconseja el 6% para manejar los rangos
      4. El jog wheel derecha:avanza - izquierda:retrocede
      5. se suelta la cancion1: izquierda y en cambio de frase se lanza la 2da
      6. con el jog, se ajusta atrasando o avanzando, si esta adelantada se le quita velocidad
      7. con el pitch, se ajusta arriba o abajo, si esta atrasada se le da velocidad
      8. primero con el jog y luego con el pitch
    ```
#### **15. Cuadrar a mano2 **
    ```jsx
      1. se coloca el mixing al 25% con el CUE activado para escuchar por los audifonos
      2. Primero se cuadra la cancion con los altavoces y luego se lanza
      3. Tecnica del 0.8% = 1 Bpm para canciones de 123-135 bpm
      4. Tempo Ring al 10%      
    ```
    | bpm | % | bpm     | % |
    |------|---------|-----------|-------------|
    | 1    | 0.8%       | 5 bpm      | 4.0%    |
    | 2    | 1.6%       | 6 bpm      | 4.8%    |
    | 3    | 2.4%       | 7 bpm      | 5.6%    |
    | 4    | 3.2%       | 8 bpm      | 6.4%    |

#### **16. Loops **
  ** Quantize: respeta el patron para que cada cosa caiga en su sitio **
    ```jsx
      1. Trozo de cancion que queremos que se repita de acuerdo a un tiempo 
         1. click en RELOOP, escogemos duracion 4,8, y click arriba para activar y es dinamico, se desactiva dandole click al numero y la cancion sigue por donde iba.
         2. Al darle click a IN, seleccionamos inicio del bucle y OUT el final y se activa, si damos click en EXIT, la cancion continua, pero memoriza el LOOP y accedemos pulsando RELOOP
         3. Mientras está sonando damos a IN, muestra el principio del LOOP con linea de tiempo parada y si pulsamos OUT, nos muestra el final
      2. IN inicio y OUT final, los botones <<(-) >>(+) controlan la duracion, EXIT sale del bucle
     
    ```
