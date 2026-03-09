Análisis de Evasión de Clientes - Telecom 

Propósito del análisis:
El objetivo de este proyecto es identificar los factores críticos que impulsan la evasión de clientes en una empresa de telecomunicaciones. Mediante un análisis descriptivo y exploratorio (EDA), se buscan patrones que permitan predecir qué perfiles tienen mayor riesgo de abandonar el servicio, permitiendo a la empresa implementar estrategias de retención proactivas.

Estructura del proyecto y organización:
Para mantener la modularidad y las mejores prácticas, el proyecto se organiza de la siguiente manera:
data/: Contiene el dataset original en formato JSON obtenido de la API de Alura/Telecom.
notebooks/: Archivo .ipynb con el proceso completo dividido en capas (Extracción, Limpieza, EDA y Conclusiones).
images/: Capturas de pantalla de las visualizaciones clave generadas durante el análisis.
README.md: Documentación actual del proyecto.

Ejemplos de gráficos e insights obtenidos
Tras procesar 7,043 registros válidos, se rescataron los siguientes hallazgos:
Tasa Global de Evasión: El 26.5% de los clientes se ha dado de baja.
Impacto del Contrato: Los clientes con contrato mes a mes tienen una tasa de fuga superior al 40%, mientras que los contratos a dos años son los más estables (~3%).
Fricción Financiera: El método de cheque electrónico presenta un riesgo de evasión del 44%.
Sensibilidad al Precio: Existe una mayor densidad de abandono en clientes con cargos mensuales altos, específicamente entre $70 y $100.

Instrucciones para ejecutar el notebook
Para replicar este análisis en tu entorno local o en Google Colab:
Clonar el repositorio:git clone (https://github.com/roizunza/AnalisisdataTelecomX)
Instalar dependencias: Asegúrate de tener instaladas las librerías pandas, seaborn y matplotlib.
Cargar los datos: Sube el archivo JSON a la carpeta raíz o conéctalo directamente a la API.
Ejecución: Corre las celdas de forma secuencial. Se recomienda poner especial atención a la Capa de Transformación Robusta para asegurar el correcto mapeo de las columnas financieras.
