# Pronóstico de ventas en el sector textil

Caso de estudio académico desarrollado en 2023 como trabajo de grado de la **Especialización en Analítica de Datos Aplicada a los Negocios** de la **Institución Universitaria EAM**. El proyecto estudió cómo utilizar datos históricos de ventas para apoyar la planificación comercial mediante modelos de pronóstico.

Esta versión de portafolio presenta el problema, el proceso analítico y las herramientas empleadas. Los registros comerciales, los datos de contacto y el informe con información privada se excluyen de esta publicación.

## Autoría

- **Juan Diego Londoño Álvarez** — coautor del proyecto.
- **Andrés Felipe Serna Muñoz** — coautor del proyecto.
- **Sergio Augusto Cardona Torres** — asesor académico.

## Objetivo

Proponer y comparar modelos predictivos de ventas a partir de información histórica, después de preparar los datos y evaluar el comportamiento de las series de tiempo.

## Trabajo realizado

1. Comprensión del problema de negocio siguiendo la metodología **CRISP-DM**.
2. Revisión de tipos de datos, valores faltantes y registros duplicados.
3. Preparación y estructuración de la información para el análisis.
4. Exploración de variables y relaciones mediante perfilado de datos y correlación.
5. Organización temporal de la serie y separación de conjuntos de entrenamiento y prueba.
6. Comparación de **árbol de regresión**, **K vecinos más cercanos (KNN)** y **red neuronal multicapa** mediante un enfoque autorregresivo.
7. Exploración de hiperparámetros y evaluación con métricas de error.

## Herramientas documentadas

| Herramienta | Uso en el proyecto |
| --- | --- |
| Python y Google Colab | Preparación, exploración y modelado |
| pandas y NumPy | Manipulación de datos y cálculos |
| scikit-learn | Modelos de regresión y métricas |
| skforecast | Pronósticos autorregresivos y búsqueda de hiperparámetros |
| Matplotlib | Visualización de resultados |
| pandas_profiling | Informe exploratorio de los datos |

El informe también describe un entorno empresarial con SQL Server. La evidencia disponible no permite atribuir a los autores el desarrollo de consultas SQL específicas dentro de este proyecto.

## Resultados y alcance

El trabajo documentó una comparación entre los tres enfoques. Según la conclusión del informe, el árbol de regresión obtuvo el menor MAPE dentro de los experimentos realizados. La experiencia permitió aplicar preparación de datos, análisis exploratorio, series de tiempo y evaluación de modelos a un problema de negocio.

No se presentan cifras comerciales ni se afirma una mejora de ventas o un despliegue productivo. Los resultados pertenecen al contexto y a los datos utilizados en el trabajo académico.

## Contenido del repositorio

- [Proceso analítico](docs/proceso-analitico.md): resumen de la metodología y las etapas documentadas.
- [Fuentes y alcance de esta versión](docs/fuentes-y-alcance.md): procedencia, restricciones de reproducción y atribución.

## Reproducibilidad

Este repositorio es una ficha del caso de estudio. No incluye el conjunto de datos privado, los cuadernos originales ni un programa ejecutable. Los fragmentos del informe no constituyen por sí solos un flujo completo reproducible, por lo que no se han reconstruido resultados ni añadido código nuevo para simularlos.

