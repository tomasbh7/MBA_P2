# MBA_P2
Repositorio para la práctica 2 del Seminario A Modelado Basado en Agentes- Semestre 2027-1

Contenido:

|-Barrera_Hernandez_Alonso_Diaz

          |---------- Practica2

                    |---------- Fuentes
                    
                    |---------- ReadmeP1.txt
                    
                    |---------- ReadmeP2.txt
                    
                    |---------- ReadmeP3.txt
                    
                    |---------- Solucion.pdf
                    
                    |---------- PresetacionProyecto.pdf/ppt

#Programa Segregación:
Crea agentes en la cuadrícula y se reparten en 3 grupos del mismo tamaño, donde cada uno recibe una similitud requerida, la cual está tomada a partir de la distribución normal (de 0 a 100) y los agentes que no estén satisfechos se mueven a un patche vacío hasta estar satisfechos con la similitud que se pide de acuerdo a los parámetros que se indican en la interfaz.
El programa se ejecuta primero presionando setup para reiniciar todo, luego presionando go.
Parámetros:
-Densidad: Es el porcentaje de patches que se ocupan por los agentes.
-Media-similitud: Media de la distribución normal de la similitud requerida, usada por todos los agentes cuando parámetros-iguales? está encendido .
-Desviación-similitud: Es la desviación estándar de la distribución, usada en el mismo caso de la Media-similitud, donde entre más grande sea más heterogéneas son las tolerancias de los agentes.
-media-naranja: Es la media de la similitud requerida para el grupo de color naranja que se usa si parametros-iguales? está apagado
-media-verde: Es la media de la similitud requerida para el grupo de color verde que se usa si parametros-iguales? está apagado
-media-azul: Es la media de la similitud requerida para el grupo de color azul que se usa si parametros-iguales? está apagado
-sd-naranja: Es la desviación estándar de la similitud requerida para  el grupo naranja, que se usa cuando parametros-iguales? está apagado
-sd-verde:  Es la desviación estándar de la similitud requerida para  el grupo verde, que se usa cuando parametros-iguales? está apagado
-sd-azul:  Es la desviación estándar de la similitud requerida para  el grupo azul, que se usa cuando parametros-iguales? está apagado
-parametros-iguales?: Es el interruptor para que los tres grupos usen la misma media-similitud y desviacion-similitud si está prendido y en caso contrario cada grupo de color usa sus propios parámetros.

Gráfica de porcentaje de similitud:Solo es una gráfica que nos va indicando el número de agentes insateisfechos con relación al tiempo (ticks)

#Programa de Termitas
Para este programa, cada termita que se determina en la poblacion camina al azar, recoge una madera, busca un cumulo del mismo color, la deja en su lugar y se aleja, para las maderas estas estan divididas en dos colores que son amarillo y rosa, se pueden cambiar los parametros con los sliders y los switches
-Poblacion: Es el numero de termitas
-Densidad: Porcentaje de patches que empiezan con una madera
-salto?: es una opcion que agregue para cambiar entre hacer el salto y no hacerlo para la graficacion, con off la termita se aleja caminando, con On cuando la termita suelta la madera salta a una posicion aleatoria del mundo

#Programa de Hormigas
Las hormigas estan en una reticula con una en cada celda, en donde mediante la formula del articulo la actividad de cada hormiga se va actualizando.
Cuando una hormiga esta activa si S supera el umbral, entonces las activas se empiezan a mover al azar una celda por cada paso, ademas las hormigas inactivas se pueden activar espontaneamente con una probabilidad.
-botones de activar-uno y varios fueron para hacer pruebas de activacion de hormigas.
-lado: Es el tamaño de la reticula en donde el predeterminado es de 10
-densidad: Son las celdas ocupadas en donde se uso para el reporte los valores de 0.06 hasta 0.9
-g: Es la ganancia de la tangente hiperbolica en donde use el 0.09 en el reporte
-umbral: Valor minimo de S para considerar una hormiga activa, use 0.01
-prob-espontanea: es la probabilidad por paso para que se active una hormiga sola, use 0.009
-monitor actividad: registra el numero de hormigas activas
-monitor de n-espontaneo: son el numero de activaciones espontaneas acumuladas
-grafica Actividad que esta en funcion al tiempo
