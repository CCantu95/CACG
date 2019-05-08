# Requisitos 
Instalar python, [numpy](https://www.numpy.org/), [scipy](https://www.scipy.org/) y [matplotlib](https://matplotlib.org/).

# Correr un programa
Abre terminal y corre python main.py NOMBRE_ARCHIVO.cag, recuerda ejecutar esta acción dentro se encuentren los archivos.

# Variables
Las variables se declaran con un % precedido de cualquier caracter, después le sigue un : y el tipo de dato, que puede ser entero o decimal.

## Locales
Las variables locales sólo se pueden utilizar en las funciones declaradas o en el main.

## Globales
Las variables globales se pueden utilizar desde donde sea.

## Arreglos
Las variables arreglo tienen la misma sintaxis que una variable normal, con el cambio de que se añade un [ENTERO].

# Condiciones
Las condiciones sirven para ejecutar código dependiendo del resultado de la comparación de dos valores.

## Operadores relacionales
- < menor que
- \> mayor que
- <= menor o igual que
- \>= mayor o igual que
- == igual igual que
- != no es igual que

## Si
Condición para ejecutar una acción de acuerdo a una comparación

      si(4 > 10){
        algo
      }
      
## Sino
Condición para tener dos opciones a ejecutar de acuerdo a una comparación
 
      si(4 > 10){
        algo
      }sino{
        algo
      }
      
# Ciclos
Se utiliza para ejecutar una acción hasta que el resultado de una comparación equivalga a algo. Se utiliza la palabra mientras, poniendo la comparación dentro del paréntesis.

     %i = 0;
     mientras(%i < 5){
        algo
        %i = %i + 1;
     }
     
# Funciones
Se utilizan para reutilización de código, así como la modularización de un programa. Requiere la palabra función seguido de : y tipo de dato, los cuales pueden ser entero, decimales y void.

## Parámetros
Los párametros son datos que son pasados como valor a una función, por ello no necesitan ninguna declaración.

## Tipos de funciones
Las funciones tienen 3 tipos: entero, decimal y void. Una función de tipo entero, tiene un valor de retorno entero, mientras que una función de tipo decimal, tiene un valor de retorno decimal. Sin embargo, las funciones void, no tienen ningún retorno, por lo que no generan un resultado.

# Funciones generales
Estas funciones sirven para leer e imprimir datos, así como la inclusión de comentarios en el programa.

## Leer
Esta función tiene como propósito recibir un input del usuario, se codifica poniendo la palabra leer antes de incluir la variable que desea ser leída.

## Imprimir
Sirve para desplegar información en consola, se codifica poniendo la palbra desplegar antes de incluir la variable, función o número que se desea desplegar en consola.

## Comentarios
Se utiliza // para comentar una línea 

# Funciones del lenguaje

Estas funciones tienen como propósito generar estadísticas descriptivas, así como gráficos para interpretar la información de un archivo de texto.

## Estadísticas
Se utiliza la palabra de la estadística: media, mediana, moda, varianza, desviación, asimetría o curtosis, precedido del nombre del archivo, una coma y un número entre 0 y 2, el cuál representa la columna que se quiere tomar del archivo, siendo 0 la columna 1, 1 la columna 2 y 2 ambas columnas.

    media "data.txt",0;
    mediana "plot_data.txt",2;
    moda "plot_data.txt",2;
    varianza "data.txt",0;
    desviacion "plot_data.txt",2;
    asimetria "plot_data.txt",1;
    curtosis "plot_data.txt",0;
    
## Plot

Se utiliza la palabra graficar precedido del nombre del archivo, coma, caracter de marcador, un número que indica el grosor de la línea, coma color, coma etiqueta.

## Histograma

Se utiliza la palabra histograma precedido del nombre del archivo, coma, un número que representa los bins, y cuatro strings que representan las etiquetas y colores de las gráficas.

## Boxplot

Se utiliza la palabra caja precedido del nombre del archivo, coma, dos strings que representan las etiquetas de los boxplots y un número que puede ser 0 y 1. Siendo 1 verdadero y 0 falso para poner en vertical el boxplot.
