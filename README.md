 #  🧾 Análisis de Ventas y Rendimiento de Alura Store
 
## 📋 Descripción general

Este proyecto realiza un **análisis integral de datos de ventas** provenientes de cuatro tiendas diferentes.  
Utilizando Python y diversas bibliotecas de análisis y visualización, se busca identificar:

* Qué tiendas generan mayores ingresos.
* Cuáles son más rentables.
* Cómo varía la satisfacción de los clientes.
* Qué estrategias podrían aplicarse si el dueño quisiera vender alguna tienda.

El trabajo se desarrolla originalmente en Google Colab y genera **un informe en Markdown y HTML**, que incluye texto interpretativo y gráficos generados dinámicamente.

## 🧰 Librerías utilizadas

| Librería | Descripción |
|------------|------------|
| pandas | Manipulación y análisis de datos tabulares |
| matplotlib | Visualización gráfica básica (barras, dispersión, etc) |
| seaborn | Extensión de Matplotlib para gráficos estadísticos con mejor estética |
| plotly | Visualizaciones interactivas, especialmente para indicadores de satisfacción |
| folium | Mapas interactivos (visualización geográfica de las tiendas) |
| IPython.display | Renderizado de Markdown dentro del notebook |

## 📂 Estructura del proyecto

AluraStoreLatam.ipynb
│
├── Carga de datos (4 tiendas desde URLs públicas)
├── Limpieza y unificación de datos
├── Funciones de análisis:
│   ├── calcular_ingreso_por_tienda()
│   ├── calcular_ventas_por_categoria()
│   ├── calcular_calificaciones_promedio()
│   ├── productos_mas_y_menos_vendidos()
│   ├── costo_envio_promedio()
│   └── rendimiento (Ingreso - Costos)
│
├── Visualizaciones:
│   ├── graficar_ingreso_por_tienda()
│   ├── graficar_satisfaccion_tiendas()
│   ├── graficar_costo_envio_promedio()
│   ├── graficar_rendimiento_tiendas()
│   └── visualizar_mapa_cluster_tiendas()
│
└── Informe final:
    └── generar_informe_venta_tienda()

## 📊 Etapas del análisis

### 1) Importación y unificación de datos

Se cargan los datasets `tienda_1.csv` a `tienda_4.csv` desde GitHub y se combinan en un único DataFrame (`df_unificado`).

### 2) Análisis descriptivo

* Ingresos totales por tienda
* Ventas por categoría de producto
* Productos más y menos vendidos
* Calificación promedio
* Costos logísticos
* Rendimiento neto (Ingreso - Costo de envío)

### 3) Visualizaciones

Cada sección genera gráficos para ilustrar los resultados:

* Barras comparativas (`matplotlib` + `seaborn`).
* Indicadores tipo gauge (`plotly`).
* Dispersión de costos promedio.
* Mapas interactivos (`folium`).

### 4) Informe

La función `generar_informe_venta_tienda()`:

* Presenta el análisis paso a paso.
* Muestra los gráficos correspondientes.
* Genera un texto conclusivo con recomendaciones estratégicas.

## 📈 Resultados esperados

El análisis final resume qué tienda tiene:

* 💸 Mayor ingreso
* 📉 Menor ingreso
* 🚚 Mayor costo logístico
* 💰 Menor costo logístico
* ⭐ Mejor calificación
* ⚠️ Peor calificación
* 📈 Mejor rendimiento (beneficio neto)
* 📉 Peor rendimiento

Además, recomienda qué tienda vender según distintos objetivos: eficiencia, reputación, reducción de costos o capital inmediato.

## 🧑‍💻 Autor

Proyecto desarrollado como práctica de análisis de datos con Python y Google Colab.  
_Practicando Python para Data Science: Challenge Alura Store_