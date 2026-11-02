# Proceso analítico

El trabajo organizó su desarrollo con CRISP-DM, desde la comprensión del problema comercial hasta la interpretación de los resultados de modelado.

## Comprensión y preparación

Se revisó la información histórica de ventas disponible para identificar variables útiles y evaluar su calidad. El informe documenta la inspección de tipos de datos y campos faltantes, la eliminación de duplicados, el análisis de correlación y el perfilado exploratorio.

La información se ordenó temporalmente. El procedimiento descrito incluyó la preparación de una serie con frecuencia diaria y la interpolación de valores faltantes. Estas decisiones deben revisarse al reproducir el análisis: una interpolación puede modificar el comportamiento de la serie y no sustituye la validación de las causas de ausencia de datos.

## Modelado

El informe presenta un enfoque autorregresivo con `ForecasterAutoreg` de skforecast y tres regresores de scikit-learn:

- `DecisionTreeRegressor` para el árbol de regresión.
- `KNeighborsRegressor` para KNN.
- `MLPRegressor` para la red neuronal multicapa.

Se exploraron ventanas de rezagos y combinaciones de hiperparámetros con `grid_search_forecaster`. Las referencias a estas interfaces reflejan el código documentado en 2023; no se han verificado como instrucciones de instalación o ejecución actuales.

## Evaluación

El trabajo describe separación temporal de datos de entrenamiento y prueba, visualización de valores observados y predichos, y comparación con MSE, RMSE, MAE, MAPE y error máximo. El MAPE se utilizó como criterio de selección del modelo reportado en las conclusiones.

La conclusión del informe favorece al árbol de regresión en los experimentos realizados. Esta versión de portafolio no reproduce las métricas ni contiene datos con los que verificarlas independientemente.

## Límites de interpretación

- El resultado es académico y depende de un conjunto de datos concreto.
- El documento no acredita una implantación en producción ni una mejora comercial medida después de su uso.
- La serie, el código ejecutable completo y las versiones de las dependencias no están incluidos en esta publicación.
- Una nueva evaluación requeriría revisar la separación temporal, prevenir el uso de información futura y comparar los modelos con pronósticos de referencia.
- El MAPE debe interpretarse con cuidado cuando existen ventas nulas o cercanas a cero.

