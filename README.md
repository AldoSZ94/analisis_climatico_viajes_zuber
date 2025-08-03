# 🚖 Proyecto: Análisis de Viajes en Taxi y Condiciones Climáticas en Chicago

Este es mi proyecto correspondiente al **Sprint N.º 8** dentro de mi formación como **Analista de Datos Jr. en TripleTen**.  
En este análisis trabajé para **Zuber**, una empresa emergente de viajes compartidos en Chicago, con el objetivo de encontrar patrones clave en los viajes en taxi, las preferencias de los pasajeros y el impacto del clima en la duración de los recorridos.

---

## 🔎 Objetivos principales

- Explorar y analizar datos históricos de viajes en taxi en Chicago.
- Comparar el desempeño de distintas empresas de taxis.
- Evaluar la popularidad de los barrios como destinos.
- Visualizar los barrios más visitados y las empresas con más viajes.
- Probar una hipótesis sobre el efecto de la lluvia en la duración de los viajes los sábados.

---

## 🛠️ Etapas del proyecto

1. **Conexión a base de datos y análisis con SQL**  
   Se consultaron y analizaron datos de cuatro tablas principales (`neighborhoods`, `cabs`, `trips` y `weather_records`) para obtener:
   - Número de viajes por empresa en fechas específicas.
   - Empresas con más actividad en la primera semana de noviembre.
   - Compañías líderes (Flash Cab y Taxi Affiliation Services) frente a otras.
   - Identificación del clima ("Good" o "Bad") por hora para evaluar su impacto.

2. **Análisis en Python**  
   Con archivos exportados de SQL:
   - Se graficaron las empresas con más viajes el 15 y 16 de noviembre.
   - Se analizaron los barrios con mayor cantidad de llegadas de taxis.
   - Se aseguraron los tipos de datos correctos y se realizaron análisis visuales con `matplotlib` y `seaborn`.

3. **Prueba de hipótesis**  
   Se comprobó la hipótesis:
   > *“La duración promedio de los viajes desde el Loop hasta el Aeropuerto Internacional O'Hare cambia los sábados lluviosos.”*

   - Se formularon hipótesis nula y alternativa.
   - Se aplicó una prueba estadística adecuada (`Mann-Whitney U`) con un nivel de significancia definido.
   - Se interpretaron los resultados y se elaboraron conclusiones basadas en evidencia.

---

## 📂 Datasets utilizados

Los datos analizados incluyen:

- `sprint8.ipynb` — notebook con el análisis completo en Python  
- `project_sql_result_01.csv` — viajes por empresa de taxis el 15 y 16 de noviembre  
- `project_sql_result_04.csv` — barrios con mayor número de llegadas  
- `project_sql_result_07.csv` — viajes desde el Loop a O'Hare los sábados, con condiciones climáticas  

---

## 📈 Herramientas y tecnologías

- **SQL** para extracción y limpieza inicial desde la base de datos.
- **Python** para análisis estadístico y visualización.
- Librerías: `pandas`, `matplotlib`, `seaborn`, `scipy`.

---
