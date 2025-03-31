# 📈 Portfolio Optimization with Hierarchical Clustering and Markowitz

This project uses **Hierarchical Clustering** 🔗 techniques and the optimization of the **Efficient Frontier** 📊 from **Markowitz** to build a diversified and optimized investment portfolio, based on historical asset price data.

## 🛠️ Process Steps

1. 📥 **Data Acquisition**: Download historical asset prices from Yahoo Finance.
2. 📊 **Logarithmic Returns Calculation**: The daily returns of each asset are calculated using the historical prices.
3. 🔗 **Correlation Analysis**: Evaluation of the correlation between assets to understand their relationship and facilitate clustering.
4. 🧩 **Hierarchical Clustering**: A hierarchical clustering analysis is performed to identify groups of assets with similar behaviors.
5. 📈 **Markowitz Optimization**: The portfolio is optimized by finding the best combination of assets with the highest risk-adjusted return (Sharpe ratio).
6. 🎯 **Efficient Frontier**: A visualization of the efficient frontier is generated, showing the relationship between risk (volatility) and return.
7. 📌 **Asset Selection**: Representative assets are selected for each cluster based on their performance and volatility.
8. ✅ **Optimization and Results**: The optimal portfolio is calculated, visualizing its performance and historical price evolution.

## 🔧 Requirements

To run this code, you need to install the following Python libraries:

- 📦 `yfinance` → For downloading historical asset price data.
- 🔢 `numpy` → For numerical calculations.
- 🗃️ `pandas` → For data handling.
- 📊 `matplotlib` and `seaborn` → For visualizing graphs.
- 🤖 `scikit-learn` → For applying machine learning techniques like PCA, clustering, and normalization.
- 🔍 `scipy` → For optimization and distance calculations.

## 📜 Process Description

### 1️⃣ Logarithmic Returns Calculation  
📈 Logarithmic returns of the assets are calculated from the closing prices obtained from Yahoo Finance. This allows for more accurate modeling of the asset behaviors and takes advantage of favorable statistical properties.

### 2️⃣ Correlation Analysis  
🔗 A **correlation matrix** 📊 is calculated to assess the relationships between assets. Assets with high correlation tend to move similarly, which aids the clustering process.

### 3️⃣ Hierarchical Clustering  
🧩 **Hierarchical Clustering** is applied to group similar assets. The distance between assets (calculated from correlation) is used to form **clusters**. The **Silhouette Score** 📊 is used to determine the optimal number of clusters.

### 4️⃣ Portfolio Optimization (Markowitz)  
📈 Using the **Markowitz Model**, the combination of assets is found that **maximizes the Sharpe ratio** (risk-adjusted return). The selection of assets from each cluster is optimized to achieve an efficient portfolio.

### 5️⃣ Efficient Frontier  
🎯 A chart of the **Efficient Frontier** is generated, showing the relationship between risk (volatility) and the expected return of the portfolio. The optimal portfolio is highlighted within this frontier.

### 6️⃣ Portfolio Evolution  
📊 The historical evolution of the optimized portfolio is calculated, showing how the portfolio value would have grown over time.

## 📊 Results

The code outputs:

✅ The optimal number of clusters based on the correlation analysis.  
✅ The assets selected for the optimized portfolio.  
✅ The weights of each asset in the optimal portfolio.  
✅ The expected return, volatility, and Sharpe ratio of the optimal portfolio.  
✅ The historical evolution of the portfolio value.

## 📡 Visualizations

The code generates several visualizations, including:

🔗 **Correlation Matrix** → Displays the relationship between assets.  
📉 **Hierarchical Clustering Dendrogram** → Visualization of the asset groups.  
📊 **Silhouette Score** → A chart to help determine the optimal number of clusters.  
📈 **Efficient Frontier** → Displays the relationship between risk and return for different asset combinations.  
📉 **Portfolio Historical Evolution** → Shows the growth of the portfolio value over time.




--------------------------------------------------------------------------------------------------------------------------------------




# 📈 Optimización de Portafolio con Clustering Jerárquico y Markowitz  

Este proyecto utiliza técnicas de **Clustering Jerárquico** 🔗 y la optimización de la **Frontera Eficiente** 📊 de **Markowitz** para construir un portafolio de inversión diversificado y optimizado, basado en datos históricos de precios de activos financieros.  

## 🛠️ Pasos del Proceso  

