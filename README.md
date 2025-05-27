# Análisis de Datos en el Mercado de Cartas Magic: The Gathering

Este proyecto tiene como objetivo analizar el mercado secundario de cartas de *Magic: The Gathering* en **Cardmarket**, para identificar oportunidades de mejora en la estrategia de precios, gestión de inventario y toma de decisiones comerciales.

El análisis se centra en comparar precios propios frente a la competencia, evaluar el nivel de saturación del mercado por carta, estimar márgenes potenciales y estudiar el estado físico del inventario.

---

## 📌 Objetivos del proyecto

- Detectar cartas infravaloradas respecto a la competencia.
- Identificar cartas con baja competencia en el mercado.
- Estimar márgenes potenciales de beneficio por carta.
- Analizar la calidad del inventario (condición de las cartas).
- Diseñar un dashboard interactivo de fácil uso para monitorizar el stock y actuar estratégicamente.

---

## 🧪 Proceso del proyecto

### 1. **Web Scraping**
- Utilicé **Selenium en Python** para automatizar la extracción de datos desde Cardmarket.
- Se recolectaron datos de:
  - Precio por carta
  - Vendedor
  - Idioma
  - Condición
  - Edición
  - Número de copias
  - Nombre de la carta

### 2. **Limpieza y transformación (ETL)**
- Usé **Pandas** para:
  - Eliminar duplicados y vacíos
  - Normalizar textos (condiciones, idiomas, nombres de ediciones)
  - Convertir precios a tipo numérico
  - Crear métricas derivadas como:
    - Precio medio de la competencia por carta
    - Diferencia frente a la competencia
    - Margen total estimado
    - Nivel de competencia (nº de vendedores)

### 3. **Análisis exploratorio (EDA)**
- Se exploraron distribuciones de precios y condiciones.
- Se identificaron cartas outlier en precio o competencia.
- Se aplicaron filtros por edición, idioma y condición para observar patrones.

### 4. **Diseño de dashboard interactivo (Tableau)**
- Se creó un dashboard con:
  - KPIs superiores
  - Gráficos de diferencia de precio, margen potencial y competencia
  - Distribución por condición y edición
  - Filtros aplicables a todo el dashboard: edición, vendedor, idioma, condición, precio

---

## 🛠️ Herramientas utilizadas

- **Python** (Selenium, Pandas)
- **Tableau**
- **Excel** (para revisión previa y formateo)
- **Markdown / GitHub** (para documentación)

---

## 📊 Estructura del Dashboard

1. **KPIs principales**:
   - Valor total en venta
   - % de cartas infravaloradas
   - Nº de cartas con poca competencia

2. **Gráficos clave**:
   - Cartas infravaloradas frente a la competencia
   - Distribución por nivel de competencia
   - Márgenes potenciales por carta
   - Condición de las cartas por edición

3. **Controles interactivos**:
   - Edición
   - Nombre del vendedor
   - Idioma
   - Condición
   - Precio (rango)

---

## 📈 Resultados clave

- El **9,92%** de las cartas están vendiéndose por debajo de la media del mercado.
- Más de **1.100 cartas** están en situación de baja competencia (≤ 3 vendedores).
- Se detectaron cartas con márgenes potenciales altos si se ajustaran los precios al nivel del mercado.
- Las condiciones de cartas varían significativamente según edición, afectando su valor.

---

## 🚀 Próximos pasos

- Automatizar la actualización del scraping de Cardmarket periódicamente.
- Incorporar una base de datos histórica para análisis temporal.
- Añadir alertas dinámicas para precios por debajo del umbral competitivo.
- Estimar márgenes reales incluyendo comisiones y gastos de envío.

---

## 👨‍💻 Autor

Luis Jiménez  
Bootcamp Data Analytics  - Hack(io)

