# 🧾 Análisis de Ventas y Rendimiento — *Alura Store LATAM*

## 📋 Descripción general

Este proyecto realiza un **análisis integral del desempeño comercial** de cuatro tiendas distintas, utilizando Python para explorar:

- Qué tiendas generan mayores ingresos.  
- Cuáles son más rentables y muestran mejores tendencias de crecimiento.  
- Cómo se comporta la satisfacción del cliente en cada tienda.  
- Qué tan eficiente es la logística según los costos y destinos de envío.  
- Qué tienda sería más conveniente vender según distintos criterios estratégicos.

El análisis se desarrolla en **Google Colab**, integra múltiples visualizaciones interactivas y genera un **informe en Markdown** con conclusiones y recomendaciones clave.

---

## 🧰 Librerías utilizadas

| Librería | Función |
|----------|---------|
| **pandas** | Manipulación y análisis de datos tabulares |
| **plotly** | Visualizaciones interactivas y dashboards |
| **folium** | Mapas interactivos y análisis geográfico |
| **IPython.display** | Renderizado dinámico de Markdown |

---

## 📂 Estructura del proyecto

**AluraStoreLatam.ipynb**

Incluye:

### 🗂️ 1. Carga y preparación de datos

- Lectura de 4 datasets desde URLs públicas.  
- Limpieza, conversión de tipos y unificación en un DataFrame único (`df_unificado`).

### 📈 2. Funciones de análisis

Entre ellas:

- `total_revenue()`  
- `monthly_revenue()`  
- `quarterly_revenue()`  
- `category_revenue()`  
- `quantity_category()`  
- `quarter_category()`  
- `category_rank()`  
- `store_rating()`  
- `top_products()`  
- `bottom_products()`  
- `product_dependency()`  
- `quarter_products()`

### 📊 3. Visualizaciones

Funciones como:

- `quarterly_chart()`  
- `revenue_graph()`  
- `quantity_graph()`  
- `satisfaction_chart()`  
- `product_dependency_chart()`  
- `top_bottom_chart()`  
- `shipping_location_chart()`  
- `heatmap_store_shipping()`

### 📝 4. Informe final

- `generate_inform()` compila un **informe ejecutivo en Markdown** con análisis y recomendaciones.

---

## 📊 Etapas del análisis

### **1) Importación y unificación de datos**
Se cargan los archivos `tienda_1.csv` a `tienda_4.csv` desde GitHub y se consolidan en un DataFrame principal, agregando indicadores de tienda y normalizando columnas clave.

---

### **2) Análisis descriptivo**

Incluye:

- Ingresos totales y por periodos (mes / trimestre)  
- Participación por categoría  
- Productos más y menos vendidos  
- Calificación promedio por tienda  
- Costos logísticos  
- Dependencia por producto  
- Evolución trimestral  

---

### **3) Visualizaciones**

Se generan gráficos interactivos para:

- Ingresos trimestrales  
- Participación por categoría  
- Volumen por producto  
- Indicadores de satisfacción  
- Mapas de envíos  
- Heatmaps de ciudades por trimestre  

Las visualizaciones utilizan **Plotly** y **Folium**.

---

### **4) Informe automático**

La función `generate_inform()`:

- Presenta el análisis completo paso a paso.  
- Resume puntos clave por área (finanzas, logística, satisfacción, surtido).  
- Genera un texto ejecutivo que sintetiza recomendaciones estratégicas.  

---

## 📈 Resultados esperados

El informe determina qué tienda tiene:

- 💸 Mayor ingreso  
- 📉 Menor ingreso  
- 🚚 Mayor costo logístico  
- 💰 Menor costo logístico  
- ⭐ Mejor calificación  
- ⚠️ Peor calificación  
- 📈 Mejor rendimiento  
- 📉 Peor rendimiento  

También propone **qué tienda vender según distintos objetivos**:

- Maximizar satisfacción del cliente  
- Reducir costos
- Minimizar riesgo comercial
- Enfocarse en crecimiento  
- Obtener liquidez inmediata  

---

## 🧑‍💻 Autor

Proyecto desarrollado como parte del desafío:
**_Practicando Python para Data Science: Challenge Alura Store_**
Analizado y documentado en Google Colab como práctica de análisis de datos, visualización e interpretación estratégica.

---