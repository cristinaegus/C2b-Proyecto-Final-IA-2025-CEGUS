# Solución de TensorFlow DLL Error en Windows

## Error encontrado:

ImportError: DLL load failed while importing \_pywrap_tensorflow_internal

## Soluciones aplicadas:

### 1. ✅ Instalación de TensorFlow-CPU 2.15.0

- Desinstalamos TensorFlow 2.19.0 que tenía problemas de compatibilidad
- Instalamos tensorflow-cpu==2.15.0 que es más estable en Windows

### 2. 📦 Dependencias adicionales requeridas:

Si persiste el error, instalar:

- Microsoft Visual C++ Redistributable for Visual Studio 2015-2022
- Descargar desde: https://aka.ms/vs/17/release/vc_redist.x64.exe

### 3. 🔄 Alternativas si el problema continúa:

```bash
# Opción A: TensorFlow con CPU específico
pip install tensorflow-cpu==2.15.0

# Opción B: Usar librerías alternativas para este proyecto
pip install scikit-learn xgboost lightgbm

# Opción C: Versión de TensorFlow compatible
pip install tensorflow==2.13.0
```

### 4. 🧪 Verificación:

```python
# Probar la importación
try:
    import tensorflow as tf
    print(f"TensorFlow version: {tf.__version__}")
    print("✅ TensorFlow importado correctamente")
except ImportError as e:
    print(f"❌ Error: {e}")
```

### 5. 📝 Notas importantes:

- TensorFlow-CPU es suficiente para este proyecto de vinos
- No requiere GPU para datasets de 7,500 registros
- Versiones 2.15.x son más estables en Windows 11
