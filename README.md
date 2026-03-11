Analisis de Evasion de Clientes - Proyecto Telecom X

Resumen del Proyecto
Este proyecto consiste en el desarrollo de un modelo de aprendizaje automatico para predecir la cancelacion de clientes (churn) en una empresa de telecomunicaciones. El analisis abarca desde la exploracion inicial de los datos y el preprocesamiento hasta la evaluacion de modelos de clasificacion, con el fin de proporcionar insights accionables que permitan reducir la tasa de perdida de usuarios.

Tecnologias Utilizadas
Python
Pandas y NumPy (Procesamiento de datos)
Matplotlib y Seaborn (Visualizacion)
Scikit-Learn (Modelado y metricas)
Imbalanced-learn (Tecnica SMOTE para balanceo de clases)

Metodologia Aplicada
1. Preprocesamiento y Limpieza
Se realizo una limpieza exhaustiva de la base de datos, eliminando columnas irrelevantes y gestionando variables categoricas mediante tecnicas de One-Hot Encoding. Las variables numericas fueron estandarizadas para garantizar que los modelos basados en distancias no presentaran sesgos por la magnitud de los datos.

2. Tratamiento de Datos Desbalanceados
Dado que la clase minoritaria (clientes que cancelan) representaba aproximadamente el 26.5% del total, se aplico la tecnica SMOTE (Synthetic Minority Over-sampling Technique). Esto permitio entrenar los modelos con una distribucion equilibrada del 50/50, mejorando significativamente la capacidad de deteccion de fuga de clientes.

3. Modelado y Evaluacion
Se entrenaron y compararon dos modelos principales:

Regresion Logistica: Utilizada como base por su alta interpretabilidad.

Random Forest: Seleccionado como el modelo final debido a su superioridad en la metrica de Recall (0.85) y su capacidad para capturar relaciones complejas no lineales.

Hallazgos Principales
El tipo de contrato mensual es el factor con mayor correlacion positiva hacia la evasion.

Los servicios de Fibra Optica presentan una tasa de cancelacion mas alta en comparacion con otras tecnologias.

La permanencia del cliente es critica; los usuarios con menos de 12 meses de antiguedad son los mas propensos a abandonar el servicio.

El metodo de pago por cheque electronico muestra una relacion directa con mayores niveles de churn.

Estrategias de Retencion Sugeridas
Implementacion de incentivos para la migracion de contratos mensuales a planes anuales.

Monitoreo proactivo de la satisfaccion del cliente durante el primer año de servicio.

Revision tecnica de la estabilidad del servicio de fibra optica en zonas de alta desercion.

Fomento de metodos de pago automaticos para reducir la friccion administrativa.

Instrucciones de Uso
Clonar el repositorio:
git clone https://github.com/DAMS-1/Challenge-2---Telecom-X.git

Instalar dependencias:
pip install pandas scikit-learn matplotlib seaborn imbalanced-learn

Ejecutar el notebook de Jupyter o Google Colab para replicar el analisis.
