# Desafio_Telecom_parte_1
Proyecto Telecom Parte 1
[README.md](https://github.com/user-attachments/files/25726510/README.md)
<h1>#Desafio Telecom Parte I</h1>
<br>
<p align="center"> <img width="500" height="500" alt="Insignia" src="https://github.com/user-attachments/assets/7193eb23-518a-4507-accb-cddbfe9ea70b" /> </p>
<br>
<h2>🚀 Instrucciones para ejecutar el Notebook</h2>
<p>Para ejecutar este notebook en Google Colab, sigue los siguientes pasos: </p>
<p>1. Abre Google Colab en tu navegador web. </p>
<p>2. Haz click en "Subir" > luego en "explorar" > y selecciona el archivo.ipynb de este proyecto desde tu computadora. </p>
<p>3. Una vez que el Notebook esté abierto en Colab, ejecuta las celdas del Notebook secuencialmente. Si quieres ejecutar todo de una vez, puedes hacerlo en la opción "Ejecutar todas".</p>
<br>
<h2>🚨 Aviso</h2>
<p>La solución de este Notebook la encuentras en el archivo: HCG_Telecom_Parte_1.ipynb</p>
<br>
<h2>📖 Descripción</h2>
<h4>Churn de Clientes</h4>
<p>La empresa Telecom X enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes. El desafío será recopilar, procesar y analizar los datos, utilizando Python y sus principales bibliotecas para extraer información.</p>
<br>
<p>¿Qué se practicará?</p>
<p>1. Importación y manipulación de datos desde una API de manera eficiente. </p>
<p>2. Aplicar los conceptos de ETL (Extracción, Transformación y Carga) en la preparación de los datos. </p>
<p>3. Crear visualizaciones estratégicas para identificar patrones y tendencias. </p>
<p>Realizar un Análisis Exploratorio de Datos (EDA) y generar un informe con insights relevantes.</p>
<br>
<h2>🎯 Objetivos del challenge</h2>
<h3>📌 1. Extracción (E - Extract)</h3>
<h4>Extracción de datos</h4>
<p>Para iniciar el análisis, necesitamos importar los datos de la API de Telecom X. Estos datos están disponibles en formato JSON y contienen información esencial sobre los clientes, incluyendo datos demográficos, tipo de servicio contratado y estado de evasión.</p>
<p>Enlace de la API: https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/refs/heads/main/TelecomX_Data.json</p>
<p>¿Qué hay que hacer? </p>
<p>-Cargar los datos directamente desde la API utilizando Python. </p>
<p>-Convertir los datos a un DataFrame de Pandas para facilitar su manipulación. </p>
<h3>🔧 2. Transformación  (T - Transform)</h3>
<h4>Conoce el conjunto de datos</h4>
<p>Tenemos que comprender la estructura del dataset y el significado de sus columnas. Esta etapa nos ayuda a identificar qué variables son más relevantes para el análisis de evasión de clientes.</p>
<p>¿Qué hay que hacer? </p>

<p>Explorar las columnas del dataset y verificar sus tipos de datos. </p>
<p>Efectuar un diccionario para comprender mejor el significado de las variables. </p>
<h4>Comprobación de incoherencias en los datos</h4>
<p>Verificar si hay problemas en los datos que puedan afectar el análisis. Hay que prestar atención a valores ausentes, duplicados, errores de formato e inconsistencias en las categorías. Este proceso es esencial para asegurar que los datos estén listos para las siguientes etapas.</p>
<h4>Manejo de inconsistencias</h4>
<p>Al identificar las inconsistencias, aplicamos las correcciones necesarias. Ajustamos los datos para asegurarnos de que estén completos y coherentes, preparándolos para las siguientes etapas del análisis.</p>
<h4>Columna de cuentas diarias</h4>
<p>Crea la columna "cuentas_diarias". Utiliza la facturación mensual para calcular el valor diario, proporcionando una visión más detallada del comportamiento de los clientes a lo largo del tiempo.</p>
<h4>Estandarización y transformación de datos</h4>
<p>Traduce o renombra columnas y datos para que la información sea más accesible y fácil de entender , puede mejorar significativamente la claridad y comunicación de los resultados, facilitando la interpretación y evitando confusiones.</p>
<p>La estandarización y transformación de datos es altamente recomendada, ya que busca hacer que la información sea más consistente, comprensible y adecuada para el análisis. Por ejemplo, puedes convertir valores textuales como "Sí" y "No" en valores binarios (1 y 0), lo que facilita el procesamiento matemático y la aplicación de modelos analíticos.</p>
<h3>📊 3. Carga y análisis (L - Load & Analysis)</h3>
<h4>Análisis Descriptivo</h4>
<p>Realizar un análisis descriptivo de los datos, calculando métricas como media, mediana, desviación estándar y otras medidas que ayuden a comprender mejor la distribución y el comportamiento de los clientes.</p>
<h4>Distribución de evasión</h4>
<p>El objetivo es comprender cómo está distribuida la variable "churn" (evasión) entre los clientes. Utiliza gráficos para visualizar la proporción de clientes que permanecieron y los que se dieron de baja. </p>
<h4>Recuento de evasión por variables categóricas</h4>
<p>Exploraremos cómo se distribuye la evasión según variables categóricas, como género, tipo de contrato, método de pago, entre otras.</p>
<p>Este análisis puede revelar patrones interesantes, por ejemplo, si los clientes de ciertos perfiles tienen una mayor tendencia a cancelar el servicio, lo que ayudará a orientar acciones estratégicas.</p>
<h4>Conteo de evasión por variables numéricas</h4>
<p>Exploraremos cómo las variables numéricas, como "total gastado" o "tiempo de contrato", se distribuyen entre los clientes que cancelaron (evasión) y los que no cancelaron. </p>
<p>Este análisis ayuda a entender si ciertos valores numéricos están más asociados con la evasión, proporcionando insights sobre los factores que influyen en el comportamiento de los clientes.</p>
<h4>Análisis de correlación entre variables</h4>
<p>Exploraremos la correlación entre diferentes variables del dataset. Esto puede ayudar a identificar qué factores tienen mayor relación con la evasión de clientes, como:</p>
<p>-La relación entre la cuenta diaria y la evasión.
<p>-Cómo la cantidad de servicios contratados afecta la probabilidad de churn.</p>
<p>Esto puede proporcionar insights valiosos para la creación de modelos predictivos más robustos.</p>
<br>
<h2>⚙️ Entorno de desarrollo</h2>
<p>Google Colab.</p>
<br>
<h2>🧠 Tecnologias utilizadas</h2>
<p>-Python.</p>
<br>
<h2>📘 Librerías utilizadas</h2>
<p>-Pandas.</p>
<p>-Matplotlib.</p>
<p>-Plotly.</p>
<p>-Seaborn.</p>
