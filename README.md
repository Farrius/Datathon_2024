# Datathon 2024
#### Desarolladores
- Oscar Garries
- Ismael el Basli
- Jordi Muñoz

Este repositorio contiene los archivos y scripts utilizados por nuestro equipo formado por Oscar Garries, Ismael el Basli i Jordi Muñoz en la participación de la **Datathon 2024**. A continuación, describiremos la estructura y propósito de cada archivo.

## Estructura del repositorio

### **Archivos de datos**
Se deberian añadir los 4 documentos siguientes en el directorio padre del actual dado que los datos eran confidenciales los dos primeros se utilizan en el archivo restb.ipynb para procesar y transformar los datos y los dos últimos se utilizan en el notebook models_training ya que ya contienen los datos procesados correctamente.
- **`train.csv`** 
- **`test.csv`**
- **`processed_train.csv`**
- **`processed_train.csv`**

### **Predicciones y resultados**
En la carpeta resultados_obtenidos tenemos
- **`GradientBoosting_predictions.csv`**: Predicciones generadas por el modelo Gradient Boosting.
- **`GradientBoosting_results.csv`**: Métricas de evaluación del modelo Gradient Boosting.
- **`LinearRegression_predictions.csv`**: Predicciones generadas por el modelo de regresión lineal.
- **`LinearRegression_results.csv`**: Métricas de evaluación del modelo de regresión lineal.
- **`RandomForest_predictions.csv`**: Predicciones generadas por el modelo Random Forest.
- **`RandomForest_results.csv`**: Métricas de evaluación del modelo Random Forest.
- **`SVR_predictions.csv`**: Predicciones generadas por el modelo de soporte vectorial (SVR).
- **`SVR_results.csv`**: Métricas de evaluación del modelo de soporte vectorial (SVR).
- **`XGBoost_predictions.csv`**: Predicciones generadas por el modelo XGBoost.
- **`XGBoost_results.csv`**: Métricas de evaluación del modelo XGBoost.

### **Scripts**
- **`restb.ipynb`**: Notebooks que se encarga de todo el procesamiento de datos.
- **`models_training.ipynb`**: Notebook para el entrenamiento de diferentes modelos aplicados.

### **Otros archivos**
- **`notas.md`**: Archivo que contiene toda la bibliografia, todos los articulos e información consultada e ideas y observaciones sobre el proyecto.
- **`preprocessing.md`**: Documento que describe los pasos de clave del preprocesamiento aplicados a los datos.
- **`requirements.txt`**: Lista de dependencias y librerías necesarias para ejecutar los scripts.

## Para usar este repositorio

1. **Importar datos**
- importar los raw .csv (train.csv y test.csv) en el directorio root del actual

2. **Instalar dependencias**:
   ```bash
   pip install -r requirements.txt
