# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA  

## 1) Caso y objetivo de negocio
- **Empresa/sector:** :contentReference[oaicite:0]{index=0} (retail y marketplace global).  
- **Problema a resolver:** Maximizar ventas por usuario y optimizar inventario reduciendo roturas de stock.  
- **Objetivo de negocio (rentabilidad):** Aumentar ingresos mediante recomendaciones personalizadas y reducir costes logísticos.

---

## 2) Big Data: recogida masiva de datos  

**Por qué es Big Data (3V):**  
- **Volumen:** Miles de millones de transacciones y eventos diarios a nivel mundial.  
- **Velocidad:** Datos generados en tiempo real (clics, compras, búsquedas, envíos).  
- **Variedad:** Datos estructurados (ventas), semiestructurados (logs), no estructurados (reseñas, voz).

- **Fuente 1:** Historial de navegación y compras.  
- **Fuente 2:** Datos logísticos (almacenes, envíos, devoluciones).  
- **Fuente 3:** Reseñas y valoraciones de productos (texto libre).  
- **Volumen/velocidad (estimación):** Millones de pedidos diarios; procesamiento en segundos.  
- **Formatos:** Tablas, JSON, texto (NLP), datos de sensores/logística.

---

## 3) Tratamiento/análisis: pipeline de datos  

- **Ingesta:** Captura en tiempo real desde web, app y centros logísticos.  
- **Limpieza/normalización:** Eliminación de duplicados, estandarización de categorías y precios.  
- **Almacenamiento:**  
  - Data Lake para datos masivos en bruto.  
  - Data Warehouse para métricas consolidadas.  
- **Feature Engineering:**  
  - Frecuencia de compra.  
  - Ticket medio.  
  - Tiempo de entrega medio.  
  - Probabilidad de devolución.  
- **Análisis/BI:** Paneles de control de ventas, logística y comportamiento cliente.

---

## 4) IA aplicada: modelo y decisión  

- **Tipo de IA/técnica:**  
  Sistema de recomendación basado en filtrado colaborativo y modelos de predicción de demanda.

- **Entrada del modelo:**  
  Historial de compras, comportamiento de usuarios similares, estacionalidad, ubicación geográfica.

- **Salida del modelo:**  
  - Productos recomendados personalizados.  
  - Predicción de demanda por región.  

- **Decisión que habilita:**  
  - Mostrar recomendaciones en la página principal.  
  - Ajustar inventario en almacenes automáticamente.  
  - Optimizar precios dinámicos.

---

## 5) Rentabilidad: KPIs antes/después  

### KPI 1: Tasa de conversión  
- **Antes:** 8%  
- **Después:** 11%  
- **Impacto:** Mayor porcentaje de visitas que terminan en compra → aumento directo de ingresos.

### KPI 2: Rotura de stock  
- **Antes:** 6% de productos clave sin disponibilidad.  
- **Después:** 2%.  
- **Impacto:** Menos ventas perdidas y mejor satisfacción del cliente.

### KPI 3: Coste logístico por pedido  
- **Antes:** 6,5 €  
- **Después:** 5,2 €  
- **Impacto:** Mejor predicción de demanda reduce transporte urgente y almacenamiento innecesario.

---

## 6) Diagrama del pipeline  

```mermaid
flowchart LR
A[Usuarios Web/App] --> B[Captura de Datos en Tiempo Real]
B --> C[Data Lake]
C --> D[Limpieza y Normalización]
D --> E[Data Warehouse]
E --> F[Modelo IA (Recomendación + Predicción)]
F --> G[Personalización Web + Gestión Inventario]
G --> H[Mejora KPIs]
