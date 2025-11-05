# Modelos de Business Intelligence - Predicción con Machine Learning

Este repositorio contiene dos proyectos de predicción usando Machine Learning y Regresión Lineal.

---

## 🥇 Proyecto Principal: Predicción del Precio del Oro

### Descripción

Sistema de **predicción del precio del oro** utilizando datos REALES de Yahoo Finance y técnicas de Machine Learning. Permite predecir el precio del oro para el próximo lunes y verificar la precisión de la predicción.

### Problema Real

**¿Cuál será el precio del oro el próximo lunes? ¿Vale la pena invertir ahora?**

Los inversionistas necesitan saber si el precio del oro va a subir o bajar para tomar decisiones informadas de compra/venta. Este proyecto proporciona predicciones basadas en datos históricos reales y verificables.

### ✅ Ventajas de Este Proyecto

- **Datos REALES**: Descarga automática desde Yahoo Finance
- **Verificable**: Puedes comprobar el lunes si acertó
- **Actualizado**: Datos hasta el día actual
- **Profesional**: Análisis completo con múltiples métricas
- **Sin costos**: API gratuita sin límites

---

## 📊 Proyecto Alternativo: Predicción de Tendencias de Hashtags

### Descripción

Sistema de **predicción de tendencias de hashtags** utilizando técnicas de Machine Learning (Regresión Lineal) para ayudar a marcas y creadores de contenido a identificar qué hashtags van a explotar en popularidad.

### Problema Real

**¿Cuál hashtag va a explotar la próxima semana? ¿Vale la pena invertir contenido ahí?**

Las marcas necesitan saber en qué hashtags invertir su tiempo y recursos ANTES que la competencia. Este proyecto proporciona predicciones basadas en datos para tomar decisiones estratégicas.

**Nota**: Este proyecto usa datos sintéticos (simulados) para demostración.

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

---

## 📁 Estructura del Proyecto

```
ModeloBIteoriaexamen3/
├── prediccion_oro.ipynb         # 🥇 Proyecto principal - Predicción precio del oro
├── prediccion_hashtags.ipynb    # 📊 Proyecto alternativo - Tendencias hashtags
└── README.md                     # Este archivo
```

---

# 🥇 PROYECTO PRINCIPAL: Predicción del Precio del Oro

## Características

### 1. Datos Reales en Tiempo Real
- Descarga automática desde **Yahoo Finance**
- Símbolo: **GC=F** (Gold Futures)
- Período: Últimos 6 meses hasta HOY
- Sin necesidad de API keys

### 2. Análisis Completo
- **Exploración de Datos**: Precio, volumen, retornos
- **Medias Móviles**: 7 y 30 días
- **Volatilidad**: Análisis de riesgo
- **Tendencias**: Corto, medio y largo plazo

### 3. Modelo de Machine Learning
- **Algoritmo**: Regresión Lineal
- **Características**: 8 variables predictoras
- **Métricas**: R², RMSE, MAE
- **Validación**: Split 80-20

### 4. Predicción Verificable
- Predice precio del **próximo lunes**
- Predicciones para 7 días futuros
- Dashboard visual completo
- **¡Puedes verificar el lunes si acertó!**

### 5. Análisis de Factores
- Inflación y tasas de interés
- Valor del dólar
- Incertidumbre geopolítica
- Oferta y demanda

## Contenido del Notebook de Oro

1. **Instalación e Importación** de librerías
2. **Descarga de Datos Reales** con yfinance
3. **Exploración de Datos (EDA)** con visualizaciones
4. **Preparación de Datos** (medias móviles, volatilidad)
5. **Modelo de Regresión Lineal** con evaluación
6. **🎯 PREDICCIÓN PARA EL LUNES** ← LO MÁS IMPORTANTE
7. **Análisis de Tendencias** (7, 30, 90 días)
8. **Factores que Afectan el Oro**
9. **Dashboard Resumen** visual completo
10. **Resumen y Recomendaciones**
11. **Guardar Predicción** para verificación

