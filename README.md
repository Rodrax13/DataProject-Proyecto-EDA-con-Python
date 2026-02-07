📊 DataProject_ Proyecto EDA con Python
📌 Objetivo del proyecto
El objetivo de este proyecto es realizar un Análisis Exploratorio de Datos (EDA) sobre campañas de marketing directo de una institución bancaria portuguesa, utilizando Python y librerías de análisis de datos.
Se busca:
•	Limpiar y transformar los datos
•	Analizar estadísticamente las variables
•	Visualizar patrones relevantes
•	Extraer conclusiones basadas en datos reales
________________________________________
📁 Estructura del repositorio
├── data/
│   ├── raw/
│   │   ├── bank-additional.csv
│   │   └── customer-details.xlsx
│   └── processed/
│       ├── bank_clean.csv
│       └── customers_clean.csv
│
├── notebooks/
│   ├── DataProject_ Proyecto EDA con Python.ipynb
│
└── README.md
________________________________________
📊 Conjuntos de datos utilizados
📄 bank-additional.csv
Contiene información sobre campañas de marketing bancario:
•	Edad, profesión, educación, estado civil
•	Historial financiero (préstamos, impagos)
•	Información de campaña (duración llamada, número de contactos)
•	Variables económicas
•	Variable objetivo: y (suscripción al producto)
________________________________________
📄 customer-details.xlsx
Información demográfica y comportamiento de clientes:
•	Ingresos anuales
•	Hijos en el hogar
•	Antigüedad como cliente
•	Visitas mensuales a la web
Las hojas fueron unificadas en un único dataset.
________________________________________
🧹 Proceso de limpieza y transformación
Se realizaron las siguientes acciones:
•	Eliminación o imputación de valores nulos
•	Conversión de columnas a tipos adecuados (numéricos y fechas)
•	Normalización de variables categóricas
•	Unión de datasets de Excel mediante pd.concat()
•	Creación de datasets limpios para análisis posterior
Resultado: datos consistentes y listos para análisis.
________________________________________
📈 Análisis exploratorio realizado
🔍 Estadística descriptiva
•	Medias, medianas, desviaciones estándar
•	Distribución de variables numéricas
•	Frecuencias de variables categóricas
•	Análisis de correlaciones
________________________________________
📊 Visualizaciones principales
•	Distribución de clientes que suscriben el producto
•	Edad vs conversión
•	Duración de llamadas vs resultado
•	Heatmap de correlaciones
•	Conversión por tipo de trabajo
•	Distribución de ingresos de clientes
________________________________________
🧠 Principales conclusiones
✔ La mayoría de los clientes no suscriben el producto (dataset desbalanceado)
✔ La duración de la llamada es el factor más influyente en la conversión: llamadas más largas presentan tasas mucho mayores de éxito
✔ Clientes de mayor edad tienden a aceptar más el producto
✔ Algunos perfiles laborales muestran mejores resultados de campaña
✔ Un número excesivo de contactos en la campaña se relaciona con menor probabilidad de conversión
✔ Variables económicas presentan relación con el comportamiento de los clientes
________________________________________
🛠️ Herramientas utilizadas
•	Python
•	Pandas
•	NumPy
•	Matplotlib
•	Seaborn
•	Visual Studio Code
________________________________________
📌 Conclusión general
El análisis exploratorio permitió comprender los factores que influyen en el éxito de las campañas de marketing bancario.
La duración del contacto y ciertos perfiles de clientes son claves para mejorar la efectividad de futuras campañas.
Este proyecto demuestra el uso de Python para:
•	Limpieza de datos
•	Análisis estadístico
•	Visualización de información
•	Extracción de insights de negocio

