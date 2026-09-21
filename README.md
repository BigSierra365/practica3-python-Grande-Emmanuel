# Práctica 3: Python — Emmanuel Grande Sierra

## Descripción
Resolución de los 20 ejercicios de la Práctica 3 sobre listas, funciones y
paquetes, NumPy, diccionarios y pandas, lógica y control de flujo, y bucles.

## Entorno
- Python 3.12
- JupyterLab
- NumPy, pandas (ver `requirements.txt`)

## Estructura del repositorio
| Carpeta | Contenido |
| --- | --- |
| `data/` | Ficheros CSV de partida |
| `notebooks/` | Notebook con la resolución |
| `src/` | Módulo de funciones auxiliares |
| `outputs/` | Ficheros generados durante la ejecución |

## Cómo reproducir
```bash
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab notebooks/practica3_python.ipynb
```

---

## Contenido del notebook

El notebook contiene **20 ejercicios organizados en 6 secciones:**

### Sección 3: Listas (Ejercicios 1-4)
- **E1:** Catálogo de productos con slicing
- **E2:** Inventario multialmacén con listas anidadas
- **E3:** Copias de listas y referencias en memoria
- **E4:** Cola de pedidos con operaciones FIFO

### Sección 4: Funciones y Paquetes (Ejercicios 5-11)
- **E5:** Funciones con parámetros por defecto y tuplas
- **E6:** Normalización de strings con métodos
- **E7:** Importaciones y módulo propio `utilidades.py`
- **E8:** Cálculo vectorizado con NumPy vs listas
- **E9:** Máscaras booleanas y subsetting
- **E10:** Matrices 2D, shape, indexación
- **E11:** Estadística descriptiva y correlación

### Sección 6: Diccionarios y Pandas (Ejercicios 12-15)
- **E12:** Diccionarios simples y anidados
- **E13:** De diccionario a DataFrame, lectura de CSV
- **E14:** Selección con corchetes, `loc`, `iloc`
- **E15:** Columnas calculadas, agregación, exportación

### Sección 7: Lógica y Control de Flujo (Ejercicios 16-18)
- **E16:** Operadores booleanos y comparaciones
- **E17:** Condicionales if/elif/else aplicados a mantenimiento predictivo
- **E18:** Filtrado avanzado de DataFrames con `query()` e `.isin()`

### Sección 8: Bucles (Ejercicios 19-20)
- **E19:** Bucles while, for, enumerate, desempaquetado
- **E20:** Iteración sobre DataFrames con `.iterrows()`, creación de diccionarios

---

## Validación del entorno

La **primera celda del notebook** contiene esta verificación obligatoria:

```python
import sys
import platform
import numpy as np
import pandas as pd

print("Python      :", sys.version)
print("Implementación:", platform.python_implementation())
print("NumPy       :", np.__version__)
print("pandas      :", pd.__version__)

assert sys.version_info[:2] == (3, 12), "Esta práctica requiere Python 3.12"
print("\nEntorno verificado correctamente.")
```

Si el `assert` falla, verifica que el **kernel seleccionado en JupyterLab** apunte a tu entorno virtual con Python 3.12.

---

