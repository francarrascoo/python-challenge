# Análisis de Datos de Ventas de Tiendas

Este proyecto realiza la importación y análisis básico de datos de ventas de cuatro tiendas diferentes, usando pandas para manipulación de datos. Se incluyen análisis de facturación, ventas por categoría, calificación promedio y productos más y menos vendidos.

---

## Contenido

1. [Importación de datos](#importación-de-datos)  
2. [Análisis de facturación](#análisis-de-facturación)  
3. [Ventas por categoría](#ventas-por-categoría)  
4. [Calificación promedio](#calificación-promedio)  
5. [Productos más y menos vendidos](#productos-más-y-menos-vendidos)  

---

## Importación de Datos

Se importan los datos desde archivos CSV disponibles en URLs públicas con pandas.

```python
import pandas as pd

url1 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_1%20.csv"
url2 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_2.csv"
url3 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_3.csv"
url4 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_4.csv"

tienda1 = pd.read_csv(url1)
tienda2 = pd.read_csv(url2)
tienda3 = pd.read_csv(url3)
tienda4 = pd.read_csv(url4)
```
---

## Análisis de facturación

Calcula la suma total de precios vendidos por tienda.

Ejemplo:

```python
total_tienda1 = tienda1["Precio"].sum()
print(f"Ingreso total tienda 1: {total_tienda1}")

total_tienda2 = tienda2["Precio"].sum()
print(f"Ingreso total tienda 2: {total_tienda2}")

total_tienda3 = tienda3["Precio"].sum()
print(f"Ingreso total tienda 3: {total_tienda3}")

total_tienda4 = tienda4["Precio"].sum()
print(f"Ingreso total tienda 4: {total_tienda4}")
```
---

## Ventas por categoría

Se realiza un análisis agrupando los productos vendidos según su categoría, para entender cuáles son las categorías con mayor volumen de ventas y su aporte a los ingresos totales.

---

## Calificación promedio

Con los datos de calificaciones de productos o servicios, se calcula el promedio para evaluar la satisfacción general de los clientes en cada tienda, lo que puede ayudar a identificar áreas de mejora.

---
## Productos Más y Menos Vendidos

Se identifican los productos con mayores y menores cantidades vendidas para conocer cuáles son los artículos más populares y aquellos que requieren estrategias para impulsar su venta.

---
