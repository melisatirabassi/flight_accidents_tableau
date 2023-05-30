# Visualizacion en Tableau Public de Accidentes Aereos

Se realizo el análisis exploratorio del dataset AccidentesAviones.csv, que contiene información de los accidentes aéreos, con JupyterLab y luego se hizo un tablero con Tableau Public.

![Captura de pantalla 2023-05-24 a la(s) 12 01 26](https://github.com/santivalor/labs_2/assets/119902985/e1fd9e63-13b7-49f6-985b-e762136c4f4c)

# EDA

Se cambia el tipo de dato de algunas de las columnas ya que todas eran strings. Se obtienen columnas numéricas y de fechas según sea el caso.
A continuación, se detallan los pasos que se siguieron para realizar el EDA en JupyterLab del dataset AccidentesAviones.csv:

-Visualización de dataset: se observan las primeras 5 filas, se extrae la cantidad de filas y columnas, los nombres de las columnas y el tipo de dato por columna.

-Se cambia el carácter “?” por valores nulos.

-Se observa la cantidad de nulos por columnas.

-Se cambia el tipo de dato de algunas de las columnas ya que todas eran strings. Se obtienen columnas numéricas y de fechas según sea el caso.

-Se observa la cantidad de nulos por columna

-Se decide no utilizar las columnas con mayores cantidades de valores de nulos

-Se eliminan algunas filas con valores nulos de las columnas numéricas, sabiendo que eso puede afectar levemente los indicadores a visualizar luego en el tablero.

-Los valores nulos de las columnas tipo object se cambian por el string “sin_dato”.

-Se crean histogramas para visualizar el top 10 de las ruta, operadores y tipos de avión con mayor cantidad de accidentes aéreos, fallecidos en el avión y fallecidos en tierra.

-Se crean gráficos de líneas históricos con la cantidad de accidentes aéreos, fallecidos en el avión y fallecidos en tierra.

-Se exporta el nuevo dataframe en formato csv para ser utilizado en Tableau Public.

-Se exportan las filas eliminadas para corroborar que la mayoría de ellas no afecte la visualización de los últimos 5 años.


# Tableu Public 

Para realizar la visualización de los datos se utilizo Tableau Public. En el siguiente link se encuentra el tablero:

https://public.tableau.com/app/profile/melisa.tirabassi/viz/Dashboard_Accidentes_Aereos/Dashboard?publish=yes

Al usar Tableau Public solo se pudo importar los datos limpios en formato csv. El tablero consta de una portada y una hoja de visualización.
En el tablero se encuentra la siguiente información:
KPIs: evalúan el año en curso vs el año anterior. Sin tomar en cuenta que el año actual puede no haber terminado.

-Tasa de mortalidad: objetivo de reducir en 5% la tasa de mortalidad a nivel anual, siendo el número de fallecidos en los accidentes. aéreos respecto al total de personas en los vuelos involucrados

-Tiempo en accidentes: se pretende mantener el tiempo promedio anual entre accidentes consecutivos mayor a 40 días.

-Cantidad de accidentes: objetivo de reducir la cantidad de accidentes anual en 10%

-Daño colateral: mantener la cantidad anual de fallecidos en tierra (personas no presentes en los vuelos) en 0.

Gráfico de cantidad de accidentes por route-operadora-tipo de avión.
Gráfico histórico de cantidad de accidentes y fallecidos totales. Tooltip de cantidad de personas a bordo y cantidad de fallecidos.
Filtro para visualizar los dos gráficos según el rango de fechas elegido por el usuario.


<img width="1434" alt="Captura de pantalla 2023-05-29 a la(s) 22 16 05" src="https://github.com/melisatirabassi/flight_accidents_tableau/assets/124107756/b844a1a4-456d-4e71-b594-553a9fcd770e">




   












