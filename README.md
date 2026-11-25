# sprint7-final-project
ConnectaTel - Análisis Exploratorio y Segmentación de Clientes
Objetivo del Proyecto
El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel utilizando datos de usuarios, planes y registros de uso. A través de un proceso de exploración, limpieza y análisis de datos, se busca identificar patrones de consumo, segmentar clientes y generar recomendaciones de negocio que permitan optimizar la oferta comercial de la compañía.

Datasets Utilizados
users_latam.csv
Contiene información demográfica y contractual de los clientes:

user_id
first_name
last_name
age
city
reg_date
plan
churn_date
plans.csv
Contiene información sobre los planes disponibles:

plan_name
messages_included
gb_per_month
minutes_included
usd_monthly_pay
usd_per_gb
usd_per_message
usd_per_minute
usage.csv
Contiene los registros de uso de los clientes:

id
user_id
type
date
duration
length
Etapas del Análisis Realizadas
1. Exploración Inicial
Revisión de la estructura de los datasets.
Identificación de dimensiones y tipos de datos.
Inspección de registros iniciales.
2. Calidad de Datos
Detección de valores nulos.
Identificación de valores inválidos y centinela.
Revisión de fechas fuera de rango.
Evaluación de consistencia de los registros.
3. Limpieza de Datos
Reemplazo del valor centinela -999 en age.
Conversión de "?" en city a valores nulos.
Corrección de fechas fuera de rango.
Validación de valores faltantes asociados al tipo de registro.
4. Construcción de Perfiles de Usuario
Cálculo de llamadas realizadas.
Cálculo de mensajes enviados.
Cálculo de minutos consumidos.
Integración de los resultados con la información de usuarios.
5. Análisis Exploratorio
Estadística descriptiva.
Histogramas.
Distribuciones de uso.
Comparación entre planes.
6. Detección de Outliers
Visualización mediante boxplots.
Aplicación del método IQR.
Evaluación de usuarios con uso intensivo.
7. Segmentación de Clientes
Segmentación por grupos etarios.
Segmentación por nivel de uso.
Identificación de oportunidades comerciales.
8. Análisis Ejecutivo
Interpretación de resultados.
Implicancias para el negocio.
Recomendaciones comerciales.
Cómo Ejecutar el Notebook
Opción 1: Google Colab
Abrir Google Colab.
Seleccionar Archivo → Subir notebook.
Cargar el archivo:
S7 Version-Estudiante-Project-ConnectaTel.ipynb
Cargar los datasets requeridos.
Ejecutar las celdas de forma secuencial.
Opción 2: Jupyter Notebook
Instalar Python.
Instalar Jupyter Notebook.
Abrir una terminal en la carpeta del proyecto.
Ejecutar:
jupyter notebook
Abrir el notebook del proyecto.
Ejecutar todas las celdas en orden.
Guía de Reproducción
Para reproducir los resultados del análisis:

Descargar el notebook del proyecto.
Disponer de los archivos:
users_latam.csv
plans.csv
usage.csv
Abrir el notebook en Google Colab o Jupyter Notebook.
Verificar que las rutas de los datasets sean correctas.
Ejecutar todas las celdas desde el inicio hasta el final.
Revisar las tablas, gráficos, segmentaciones y conclusiones generadas automáticamente.
Principales Hallazgos
Se detectaron y corrigieron problemas de calidad de datos.
La mayoría de los clientes pertenece al segmento Adulto.
El 73,58% de los usuarios presenta un nivel de uso medio.
Se identificaron usuarios con consumos significativamente superiores al promedio.
Los clientes de alto uso representan oportunidades para estrategias de fidelización y planes premium.
La segmentación de clientes permite diseñar ofertas más adaptadas a distintos perfiles de consumo.
Autor
Proyecto desarrollado como parte del Sprint 7 de análisis de datos aplicados a ConnectaTel.
