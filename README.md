# sprint7-final-project
Proyecto de Practica Telecom

## :high_brightness: OBJETIVO
En esta práctica, tuvimos la oportunidad de compilar datos relacionados con el comportamiento de clientes de una empresa de telecomunicaciones. Aquí pudimos visualizar diferentes tipos de parámetros como son
la cantidad de llamdas, mensajes que se estan registrando, o bien el total de minutos que los usuarios estan registrando por llamadas. Asimismo, nos dimos a la tarea de realizar este análisis por sectores,
diferenciando entre diversos rangos de edades y uso que se le dan a dichos servicios.

## :hammer: DATASETS UTILIZADOS
Utilizamos 3 tipos de datasets:

## :ballot_box_with_check: plans.csv - Información de planes: Basicamente nos ayuda a enteder los servicios que ofrece la empresa, es decir, los tipos de planes y GB disponibles.

## :white_check_mark: users_latam.csv - Información de clientes: Datos de los usuarios registrados para el uso de este servicio. 
Contiene datos personales los cuales nos van a ayudar a segmentar por diferentes tipos de valores (edad, ciudad, fecha de registro, plan contratado)

## :ballot_box_with_check: usage.csv - Actividad real de uso: Como se estan utilizando los servicios. Es decir, el comportamiento de los usuarios relacionados con la duración de llamdas o la cantidad de mensajes. 

## :grey_exclamation: ETAPAS DE ANALISIS

## :white_circle: Cargar y Explorar: Se importaron los datasets y se exploraron las estructuras con .head(), .shape, .info()

## :white_circle: Identificación de problemas de calidad: Se revisaron rangos de fechas y se detectaron valores inválidos y nulos con .isna().sum() y .isna().mean()

## :white_circle: Limpieza basica de datos: Se reemplazo y corrigio información la cual, no era posible (eg. fechas imposibles)

## :white_circle: Resumen por usuario: Se crearon metricas por usuario mediante el uso de los datos sobre cantidad de mensajes, llamadas y llamadas por minutos, se utilizó pd.merge(), yo generé el data df_merged

## :white_circle: Visualización de distribuciones y outliers: Se realizó la creación de histogramas para entender distribuciones, se identificaron outliers mediante boxplots y se analizaron patrones por tipo de plan

## :white_circle: Segmentación de clientes: Se realizaron gráficas para visualizar segmentos, para esto se crearon dos grupos: grupo_uso y grupo_edad

## :white_circle: Insight Ejecutivo: Al final respondimos diversas preguntas sobre el análisis de dicha información así como realizar diversas recomendaciones. También pudimos percatarnos que se podría realizar una análisis de esa información de manera aún mas específica.

\## 📁 EJECUCIÓN DEL NOTEBOOK
Podemos ejecutar ese ejercicio abriendolo directamente en una página de GitHub para poder visualizarlo.

## :lollipop: Google Colab
Ve a colab.research.google.com
Haz clic en "Archivo" → "Abrir notebook"
Selecciona "Subir" y carga tu archivo .ipynb
Los datasets deberán estar en la carpeta /datasets/ o puedes subirlos manualmente

## :cherries: Jupyter Notebook local
Instala Python y Jupyter en tu computadora
Abre terminal/cmd y ejecuta: jupyter notebook
Navega hasta tu archivo y ábrelo
Asegúrate de tener los datasets en la ruta correcta
