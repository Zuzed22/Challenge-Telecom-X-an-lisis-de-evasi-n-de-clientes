Proyecto de Análisis de Evasión de Clientes (Churn) - Telecom X
## 🚀 Propósito del Proyecto

Este proyecto tiene como objetivo analizar la evasión de clientes (churn) en la empresa **Telecom X** mediante el uso de Python, ciencia de datos y aprendizaje automático. A partir de los datos de clientes, se exploran patrones de cancelación, se entrenan modelos predictivos y se generan recomendaciones para reducir la fuga de clientes.

## 📂 Estructura del Proyecto

```
TelecomX-Churn/
├── data/                       # Datos originales y procesados
│   ├── TelecomX_Data.json
│   ├── telecomx_flat_renombrado.parquet
│   └── clientes_alto_riesgo.csv
├── notebooks/                 # Análisis exploratorio y modelado
├── scripts/                   # Funciones reutilizables (ETL, modelado)
├── models/                    # Modelos entrenados
├── TelecomX_LATAM.ipynb       # Informe final
└── README.md                  # Este archivo
```
## ⚙️ Instalación y Requisitos

### Requisitos previos

- Python 3.8 o superior
    
- pip
    

### Instalación de dependencias

Con `pip`:

```
pip install -r requirements.txt
```

O instala manualmente:

```
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm
```
## 📃 Uso del Proyecto

### 1. Clonar el repositorio

```
git clone https://github.com/tu-usuario/telecomx-churn.git
cd telecomx-churn
```

### 2. Correr el flujo de análisis

Puedes abrir y ejecutar el notebook principal en Jupyter o Google Colab:

```
notebooks/analisis_churn.ipynb
```

O ejecutar scripts desde la terminal o editor:

```
from scripts.modeling import train_model
model, X_test, y_test = train_model(df)
```

### 3. Generar lista de clientes en riesgo

```
from scripts.alerts import export_alerts
export_alerts(df, model)
```

## ⚠️ Posibles Problemas y Soluciones

|Problema común|Solución|
|---|---|
|`ModuleNotFoundError`|Verifica que instalaste todas las dependencias|
|`ValueError: could not convert string...`|Revisa limpieza de datos y tipos|
|`LightGBMError: categorical_feature`|Asegúrate de que las columnas sean tipo category|

## 🙌 Contribuciones

Este proyecto está abierto a mejoras. Para contribuir:

1. Haz un fork del repositorio
    
2. Crea una nueva rama: `git checkout -b feature/nombre`
    
3. Realiza tus cambios y haz commit
    
4. Sube la rama y abre un Pull Request
    

## 🙏 Agradecimientos

Este proyecto forma parte del desafío de ciencia de datos AuraLATAM. Gracias a todos los que aportaron conocimiento y revisiones.

**Autor:** [Zuleika González]  
