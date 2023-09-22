# Modelos-de-Clasificacion
CÓdigo python para limpieza y preparación de Dataset y evaluación de modelos de clasificación


ALGORITMO DE PREPARACIÓN DATASET Y MODELOS DE CLASIFICACIÓN SOBRE DATA DE REIGRESO HOSPITALARIO EN PACIENTES CON DIABETES

El proyecto considera algoritmo para análisis previo, limpieza y preparación de Dataset compartido "diabetic_data", 
aplicando herramientas de Machine Learning, mediante programación en python.

OBJETIVO: Predecir si un paciente con diabetes va a ser readmitido aun hospital en función de ciertos atributos.


DESCRIPCIÓN DATASET:

Para llevar a cabo este trabajo, se utiliza un conjunto de datos disponible públicamente en la web (www.kaggle.com). 
Este conjunto de datos representa 10 años (1999-2008) de atención clínica en 130 hospitales de EE. UU. y contiene 
101.766 observaciones durante 10 años. Incluye más de 50 atributos, que representan características del paciente,
diagnósticos, exámenes, etc. La información se extrajo de la base de datos que contenía registros que cumplían con los 
siguientes criterios.

1) Cada servicio representa una estancia hospitalaria.
2) Sólo incluye la atención a pacientes diabéticos, es decir, aquellos en los que se introdujo al sistema como diagnóstico 
   algún tipo de diabetes.
3) La duración de la estancia fue de mínimo 1 día y máximo de 14 días.
4) Se realizaron pruebas de laboratorio durante el servicio.
5) Se administraron medicamentos durante el servicio.

Los datos contienen atributos como número de paciente, raza, sexo, edad, tipo de hospitalización, tiempo de estancia en el 
hospital, número de pruebas de laboratorio realizadas, resultados de la prueba HbA1c, diagnósticos, cantidad de medicamentos 
utilizados, si utiliza medicamentos para la diabetes y cuáles, número de visitas ambulatorias, hospitalarias y de urgencias 
en el año previo a la hospitalización, etc. Algunos de estos atributos no serán tenidos en cuenta en este análisis ya que no 
serán relevantes para el objetivo del trabajo.


DESCRIPCIÓN ALGORITMO:

En primera instancia se realiza lectura de Dataset junto a un análisis previo de interpretación de variables. Posteriormente se renombran variables y se efectúa un análisis descriptivo de los datos. Se identifican anomalías y se procede a eliminar datos nulos, simbología inadecuada, datos faltantes y otros. 
Una vez limpio y estructurado el Dataset, se procede a codificar variables discretas mediante números, para preparar datos antes de entrenar los modelos, y realizar visualizaciones previas como histogramas y matriz de correlación.
Posterior al análisis exploratorio, se efectúa una separación de los datos en conjuntos de entrenamiento y test en una proporciòn 70-30. Luego se entrenan los 4 siguientes modelos:
- Decisión tree
- Random forest
- Gaussian Naive Bayes
- K-Nearest-Neighbor

Con el conjunto de test se procede a calcular métricas como "Recall", "Accuracy", "Precision", entre otras, para poder comparar la efectividad entre los modelos.

Dado los resultados comparativos obtenidos, se procede a balancear los datos mediante técnicas de Oversampling, para mejorar los resultados anteriores. Una vez realizado, se vuelve a entrenar y evaluar los modelos anteriores. Finalmente es posible apreciar que el mejor modelo de aquellos evaluados, corresponde a "Random Forest".


PROPÓSITO:
El proyecto resulta útil para conocer básicamente metodología típica de desarrollo de proyectos de Data Science, considerando etapas de análisis exploratorio previo, limpieza de Dataset, preparación de datos y conjuntos, entrenamiento de modelos, evaluación y comparación de resultados.


REQUERIMIENTOS:
Entorno de desarrollo en Python. (se recomienda Google Colab, ya que no requiere instalación ni uso de recursos).
Librerias Python (Pandas, Numpy, Matplotlib, Seaborn, Sklearn).


PRIMEROS PASOS:
Lenguaje de programación Python nivel intermedio (para comprender uso de librerías y proceso tras código).
Metodología de proyectos Data Science.


UTILIZACIÓN:
Para poder emplear el código y realizar la revisión de todo el algoritmo, se recomienda seguir los siguientes pasos:
a. Descargar material (archivo código y Dataset) desde el repositorio (https://github.com/JorgeIgnadv/Modelos-de-Clasificacion/edit/main/).
b. Abrir Google Colab desde el navegador
c. Crear nuevo archivo de trabajo y cargar archivo de código ("Project"), descargado del repositorio previamente.
d. Cargar Dataset ("diabetic_data"), descargado del repositorio previamente.
e. Ejecutar en orden los códigos que se encuentran en el archivo cargado.
f. Frente a dudas o consultas, favor escribir a información de contacto.

TRABAJO FUTURO:
Aplicación de metodologías de eliminación o reducción de parámetros mediante PCA.
Aplicación de otros modelos de clasificación como Support Vector Machine o redes neuronales.
Aplicación de herramientas de balance de conjuntos como Undersampling, u otros.


CONTACTO
JORGE_IGNACIO_DV@HOTMAIL.COM