1. 📥 **Obtención de datos**: Descarga de precios históricos de activos financieros desde Yahoo Finance.  
2. 📊 **Cálculo de retornos logarítmicos**: Los retornos diarios de cada activo se calculan usando los precios históricos.  
3. 🔗 **Análisis de Correlación**: Evaluación de la correlación entre activos para entender su relación y facilitar el clustering.  
4. 🧩 **Clustering Jerárquico**: Se realiza un análisis de agrupamiento jerárquico para identificar grupos de activos con comportamientos similares.  
5. 📈 **Optimización de Markowitz**: Se optimiza el portafolio buscando la mejor combinación de activos con el mejor rendimiento ajustado por riesgo (índice de Sharpe).  
6. 🎯 **Frontera Eficiente**: Se genera una visualización de la frontera eficiente que muestra la relación entre riesgo (volatilidad) y retorno.  
7. 📌 **Selección de Activos**: Se seleccionan activos representativos para cada cluster basándose en su rendimiento y volatilidad.  
8. ✅ **Optimización y Resultados**: Se calcula el portafolio óptimo, visualizando su rendimiento y la evolución histórica de su precio.  

## 🔧 Requisitos  

Para ejecutar este código, necesitas instalar las siguientes bibliotecas de Python:  

- 📦 `yfinance` → Para descargar datos históricos de activos financieros.  
- 🔢 `numpy` → Para cálculos numéricos.  
- 🗃️ `pandas` → Para manejo de datos.  
- 📊 `matplotlib` y `seaborn` → Para visualización de gráficos.  
- 🤖 `scikit-learn` → Para aplicar técnicas de machine learning como PCA, clustering y normalización.  
- 🔍 `scipy` → Para optimización y manejo de distancias.  

## 📜 Descripción del Proceso  

### 1️⃣ Cálculo de los retornos logarítmicos  
📈 Se calculan los retornos logarítmicos de los activos a partir de los precios de cierre obtenidos de Yahoo Finance. Esto permite modelar mejor su comportamiento y aprovechar sus propiedades estadísticas favorables.  

### 2️⃣ Análisis de Correlación  
🔗 Se calcula una **matriz de correlación** 📊 para evaluar las relaciones entre los activos. Activos con alta correlación tienden a moverse de manera similar, lo que ayuda en el proceso de clustering.  

### 3️⃣ Clustering Jerárquico  
🧩 Se aplica **Clustering Jerárquico** para agrupar activos similares. Se usa la distancia entre los activos (calculada a partir de la correlación) para formar **clusters**. Se emplea el **Silhouette Score** 📊 para determinar el número óptimo de clusters.  

### 4️⃣ Optimización del Portafolio (Markowitz)  
📈 Utilizando el **Modelo de Markowitz**, se encuentra la combinación de activos que **maximiza el índice de Sharpe** (rendimiento ajustado por riesgo). Se optimiza la selección de activos de cada cluster para lograr un portafolio eficiente.  

### 5️⃣ Frontera Eficiente  
🎯 Se genera una gráfica de la **Frontera Eficiente**, que muestra la relación entre el riesgo (volatilidad) y el retorno esperado del portafolio. El portafolio óptimo se resalta dentro de esta frontera.  

### 6️⃣ Evolución del Portafolio  
📊 Se calcula la evolución histórica del portafolio optimizado, mostrando cómo habría crecido el valor del portafolio a lo largo del tiempo.  

## 📊 Resultados  

El código imprime:  

✅ El número óptimo de clusters basado en el análisis de correlación.  
✅ Los activos seleccionados para el portafolio optimizado.  
✅ Los pesos de cada activo en el portafolio óptimo.  
✅ El rendimiento esperado, la volatilidad y el índice de Sharpe del portafolio óptimo.  
✅ La evolución histórica del valor del portafolio.  

## 📡 Visualizaciones  

El código genera varias visualizaciones, entre ellas:  

🔗 **Matriz de correlación** → Muestra la relación entre los activos.  
📉 **Dendrograma de Clustering Jerárquico** → Visualización de los grupos de activos.  
📊 **Silhouette Score** → Gráfico que ayuda a determinar el número óptimo de clusters.  
📈 **Frontera Eficiente** → Muestra la relación entre riesgo y retorno para diferentes combinaciones de activos.  
📉 **Evolución histórica del portafolio** → Visualiza el crecimiento del valor del portafolio a lo largo del tiempo.  
