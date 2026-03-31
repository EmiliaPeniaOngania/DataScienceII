# DataScienceII

# Modelo de Riesgo Crediticio Bancario- BCRA

Modelo Predictivo de Riesgo Crediticio Bancario

## Descripción

Este proyecto desarrolla un modelo de análisis y proyección del riesgo crediticio en entidades financieras del sistema argentino, utilizando datos públicos del BCRA y variables macroeconómicas.

El enfoque combina análisis descriptivo, construcción de indicadores financieros y un modelo de machine learning para anticipar la evolución del riesgo.


## Objetivo

- Evaluar el riesgo crediticio de bancos
- Analizar la calidad de cartera
- Proyectar la evolución futura del riesgo (t+1)
- Permitir el análisis individual y comparativo mediante selección de uno o múltiples entidades financieras,
- Generar una herramienta de apoyo para la toma de decisiones

## Datos utilizados

- 📊 Balance resumido de entidades financieras (bcra.gob.ar)
- 📉 Estado de situación de deudores (bcra.gob.ar)
- 📈 Indicadores financieros (ROE, ROA, liquidez, etc.) (bcra.gob.ar)
- 🌐 API de actividad económica (datos.gob.ar)


## Metodología

- Integración de múltiples tablas del BCRA
- Limpieza y normalización de datos
- Corrección de encoding
- Generación de dataset unificado
- Se construyen indicadores clave:

      - Ratio de cartera irregular
      - Cartera / Activo
      - Previsiones / Préstamos
      - Irregular / Patrimonio
- Se implementa un modelo predictivo de Machine Learning:
      - Algoritmo: Random Forest
      - Enfoque temporal: predicción t+1
      - Target: ratio de cartera irregular futuro
- Selección dinamica de una o multiples entidades financieras para análisis comparativo

## El modelo permite:

- Predecir el ratio futuro
- Detectar deterioro o mejora
- Clasificar riesgo en niveles

## Output del modelo

Para cada banco se obtiene:

- Ratio actual
- Ratio proyectado
- Variación esperada
- Nivel de riesgo:
  - 🟢 Bajo
  - 🟡 Medio
  - 🔴 Alto
- Tendencia:
  - Mejora
  - Estable
  - Empeora

##  Análisis realizado

El proyecto incluye:

- Evolución temporal del riesgo
- Ranking de bancos
- Composición de cartera (normal vs irregular)
- Comparación contra sistema financiero
- Vista ejecutiva por entidad

##  Persistencia de datos

- Exportación de dataset a MySQL
- Generación de tabla de scoring del modelo
- Inclusión de fecha de carga

##  Visualización

- Gráficos en Python (matplotlib / seaborn)
- Integración posible con Power BI

##  Próximas mejoras

- Dashboard en Power BI

##  Conclusión

El modelo desarrollado permite anticipar la evolución del riesgo crediticio en entidades financieras, funcionando como una herramienta de alerta temprana y análisis estratégico.

