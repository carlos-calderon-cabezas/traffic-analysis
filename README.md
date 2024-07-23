# Análisis y Predicciones de Datos de Tráfico Vehicular

El presente proyecto es una demostración breve y sencilla del análisis de datos y las predicciones de tráfico vehicular que yo realizaba para una empresa importante en Ecuador, dedicada a los estudios, planificación y construcción de proyectos de infraestructura vial. En este caso concreto, se trataba de la ampliación de una carretera.

Dadas las políticas de confidencialidad de la empresa en cuanto a los datos del proyecto, no me es posible incluir el total de parámetros obtenidos por este sensor, ni todas las variables que formaron parte del estudio, ni proporcionar la ubicación exacta del mismo. Asimismo, se han modificado intencionalmente parte de los datos que se muestran aquí.

Este proyecto se realiza con datos obtenidos de mediciones de tráfico vehicular realizadas entre el 2 de agosto de 2021 y el 12 de octubre de 2021, en un total de 71 días continuos.

Para realizar el proyecto, se colocó un sensor de tráfico en un tramo estratégico de la vía, el cual era capaz de contar los vehículos que pasaban y detectar características tales como el tipo de vehículo, su velocidad, así como la fecha y hora en que circulaban. En el dataset correspondiente al sensor o medidor de tráfico (*sensor_df*), cada fila representa la cantidad por hora de vehículos que han circulado por cada tipo, su velocidad promedio y su velocidad en el percentil 85.

Adicionalmente, se tiene un conjunto de datos correspondiente al estado del clima en el momento en que se tomaron los datos del tráfico. Estos datos también fueron registrados durante cada una de las 24 horas de cada uno de los 71 días de mediciones de tráfico. Se pueden obtener datos climáticos históricos de diferentes partes del mundo en [Visual Crossing](https://www.visualcrossing.com/weather/weather-data-services).

En el proyecto se analizan datos como, por ejemplo, la cantidad de vehículos que pasan a determinada hora o los días de la semana con más vehículos de un cierto tipo, etc.

En el análisis predictivo de este proyecto, se estudia el comportamiento del flujo vehicular influenciado por el día de la semana, la hora y el estado del clima actual.
