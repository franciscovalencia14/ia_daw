# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA

## 1) Caso y objetivo de negocio
- Empresa/sector (real o ficticia): Amazon — sector retail y marketplace global.
- Problema a resolver: Optimizar la gestión de inventario y aumentar la conversión mediante recomendaciones personalizadas, reduciendo roturas de stock y costes logísticos
- Objetivo de negocio (rentabilidad): Aumentar ventas por usuario y reducir costes operativos mediante el uso de Big Data e Inteligencia Artificial aplicada a recomendación y predicción de demanda.

## 2) Big Data: recogida masiva de datos
Describe por qué es Big Data (volumen, velocidad, variedad).
-Volumen:Millones de pedidos diarios y miles de millones de eventos de navegación.
-Velocidad:Procesamiento en tiempo real (clics, búsquedas, compras).
-Variedad:Datos estructurados (ventas), semiestructurados (logs JSON), no estructurados (reseñas en texto libre).
- Fuente 1:Historial de navegación y compras de usuarios.
- Fuente 2:Datos logísticos (inventario, tiempos de envío, devoluciones).
- Fuente 3:Reseñas y valoraciones de productos (texto libre).
- Volumen/velocidad (estimación):Millones de transacciones diarias procesadas en segundos mediante sistemas distribuidos.
- Formatos (texto, eventos, series temporales, imágenes, etc.):Tablas relacionales, JSON, logs de eventos, texto (NLP), series temporales de demanda.

## 3) Tratamiento/análisis: pipeline de datos
Explica el flujo de forma ordenada:
- Ingesta (captura/eventos):Captura en tiempo real desde web, app móvil y sistemas logísticos mediante eventos de usuario y transacciones.
- Limpieza/normalización:Eliminación de duplicados, corrección de errores, normalización de categorías, monedas y precios.
- Almacenamiento (data lake/warehouse):
  Data Lake: almacenamiento masivo de datos en bruto.
  Data Warehouse: datos estructurados para análisis y reporting.
- Preparación de variables (features):
Frecuencia de compra (RFM).
Ticket medio.
Tiempo medio de entrega.
Probabilidad de devolución.
Estacionalidad y tendencia de demanda.
- Análisis/BI (opcional):Dashboards de ventas, rotura de stock, eficiencia logística y margen por categoría.

## 4) IA aplicada: modelo y decisión
- Tipo de IA/técnica (clasificación, predicción, recomendación, anomalías, NLP...):Sistema de recomendación (filtrado colaborativo + modelo híbrido) y modelo predictivo de demanda (series temporales).
- Entrada del modelo (qué datos usa):Historial de compras, comportamiento de usuarios similares, ubicación geográfica, estacionalidad, stock disponible.
- Salida del modelo (qué produce):
Recomendaciones personalizadas de productos.
Predicción de demanda por región y categoría.
- Decisión que habilita (qué hace la empresa con esa salida):
Mostrar productos personalizados en la web.
Ajustar inventario automáticamente.
Optimizar precios dinámicos.

## 5) Rentabilidad: KPIs antes/después (mínimo 3)
KPI 1 (ingresos/coste/eficiencia):
- Antes:8%
- Después:11%
- Por qué mejora la rentabilidad:Mayor porcentaje de visitas se convierten en compras → incremento directo de ingresos.

KPI 2:
- Antes:6%
- Después:2%
- Por qué mejora la rentabilidad:Menos ventas perdidas y mayor satisfacción del cliente → fidelización.

KPI 3:
- Antes:6,5€
- Después:5,2€
- Por qué mejora la rentabilidad:Mejor predicción reduce transporte urgente y exceso de inventario.

## 6) Diagrama del pipeline (ASCII o Mermaid)
flowchart LR
A[Usuarios Web/App] --> B[Captura de Eventos]
B --> C[Data Lake]
C --> D[Limpieza y Transformación]
D --> E[Data Warehouse]
E --> F[Feature Engineering]
F --> G[Modelo IA]
G --> H[Recomendaciones + Predicción Demanda]
H --> I[Optimización Inventario]
I --> J[Mejora de KPIs]

## 7) Riesgos y mitigación
Riesgo 1:
- Mitigación 1:

Riesgo 2:
- Mitigación 2:

## 8) Valoración (criterio c): importancia presente y futura de la IA (10–15 líneas)
- Importancia actual (hoy):
- Importancia futura (3–5 años):
- Condiciones/limitaciones (datos, costes, regulación, ética, seguridad, empleo):
- Conclusión razonada:

## 9) Fuentes oficiales (mín. 2)
- Big Data/analítica (enlace oficial):
- IA/técnica/modelo (enlace oficial):
