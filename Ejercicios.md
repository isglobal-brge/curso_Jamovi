# Lectura y manejo de datos

**Ejercicio 1:** Importa los datos `Test_Condicion_Fisica.txt` a Jamovi, crea las siguientes variables y guarda el fichero con las nuevas variables en formato Jamovi:

1. `Abdominals_2`que contenga el número de abdominales en 10 segundos
2. `Velocitat_zscore` que contenga la velocidad estandarizada (resta la media y divide por la desviación típica). 
3. `Salt_zscore` que contenga la distancia del salto estandarizado. 
4. `IPAQ_ln` que contenga el logaritmo neperiano del IPAQ.
5. `IMC_cat` que sea`:

> * `bajo` para IMC<20
> * `normal` para 20>=IMC<25
> * `alto` para IMC>=25

**Ejercicio 2:** Importa los datos `multicentric.txt` a Jamovi. Estos datos contienen la información de un estudio de casos y controles (variable `status`) para conocer los factores de riesgo para el cáncer de Cervix. Crea las siguientes variables y guarda el fichero final en formato Jamovi:

1. `continente` una variable que contenga el continente (América, Africa, Europa, Asia) en función del pais (variable `pais`).
2. `edad1sex_rec` que contenga una variable que indique si la mujer tuvo su primera relación sexual (variable `edad1sex`) antes de los 15 años o no (<15).
3. `nembara_zscore` que contenga el número de embarazos (variable `nembara`) standarizada.


**Solución ejercicio 1** 

IF(pais="Brasil" or pais="Colombia" or pais="Peru", "America", IF(pais="España", "Europa", IF(pais="Tailandia" or pais="Filipinas", "Asia", IF(pais="Marruecos", "Africa"))))


# Estadísica descriptiva

**Ejercicio 4** Contesta a las siguientes preguntas usando las variables que has obtenido tras realizar el ejercicio 1:

1. Describe la variable `sexo`.
2. Describe la variables `IPAQ`  e `IPAQ_ln`. ?Qu? conclusi?n podemos obtener de este an?lisis descriptivo?
2. ?Qu? variable es m?s dispersa, el n?meo de saltos o el de abdominales?
3. ?Qu? n?mero de abdominales deber?a realizar un hombre para estar en el percentil 95? ?y una mujer?
4. Describe gr?ficamente la variable `IPAQ` para hombres y mujeres.
5. Describe gr?ficamente la variable `IPAQ` e `IPAQ_ln`seg?n la variable `IMC_cat`. 
6. ?Qu? conclusiones podemos obtener de los tres gr?ficos anteriores?
7. ?Qu? tipo de relaci?n existe entre el `IMC_cat` y el sexo de los participantes? 

**Ejercicio 5**  Contesta a las siguientes preguntas usando las variables que has obtenido tras realizar el ejercicio 2:

1. ?Qu? pais aporta m?s casos de c?ncer al estudio? ?y qu? continente?
2. ?Cu?l es la frecuencia de casos en Filipinas? ?Y de controles?
3. Describe gr?fica y num?ricamente la variable `edad1sex` para casos y controles. ?Qu? conclusi?n se puede extraer?
4. ?Cu?l es la relaci?n entre la variable `vph` (positivo, negativo) y `status` (caso, control)?
5. ?Qu? relaci?n existe entre la variable `edad1sex` y `edademba`?
6. ?Cu?l es el rango intercuart?lico para la variable `nembara`?
7. ?Cu?l es el percentil 90 de la variable `edad1sex` en casos? ?y en controles?
