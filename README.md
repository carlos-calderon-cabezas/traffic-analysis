# Análisis y Predicciones de Datos de Tráfico Vehicular

![image](https://github.com/user-attachments/assets/45336690-769a-4dec-a385-a87ede89dd79)

## Tabla de Contenidos

- [Descripción del proyecto](#descripción-del-proyecto)
- [Contenido del proyecto](#contenido-del-proyecto)
- [Instrucciones de uso](#instrucciones-de-uso)
- [Breve resumen de conclusiones y recomendaciones](#breve-resumen-de-conclusiones-y-recomendaciones)

## Descripción del proyecto

El presente proyecto es una demostración breve y sencilla del análisis de datos y las predicciones de tráfico vehicular que yo realizaba para una empresa importante en Ecuador, dedicada a los estudios, planificación y construcción de proyectos de infraestructura vial. En este caso concreto, se trataba de la ampliación de una carretera.

Dadas las políticas de confidencialidad de la empresa en cuanto a los datos del proyecto, no me es posible incluir el total de parámetros obtenidos por este sensor, ni todas las variables que formaron parte del estudio, ni proporcionar la ubicación exacta del mismo. Asimismo, se han modificado intencionalmente parte de los datos que se muestran aquí.

Este proyecto se realiza con datos obtenidos de mediciones de tráfico vehicular realizadas entre el 2 de agosto de 2021 y el 12 de octubre de 2021, en un total de 71 días continuos.

Para realizar el proyecto, se colocó un sensor de tráfico en un tramo estratégico de la vía, el cual era capaz de contar los vehículos que pasaban y detectar características tales como el tipo de vehículo, su velocidad, así como la fecha y hora en que circulaban. En el dataset correspondiente al sensor o medidor de tráfico (*sensor_df*), cada fila representa la cantidad por hora de vehículos que han circulado por cada tipo, su velocidad promedio y su velocidad en el percentil 85.

Adicionalmente, se tiene un conjunto de datos correspondiente al estado del clima en el momento en que se tomaron los datos del tráfico. Estos datos también fueron registrados durante cada una de las 24 horas de cada uno de los 71 días de mediciones de tráfico. Se pueden obtener datos climáticos históricos de diferentes partes del mundo en [Visual Crossing](https://www.visualcrossing.com/weather/weather-data-services).

En el proyecto se analizan datos como, por ejemplo, la cantidad de vehículos que pasan a determinada hora o los días de la semana con más vehículos de un cierto tipo, etc.

En el análisis predictivo de este proyecto, se estudia el comportamiento del flujo vehicular influenciado por el día de la semana, la hora y el estado del clima actual.

## Contenido del proyecto

- `Traffic_analysis.ipynb`: Jupyter Notebook de Google Colab escrito en Python.
- Carpeta `input` con los siguientes datasets de entrada:
   - Dataset `norte_sur_df.csv` con mediciones tráfico vehicular realizadas con sensor de tráfico *MetroCount RoadPod VT*.
   - Dataset `weather_df.csv` con datos históricos de clima tomados durante el tiempo de medición de tráfico.


## Instrucciones de uso

Para utilizar este proyecto es necesario seguir estos pasos:

1. Clonar el repositorio o descargar todos los archivos.
2. Asegurarse de tener instaladas las dependencias necesarias, como Jupyter Notebook y las bibliotecas de Python utilizada en los notebooks, incluyendo *pandas*, *matplotlib* y *seaborn*.
3. Abrir el archivo `Traffic_analysis.ipynb` en Jupyter Notebook o JupyterLab.
4. Ejecutar las celdas del notebook para ver los análisis y predicciones.

No es necesario instalar software adicional ni configurar el entorno más allá de tener Jupyter y las librerías de Python previamente descritas.

## Breve resumen de conclusiones y recomendaciones

- Se realizó un histograma para analizar la velocidad promedio, y se vio que la gran mayoría de vehículos circulan a velocidades entre 65 y 75 kilómetros por hora, dado que al estar el sensor de tráfico en una zona urbana y el límite de velocidad es de 50 km/h, se recomienda colocar dispositivos rompevelocidades en el centro del poblado, así como solicitar a la autoridad de tránsito competente la colocación de un radar de velocidad para infraccionar a los conductores que no respeten el límite.
- Se pudo observar que existe un volumen considerable de tránsito pesado que circula por las madrugadas, especialmente entre 11 de la noche y 3 de la mañana, por lo cual se recomienda solicitar a la autoridad de tránsito competente mantener el semáforo encendido y activo durante las 24 horas del día, debido a que entre 12 y 5 de la mañana, este se apaga. Esto va a majorar la seguridad, especialmente de peatones y vehículos que cruzan por las calles transversales y podrá reducir el número de accidentes.
- Se realizó un breve estudio de la posible recaudación de la nueva estación de peaje que la consecionaria planea construir, y dada la fuerte afluencia de vehículos pesados y la tarifa elevada que estos deben pagar, se estima un recaudación mensual de USD 320.000 al mes, por lo cual con lo recuadado, se recomienda a la consecionaria mantener en óptimas condiciones tanto la superficie asfáltica, así como la señalética vial para incentivar a los conductores que tomen esa vía y no rutas alternas.
- Se realizó un análisis predictivo de la flota vehícular para predecir el tráfico máximo que puede llegar a tener en los próximos 30 años, analizando varias variables adicionales, incluyendo índices económicos del país, el crecimiento del parque automotor, entre otras variables, y se estima un flujo vehicular solo en tránsito pesado de aproximadamente 15.000 vehículos pesados en el día después de 30 años. Sin embargo por motivos de confidencialidad del proyecto, no se permite mostrar todos los detalles del estudio realizado.
  - Este modelo predictivo permitió recomendar a la consecionaria ampliar la carretera existente que es de 1 carril por sentido, hasta 3 carriles por sentido de circulación, así como cumplir con ciertos parámetros para la compra de materiales, maquinaria, la cantidad de excavaciones que deben realizarse por tramo y las técnicas de construcción que se deben emplear.
