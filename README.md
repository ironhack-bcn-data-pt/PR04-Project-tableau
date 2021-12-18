![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Business Intelligence with Tableau

## Overview

El objetivo de este proyecto es el de mostrar cómo han evolucionado la economía de 5 países sudamericanos a lo largo de 4 décadas (1980-2020). Una vez presentados la evolución de los indicadores macroeconómicos más relevantes los comparamos y clasificamos las economías en función de su evolución para cada década.

Queremos también descubrir si la ideología de los gobernantes de cada país a lo largo de los años afecta a la evolución de la economía.

---

## Indicadores macroeconómicos y paises

Los indicadores que han sido seleccionados para mostrar la evolución de cada economía son:
* Crecimiento anual porcentual del PIB (calculado a precios constantes)
* Indice de Desarrollo Humano Anual (sólo hay datos a partir de 1990)
* Tasa de paro anual
* Deuda Externa Total sobre el PIB anual a precios corrientes (en $) anual.
* Indice de Precios al Consumidor anual.

Los países seleccionados han sido:
* Argentina
* Brasil
* Chile
* Paraguay
* Venezuela

## Recopilación de datos

Información de Gobiernos: hemos recopilado datos de presidente, partido e ideología económica de cada país por año a través de escrapear las tablas “Annexo presidentes” de la Wikipedia.

No hemos encontrado una fuente de datos que agrupe toda la información necesaria para nuestros indicadores. Por lo tanto, hemos tenido que crear nuestro dataset a partir de varias fuentes de datos:
* CEPALSTAT: CEPAL es una comisión regional de las Naciones Unidades para América Latina y el Caribe. En su página web CEPALSTAT disponemos una amplia base de datos para estos países. Aquí hemos obtenido datos para el PIB, Tasa de paro, Deuda Externa y IPC.
* World Bank: Esta institución mundial financiera dispone de una amplia base de datos económicos sobre la mayoría de país del mundo. Aquí hemos obtenido los datos que nos faltaba para el PIB.
* Programa Naciones Unidas para el Desarrollo: Agencia de las Naciones Unidas cuyo objetivo es la erradicación de la pobreza y la reducción de las desigualdades de los países. En su página web obtenemos datos del IDH desde 1990.

## ETL en Jupyter Notebook

# Procesos iniciales
* Hemos importado CSV y archivos JSON.
* Hemos transformado los datos para que sean homólogos y hemos creado 14 tablas diferentes para relacionarlas en una base de datos relacional cargada en PostgreSQL.
# Procesos posteriores
* Desde tableau hemos agrupado los indicadores por décadas y hemos generado un ranking por países a partir de una valoración subjetiva de los indicadores de cada país. La clasificación se ha guardado en un Excel. Este Excel se ha cargado en el notebook y se ha subido y relacionado en la base de datos de PostgreSQL.
* Investigando la historia económica de cada país hemos creado un Excel con la explicación de las políticas económicas de cada país en cada década.

## Tableau

Hemos creado gráficos para cada indicador y para cada década y lo hemos relacionado todo en 5 dashboards (4 décadas y 1 acumulado)

## Presentación

Hemos publicado los dashboards en tableau public y los hemos incrustado en una página web para crear una historia visual a partir de un scroll

## Conclusiones

Se observa que si bien los países que han tendido a tener gobiernos de ideología neoliberal han presentado mejores indicadores no podemos afirmar que sea determinante. Por ejemplo en Chile se fue alternando gobernantes liberales y socialdemócratas y no afectó a su evolución económica. 

Un indicador con mayor relevancia podría ser la estabilidad social/política. Por ejemplo: Chile y Paraguay versus Argentina y Venezuela.



## Que hemos aprendido?
- Busqueda de datos abiertos
- Scrapping de tablas no estructuradas
- Planificacion y manejo de base de datos (Postgresql)
- Tableau
- Html

## Enlaces al resultado:
- 1980: https://public.tableau.com/app/profile/sergio7692/viz/1980SergioCarlos/Dashboard_80s
- 1990: https://public.tableau.com/app/profile/sergio7692/viz/1990SergioCarlos/Dashboard_90s
- 2000: https://public.tableau.com/app/profile/sergio7692/viz/2000SergioCarlos/Dashboard_00s
- 2010: https://public.tableau.com/app/profile/sergio7692/viz/2010SergioCarlos/Dashboard_10s
- Resumen 1980-2020: https://public.tableau.com/app/profile/sergio7692/viz/FinalSergioCarlos/Dashboard_FINAL
- Enlace a google drive con los datos e imagenes: https://drive.google.com/drive/folders/1V-lubVWK8wIYO7ltDYv3nRo_J4QaQ8GO?usp=sharing
- Enlace a la imagen de la base de datos: https://drive.google.com/file/d/1aMA4TwsL8nhSYS9Tog49TMc-Dq7kb8Sn/view?usp=sharing

# Enlaces de interes:
- Historia economica: http://countrystudies.us/brazil/
- IDH: http://hdr.undp.org/en/indicators/137506#
- Indicadores macroeconomicos: https://data.worldbank.org/
- Presidentes: Wikipedia.com
