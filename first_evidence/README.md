# **Módulo 5 | Procesamiento de datos multivariados**

_Autor: Myroslava Sánchez Andrade_
<br>_Fecha de creación: 05/10/2022_
<br>_Última modificación: 13/10/2022_

---

## **Visión general**

El propósito de este repositorio es el análisis de los estados financieros del primer trimestre del año 2022 de todas las empresas de la industria de servicios públicos de EE. UU. que están listados en el New York Exchange y NASDAQ utilizando álgebra lineal; siendo `['epsp', 'mediana empresa', 'gran empresa', 'margen de beneficio', 'libro/mercado', 'apalancamiento corto']` las variables explicativas (independientes) y `['f1 stock return']` la variable dependiente.

---

## **Configuración**

Para la realización de este proyecto se utilizó el archivo csv _[us_2022q1_service_industries.csv](https://github.com/myrosandrade89/IA95022/tree/main/Statistics/Reto/dataset)_ el cual fue extraído del repositorio: https://github.com/myrosandrade89/IA95022. De este archivo .csv sólo fueron extraídas las variables independientes y dependientes para el problema.

---

## **Exploratory analysis**

En este apartado, se llevaron a cabo los siguientes análisis utilizando álgebra lineal:

- Cálculo de la matriz de varianza-covarianza
- Cálculo de la matriz de correlación
- Detección de outliers y leverage points

---

## **Multicollinearity detection**

En este apartado se detecta si existe multicolinearidad entre las variables independientes, esto ocurre cuando dos o más variables independientes tienen una alta correlación entre sí mismas, esto puedo causar una estimación poco fiable.

Para la detección de la multicolinearidad la técnica **Variance Inflaction Factor (VIF)** fue utilizada. Este método hace una regresión de cada variable independiente contra todas las demás.

---

## **Transformations**

Dados los resultados de los apartados anteriores, se implementan soluciones a los problemas detectados para que el modelo sea el más adecuado.

---

## **Model | OLS derivation**

En este apartado se estima y se propone un modelo de regresión múltiple. Se utiliza álgebra lineal para la estimación de los coeficientes y de sus errores estándar del modelo de regresión.
