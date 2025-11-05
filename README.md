# Predicción de Tendencias de Hashtags

## Descripción del Proyecto

Este proyecto implementa un sistema de **predicción de tendencias de hashtags** utilizando técnicas de Machine Learning (Regresión Lineal) para ayudar a marcas y creadores de contenido a identificar qué hashtags van a explotar en popularidad.

## Problema Real

**¿Cuál hashtag va a explotar la próxima semana? ¿Vale la pena invertir contenido ahí?**

Las marcas necesitan saber en qué hashtags invertir su tiempo y recursos ANTES que la competencia. Este proyecto proporciona predicciones basadas en datos para tomar decisiones estratégicas.

## Características del Proyecto

### 1. Análisis de Datos
- Volumen de posts por hashtag por día
- Engagement promedio (likes, comments, shares)
- Relación con eventos del mundo real

### 2. Modelo Predictivo
- **Algoritmo**: Regresión Lineal
- **Objetivo**: Predecir volumen de posts para los próximos 7 días
- **Características**: día, día de la semana, eventos, engagement

### 3. Análisis de Tendencias
- Identificación de hashtags en crecimiento vs decrecimiento
- Cálculo de cambios porcentuales
- Visualizaciones interactivas

### 4. Impacto de Eventos
- Análisis de cómo eventos mundiales afectan hashtags
- Incremento de actividad durante eventos especiales
- Recomendaciones de timing para publicaciones

## Estructura del Proyecto

```
ModeloBIteoriaexamen3/
├── prediccion_hashtags.ipynb    # Notebook principal con análisis completo
└── README.md                     # Este archivo
```

## Requisitos

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Librerías necesarias:
- `pandas`: Manipulación de datos
- `numpy`: Operaciones numéricas
- `matplotlib`: Visualizaciones
- `seaborn`: Visualizaciones estadísticas
- `scikit-learn`: Modelo de Machine Learning
- `jupyter`: Para ejecutar notebooks

## Cómo Usar

### 1. Instalar dependencias

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 2. Ejecutar el notebook

```bash
jupyter notebook prediccion_hashtags.ipynb
```

### 3. Ejecutar todas las celdas

Puedes ejecutar todas las celdas desde el menú: `Cell > Run All`

## Contenido del Notebook

El notebook está organizado en las siguientes secciones:

1. **Importación de Librerías**
2. **Generación de Datos Sintéticos** (incluye 10 hashtags populares)
3. **Exploración de Datos (EDA)** con visualizaciones
4. **Preparación de Datos** para el modelo
5. **Modelo de Regresión Lineal** con evaluación
6. **Predicción de Tendencias** para los próximos 7 días
7. **Análisis de Tendencias** (hashtags subiendo vs bajando)
8. **Relación con Eventos** del mundo real
9. **Recomendaciones Estratégicas** para marcas
10. **Dashboard Resumen** visual
11. **Conclusiones** y próximos pasos

## Resultados Esperados

El notebook genera:

- Predicciones de volumen de posts para los próximos 7 días
- Identificación de hashtags con mayor potencial de crecimiento
- Análisis de impacto de eventos en popularidad de hashtags
- Recomendaciones estratégicas para marcas
- Múltiples visualizaciones y gráficos interactivos
- Dashboard resumen con métricas clave

## Métricas del Modelo

El modelo de regresión lineal incluye las siguientes métricas:

- **R² Score**: Mide qué tan bien el modelo explica la variabilidad
- **RMSE**: Error cuadrático medio
- **MAE**: Error absoluto medio

## Casos de Uso Real

### Para Marcas:
- Identificar hashtags emergentes antes que la competencia
- Optimizar calendario de contenido
- Aprovechar eventos para maximizar alcance
- Evitar inversión en hashtags en declive

### Para Creadores de Contenido:
- Saber qué hashtags usar en próximas publicaciones
- Timing óptimo para publicar contenido
- Anticiparse a tendencias virales

### Para Agencias de Marketing:
- Reportes de tendencias para clientes
- Estrategias data-driven
- ROI mejorado en campañas de redes sociales

## Datos

El proyecto actualmente utiliza **datos sintéticos** generados algorítmicamente que simulan:
- Tendencias crecientes y decrecientes
- Eventos del mundo real y su impacto
- Variabilidad natural del engagement

### Integración con Datos Reales

Para usar datos reales, puedes integrar APIs de:
- **Twitter API** (X API)
- **Instagram Graph API**
- **TikTok API**
- **YouTube Data API**

Simplemente reemplaza la sección de generación de datos sintéticos con llamadas a estas APIs.

## Próximos Pasos / Mejoras Futuras

1. Integrar datos reales de APIs de redes sociales
2. Añadir análisis de sentimiento a los posts
3. Implementar modelos más complejos (Random Forest, LSTM)
4. Crear dashboard web interactivo con Streamlit o Dash
5. Sistema de alertas automáticas para hashtags emergentes
6. Análisis geográfico de tendencias
7. Predicciones personalizadas por industria/nicho

## Impacto Real

Este tipo de análisis permite a las marcas:
- **Adelantarse a la competencia** identificando tendencias emergentes
- **Maximizar ROI** invirtiendo en los hashtags correctos
- **Optimizar recursos** evitando hashtags en declive
- **Aprovechar eventos** para aumentar visibilidad

## Autor

Proyecto creado como parte del examen de teoría - Modelo BI

## Licencia

Este proyecto es de código abierto y está disponible para uso educativo y comercial.

---

**Nota**: Este es un proyecto educativo que demuestra el poder del análisis de datos y Machine Learning aplicado a redes sociales. Los datos sintéticos generados son representativos pero no reflejan tendencias reales actuales.
