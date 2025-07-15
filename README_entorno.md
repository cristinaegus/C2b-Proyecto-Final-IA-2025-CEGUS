# VinoValue - Predicción de Precios de Vinos Españoles

## Configuración del Entorno Virtual

### Prerrequisitos

- Python 3.12 o superior instalado en tu sistema
- VS Code con las extensiones de Python y Jupyter

### Estructura del Proyecto

```
ProyectoFinal2025Cegus/
├── venv_vinovalue/              # Entorno virtual
├── vinovalue-predicting-spanish-wine-price.ipynb  # Notebook principal
├── wines_SPA (1).csv           # Dataset de vinos españoles
├── requirements.txt            # Dependencias del proyecto
├── activar_entorno.bat         # Script para activar el entorno
├── iniciar_jupyter.bat         # Script para iniciar Jupyter
└── README.md                   # Este archivo
```

### Instalación y Configuración

#### Opción 1: Usando los scripts incluidos

1. **Activar el entorno virtual:**

   - Hacer doble clic en `activar_entorno.bat`
   - O desde PowerShell: `.\activar_entorno.bat`

2. **Iniciar Jupyter Notebook:**
   - Hacer doble clic en `iniciar_jupyter.bat`
   - O desde PowerShell: `.\iniciar_jupyter.bat`

#### Opción 2: Manualmente desde PowerShell

```powershell
# Activar el entorno virtual
.\venv_vinovalue\Scripts\Activate.ps1

# Verificar las librerías instaladas
pip list

# Iniciar Jupyter Notebook
jupyter notebook
```

### Librerías Instaladas

- **jupyter**: Entorno de desarrollo interactivo
- **pandas**: Manipulación y análisis de datos
- **numpy**: Computación numérica
- **matplotlib**: Visualización de datos
- **seaborn**: Visualización estadística
- **scikit-learn**: Machine Learning
- **tensorflow**: Deep Learning
- **keras**: API de alto nivel para TensorFlow
- **keras-tuner**: Optimización de hiperparámetros
- **plotly**: Visualizaciones interactivas

### Uso del Notebook

1. Una vez que Jupyter esté ejecutándose, abre el archivo:
   `vinovalue-predicting-spanish-wine-price.ipynb`

2. El notebook ya está configurado con el kernel correcto (`venv_vinovalue`)

3. Puedes ejecutar las celdas secuencialmente para:
   - Cargar y explorar el dataset de vinos españoles
   - Realizar análisis exploratorio de datos
   - Entrenar modelos de machine learning
   - Predecir precios de vinos

### Desactivar el Entorno

Para desactivar el entorno virtual:

```powershell
deactivate
```

### Troubleshooting

**Si encuentras errores de permisos en PowerShell:**

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

**Para reinstalar las dependencias:**

```powershell
pip install -r requirements.txt
```

**Para actualizar las librerías:**

```powershell
pip install --upgrade -r requirements.txt
```

### Información del Proyecto

- **Objetivo**: Predicción de precios de vinos españoles usando machine learning
- **Dataset**: 7,500 vinos tintos españoles
- **Tecnologías**: Python, TensorFlow, scikit-learn, Jupyter
- **Entorno**: Python 3.12.10 con entorno virtual

¡El entorno está listo para trabajar con el análisis de vinos españoles! 🍷
