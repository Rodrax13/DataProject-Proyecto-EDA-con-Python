# 📊 DataProject: Proyecto EDA con Python

## 📌 Objetivo del proyecto
Mi objetivo en este proyecto ha sido realizar un Análisis Exploratorio de Datos (EDA) exhaustivo sobre campañas de marketing telefónico de una institución bancaria. 

A través de Python, he buscado limpiar, transformar y visualizar los datos con un enfoque analítico crítico, desmintiendo supuestos previos y encontrando los patrones de comportamiento que dictan por qué un cliente suscribe el producto.

---

## 📁 Estructura del repositorio

Proyecto4_DataProject-Proyecto-EDA-con-Python
├── data/
│   ├── raw/
│   │   ├── bank-additional.csv
│   │   └── customer-details.xlsx
│   └── processed/
│       ├── bank_clean.csv
│       ├── customers_clean.csv
│       ├── df_final_clean.csv
│
├── notebooks/
│   ├── DataProject_ Proyecto EDA con Python V2.ipynb
│
└── README.md

 


🧹 Proceso de limpieza y transformación

Para garantizar la fiabilidad de mi análisis, ejecuté el siguiente flujo de preparación:

Imputación lógica: Utilicé medianas y medias para las variables numéricas, y modas para rescatar los nulos de variables binarias sin alterar su peso estadístico.

Conversión de tipos: Limpié cadenas de texto numéricas (comas por puntos) y optimicé el consumo de memoria convirtiendo textos a tipos categóricos.

Tratamiento temporal: Transformé los meses en español a fechas válidas (datetime) para extraer mes y día laborable.

Cruce (Merge): Fusioné eficientemente los datos de campaña del banco con los datos financieros del cliente usando sus ID únicos.




📈 Análisis de Resultados e Insights Obtenidos

Tras analizar los gráficos y métricas, he extraído los siguientes hallazgos de negocio:

✔️ Alta ineficiencia global: El dataset presenta un fuerte desbalanceo (~11% de conversión). La estrategia actual de llamadas masivas en frío es ineficiente y quema recursos.

✔️ El mito de los ingresos: Al cruzar la edad con los ingresos anuales, he demostrado que el nivel salarial no es un factor discriminante. El producto es contratado por perfiles de todos los rangos de ingresos.

✔️ El perfil demográfico óptimo: El banco concentra sus llamadas en personas de 30 a 45 años con baja conversión. Sin embargo, los jubilados (mayores de 60) y estudiantes tienen una predisposición a contratar el depósito excepcionalmente más alta.

✔️ El peso del éxito previo: Los clientes que ya aceptaron una oferta en el pasado (poutcome = SUCCESS) son el segmento más seguro y deben ser la prioridad absoluta.

✔️ Optimización de Estacionalidad: El mes de mayo concentra el mayor volumen de llamadas de todo el año, pero tiene la peor tasa de conversión. Redistribuir las campañas hacia el verano (junio, julio, agosto) y la recta final/inicio de año (octubre a enero) dispara la eficiencia. Además, he comprobado que el día de la semana es totalmente irrelevante.




🛠️ Herramientas utilizadas

Python (Pandas, NumPy) para manipulación y limpieza de datos.

Matplotlib y Seaborn para visualización avanzada (gráficos de doble eje, segmentación, eliminación de outliers).

Jupyter Notebooks / VS Code para el entorno de desarrollo y presentación.




📌 Conclusión General y Siguientes Pasos

Este análisis me ha permitido demostrar que el éxito de la campaña no reside en llamar masivamente durante todo el año a los perfiles más abundantes (30-45 años), ni depende fuertemente de los ingresos del cliente.

La clave del éxito reside en cambiar hacia un modelo de calidad vs. cantidad: priorizar a aquellos con éxito en campañas pasadas, aprovechar perfiles receptivos (jubilados/estudiantes) y redistribuir el esfuerzo comercial a los meses de mayor conversión. Como siguientes pasos, sugiero analizar el umbral de "fatiga comercial" (límite de llamadas por cliente) y alinear los lanzamientos con momentos macroeconómicos favorables.