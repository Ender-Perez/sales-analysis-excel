# Análisis de Ventas 2024

## Objetivo
Analizar la evolución de las ventas durante el año 2024, identificar productos y categorías con bajo rendimiento y detectar posibles causas de caídas en el nivel de ventas para proponer acciones de mejora basadas en datos.

---

## Contexto
El análisis se realiza sobre un dataset de ventas minoristas que contiene información de productos, categorías, fechas, unidades vendidas, precios y regiones.  
El dataset presenta errores típicos de carga, como valores negativos y datos inconsistentes, simulando un escenario real de trabajo.

---

## Herramientas utilizadas
- Microsoft Excel
- Tablas dinámicas
- Gráficos de columnas y barras

---

## Proceso de análisis

### Limpieza de datos
Se detectaron registros con ventas negativas, los cuales fueron interpretados como errores de carga.  
Dado que el dataset no cuenta con un campo que identifique devoluciones, estos registros fueron eliminados del análisis, ya que distorsionan métricas clave como ventas totales y ticket promedio.

Luego de la limpieza, el dataset final quedó compuesto por **397 registros válidos**.

---

### Análisis de ventas por mes
Se realizó un análisis de la evolución mensual de las ventas utilizando tablas dinámicas y gráficos.

Se observa una caída significativa en el nivel de ventas durante el primer trimestre del año.  
En enero las ventas alcanzan $22.571.592, en febrero se produce una recuperación hasta $36.157.061 y en marzo se registra el nivel más bajo del año con $16.468.357.  
A partir de abril, las ventas se recuperan y mantienen un comportamiento estable durante el resto del año.

La disminución de ventas observada se explica principalmente por una fuerte caída en las unidades vendidas, más que por una reducción del ticket promedio.

(images/ventas_mensuales.png)

---

### Análisis por categoría
La categoría con mayor peso en el negocio es "Electrónica", tanto en volumen de unidades vendidas como en facturación total.  
La categoría con peor rendimiento es "Oficina", con un total de 281 unidades vendidas.

No se identificaron categorías con alto volumen de ventas y baja facturación. Las categorías analizadas mantienen una relación proporcional entre unidades vendidas y monto facturado.

(images/ventas_categoria.png)

---

### Productos con bajo rendimiento
Se identificaron los productos con menor volumen de ventas: "Impresora", "Router" y "Tablet", con 281, 294 y 340 unidades vendidas respectivamente.

Se detecta un comportamiento atípico en el producto "Router", cuyo nivel de facturación es similar al de "Notebook", a pesar de vender menos unidades.  
Por ejemplo, Router registra 294 unidades y $51.567.454, mientras que Notebook alcanza 366 unidades y $50.929.468, lo que sugiere un precio unitario elevado para el Router en comparación con otros productos.

(images/bottom_productos.png)

---

## Conclusiones y recomendaciones
- La principal caída de ventas se debe a una reducción en el volumen de unidades vendidas, especialmente durante el primer trimestre.
- La categoría Oficina presenta bajo rendimiento y podría requerir una revisión de su estrategia comercial.
- El producto Router muestra un precio unitario elevado en relación con otros productos como la Notebook que es más barata, lo que podría estar afectando su rotación.
- Se recomienda analizar estrategias de pricing y promociones para los productos con bajo desempeño.

---

## Archivos del proyecto
- 'ventas_original.xlsx': dataset original sin modificaciones  
- 'ventas_limpias.xlsx': dataset luego del proceso de limpieza  
- Gráficos en formato PNG para visualización de resultados