## Cómo Usar el Proyecto del Oro

### 1. Instalar dependencias

```bash
pip install yfinance pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 2. Ejecutar el notebook

```bash
jupyter notebook prediccion_oro.ipynb
```

### 3. Ejecutar todas las celdas

El notebook descargará automáticamente los datos más recientes y generará la predicción para el próximo lunes.

### 4. Verificar el lunes

Guarda la predicción y el lunes compara con el precio real en:
- [Yahoo Finance - Gold](https://finance.yahoo.com/quote/GC=F/)
- [Investing.com - Gold](https://www.investing.com/commodities/gold)

## Resultados que Obtendrás

### Predicción del Lunes
```
🎯 PRECIO PREDICHO PARA EL LUNES: $2,XXX.XX USD
📈 Tendencia: SUBIDA/BAJADA
✅ Recomendación: COMPRAR/VENDER/ESPERAR
```

### Métricas del Modelo
- **R² Score**: Qué tan bien predice (0-1, mejor cerca de 1)
- **RMSE**: Error promedio en dólares
- **MAE**: Error absoluto medio

### Visualizaciones
- Evolución histórica del precio
- Predicción vs datos reales
- Medias móviles
- Distribución de retornos
- Tendencias por período
- Dashboard completo

## Ejemplo de Uso Real

**Caso práctico del lunes:**

1. **Hoy (antes del lunes)**:
   - Ejecutas el notebook
   - Obtienes predicción: "$2,050.00 USD"
   - Recomendación: "COMPRAR (se espera subida del 1.5%)"

2. **El lunes**:
   - Revisas precio real del oro
   - Comparas con predicción
   - Calculas precisión del modelo

3. **Resultado**:
   - Si acertó dentro de $20-30: ¡Excelente modelo!
   - Si la tendencia fue correcta: Modelo útil para decisiones

## Por Qué Este Proyecto es Mejor para tu Examen

✅ **Datos Reales**: No son simulados, son del mercado real
✅ **Verificable**: El lunes puedes demostrar si funcionó
✅ **Profesional**: Análisis de nivel financiero
✅ **Sin Costos**: API gratuita
✅ **Actualizado**: Datos hasta hoy
✅ **Impactante**: Predecir el futuro impresiona más
✅ **Aplicable**: Se usa en el mundo real de inversiones

---

# 📊 PROYECTO ALTERNATIVO: Hashtags (Datos Sintéticos)

## Estructura del Proyecto (Hashtags)

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

---

## 🎓 Información del Proyecto

**Proyecto creado para**: Examen de Teoría - Modelos de Business Intelligence

**Objetivo**: Demostrar la aplicación práctica de Machine Learning en predicción de datos del mundo real

**Tecnologías**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, yfinance

## 📝 Notas Importantes

### Para el Proyecto del Oro (Principal):
- Los datos son **100% reales** descargados de Yahoo Finance
- La predicción es **verificable** el próximo lunes
- No requiere API keys ni costos
- Se actualiza automáticamente con los datos más recientes

### Para el Proyecto de Hashtags (Alternativo):
- Los datos son **sintéticos** (generados algorítmicamente)
- Útil para demostración de conceptos
- No verificable con datos reales

## 🚀 Recomendación

**Usa el proyecto del ORO (`prediccion_oro.ipynb`) para tu examen** porque:
1. Datos reales y actuales
2. Puedes verificar la predicción el lunes
3. Más profesional e impactante
4. Aplicación real en el mundo financiero

## 📚 Recursos Adicionales

- [Yahoo Finance API](https://finance.yahoo.com/)
- [yfinance Documentation](https://pypi.org/project/yfinance/)
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)

## Licencia

Este proyecto es de código abierto y está disponible para uso educativo y comercial.

---

**¡Buena suerte en tu examen! 🎓📊**
