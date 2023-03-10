---
sidebar_position: 0
---

# Fundamentos

Guía de rapida y practica de Tailwind css 🍭

¿Qué es?

Tailwind CSS es un Framework de CSS que principalmente brinda clases útiles para nuestros desarrollos web.

- [TailwindCSS](https://tailwindcss.com//)

## Instalacion Tailwind con Next.JS

- [Tailwind en NextJs](https://tailwindcss.com/docs/guides/nextjs/)


## Tabla de rellenos y margenes

|      Espaciado      | Padding | Margin  |
| ------------------- | ------- | ------- |
| Izquierda           | pl      | ml      |
| Derecha             | pr      | mr      |
| Arriba              | pt      | mt      |
| Abajo               | pb      | mb      |
| Arriba-Abajo        | py      | my      |
| Izquierda-Derecha   | px      | mx      |
| Centrado Horizontal | px-auto | mx-auto |

## Tabla de columnas

| Posicion | Columnas |
| -------- | -------- |
| w-full   | 1        |
| w-1/2    | 2        |
| w-1/3    | 3        |
| w-1/4    | 4        |
| w-1/5    | 5        |
| w-1/6    | 6        |


## Tamaño de fuente

|Clase       |    rem    |  px   | 
|------------|-----------|-------|    
| text-xs    | 0.75 rem  | 12 px |    
| text-sm    | 0.875 rem | 14 px |    
| text-base  | 1 rem     | 16 px |    
| text-lg    | 1.125 rem | 18 px |    
| text-xl    | 1.25 rem  | 20 px |    
| text-2xl   | 1.5 rem   | 24 px |    
| text-3xl   | 1.875 rem | 30 px |    
| text-4xl   | 2.25 rem  | 36 px |    
| text-5xl   | 3 rem     | 48 px |    
| text-6xl   | 4 rem     | 64 px |

## Flex direccional

|Clase   		 | Direccion	   	|    
|------------------|--------------------- |    
|flex-row    	 | izquerda -> derecha  |    
|flex-col    	 | arriba -> abajo      |    
|flex-row-reverse  | derecha -> izquerda  |    
|flex-col-reverse  | abajo -> arriba      |


## Justificar contenido horizontal

|Clase           |  Alineacion  | Modelo  |       
|----------------|--------------|---------|    
|justify-start   | inicio       |*--------|    
|justify-end     | final        |--------*|    
|justify-between | centrado     |----*----|


## Justificar contenido vertical

|Clase           |  Alineacion  | Modelo  |  
|----------------|--------------|---------|     
|items-start     | arriba       |*--------|      
|items-end       | abajo        |--------*|   
|items-center    | centrado     |----*----|   
|items-stretch   | se estiran   |----*----|