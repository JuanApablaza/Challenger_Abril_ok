# Análisis de Rentabilidad de Tiendas 🏪📊

Este proyecto realiza un análisis comparativo de 4 tiendas en base a datos de ventas, costos de envío, calificaciones y categorías de productos.

## 📌 Descripción

El análisis incluye:
- Facturación total por tienda
- Ventas por categoría de producto
- Calificación promedio de clientes
- Productos más y menos vendidos
- Costos de envío
- Cálculo de utilidades (precio - costo de envío)

## 📊 Resultados Clave

### Facturación Total
| Tienda   | Facturación      |
|----------|------------------|
| Tienda 1 | $1,150,880,400   |
| Tienda 2 | $1,116,343,500   |
| Tienda 3 | $1,098,019,600   |
| Tienda 4 | $1,038,375,700   |
| **Total**| **$4,403,619,200** |

### Calificaciones Promedio
| Tienda   | Calificación |
|----------|--------------|
| Tienda 1 | 3.977        |
| Tienda 2 | 4.037        |
| Tienda 3 | 4.048        |
| Tienda 4 | 3.996        |
| **Promedio Total** | **4.015** |

### Utilidades
![Utilidad por Tienda](utilidad_plot.png)

## 🔍 Hallazgos Principales

1. **Tienda 4 tiene el peor desempeño**:
   - Menor facturación ($1,038M vs promedio $1,101M)
   - Utilidades más bajas
   - Costos de envío más bajos (no se traduce en mejores resultados)
   - 3° peor calificación (3.996)

2. **Categorías más populares**:
   - Muebles (1,886 unidades)
   - Electrónicos (1,772 unidades)
   - Juguetes (1,290 unidades)

3. **Productos destacados**:
   - Más vendido: "Mesa de noche"
   - Menos vendido: "Celular ABXY"

## 🚀 Recomendación

**Cerrar la Tienda 4** debido a:
- Bajo rendimiento financiero
- Utilidades consistentemente inferiores
- Calificaciones mediocres
- Costos bajos que no generan ventaja competitiva

## 💻 Código

El análisis completo se realizó en Python usando:
```python
import pandas as pd
import matplotlib.pyplot as plt

# Carga de datos
urls = [...]
tiendas = [pd.read_csv(url) for url in urls]

# Análisis (ver notebook completo)
