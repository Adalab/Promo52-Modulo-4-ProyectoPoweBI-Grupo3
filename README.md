# Promo52-Modulo-4-ProyectoPoweBI-Grupo3
# 🎬 CineLab Studios - Análisis Cinematográfico

## 📖 Historia del Proyecto

Estamos a punto de dar vida a una nueva película. Pero antes de rodar la primera escena, queremos entender qué hace que una historia conecte, emocione y triunfe.

Como **CineLab Studios**, nos sumergimos en los datos de Rotten Tomatoes para descubrir los ingredientes del éxito cinematográfico. Este análisis no solo es una mirada al pasado, sino una brújula creativa que guiará nuestras decisiones hacia una película que deje huella.

## 🎯 Objetivo

Analizar patrones de éxito en la industria cinematográfica mediante el estudio de datos históricos de Rotten Tomatoes, con el fin de identificar factores clave que contribuyen al éxito comercial y crítico de las películas.

## 📊 Dataset

### Fuente de Datos
- **Origen**: Rotten Tomatoes Movies Dataset
- **Registros iniciales**: 17,712 películas
- **Registros finales**: 14,156 películas (después de limpieza)

### Columnas del Dataset
- **Titulo pelicula**: Nombre de la película
- **Sinopsis**: Descripción de la película
- **Clasificacion edad**: Rating de edad (G, PG, PG-13, R, NR)
- **Generos**: Género principal de la película
- **Directores**: Director principal
- **Guionistas**: Guionista principal
- **Actores**: Dos actores principales
- **Fecha estreno original**: Fecha de estreno inicial
- **Fecha estreno streaming**: Fecha de estreno en streaming
- **Duracion**: Duración en minutos
- **Productora**: Casa productora
- **Estado**: Estado en Rotten Tomatoes (Fresh, Rotten, Certified-Fresh)
- **Valoracion criticos**: Puntuación de críticos (0-100)
- **Numero criticas**: Número de reseñas de críticos
- **Valoracion audiencia**: Puntuación de audiencia (0-100)
- **Numero valoraciones audiencia**: Número de valoraciones de audiencia

## 🔧 Proceso de Limpieza de Datos

### Transformaciones Realizadas

1. **Traducción de columnas** al español para mejor comprensión
2. **Eliminación de columnas irrelevantes**:
   - `rotten_tomatoes_link`
   - `Consenso criticos` (48% valores nulos)
   - `Estado audiencia`
   - `Numero top criticos`
   - `Numero criticas favorables`
   - `Numero criticas negativas`

3. **Limpieza de valores nulos**: Eliminación de filas con datos faltantes
4. **Simplificación de campos múltiples**:
   - Géneros: Se mantiene solo el género principal
   - Directores: Se mantiene solo el director principal
   - Guionistas: Se mantiene solo el guionista principal
   - Actores: Se mantienen solo los dos actores principales

### Estadísticas de Calidad de Datos

**Porcentaje de valores nulos por columna (antes de limpieza)**:
- Consenso críticos: 48.43%
- Guionistas: 8.71%
- Fecha estreno original: 6.58%
- Productora: 2.82%
- Estado audiencia: 2.53%
- Fecha estreno streaming: 2.17%
- Actores: 1.99%
- Sinopsis: 1.81%
- Duracion: 1.77%
- Valoracion audiencia: 1.67%

## 📈 Estructura de Dashboards

### 1. Dashboard de Introducción 📊
- **KPIs principales**: 
  - Número total de películas
  - Géneros únicos
  - Valoración promedio crítica
  - Valoración promedio audiencia
  - Total de críticas y valoraciones
- **Visualizaciones**:
  - Distribución por género
  - Análisis por clasificación de edad

### 2. Dashboard de Evolución Temporal ⏰
- **Análisis cronológico**:
  - Número de estrenos por año
  - Evolución de géneros a lo largo del tiempo
  - Tendencias en duración de películas
  - Patrones estacionales de lanzamientos

### 3. Dashboard de Participantes 🎭
- **Análisis de talento**:
  - Ranking de actores más frecuentes
  - Directores destacados por puntuaciones
  - Análisis de géneros preferidos
  - Comparación crítica vs. audiencia
  - Identificación de películas con mayor discrepancia de valoraciones

### 4. Dashboard de Productoras 🏢
- **Análisis empresarial**:
  - Ubicación geográfica de productoras
  - Tiempo entre producción y estreno
  - Selección de actores por productora
  - Especialización por tipo de película

### 5. Dashboard de Conclusiones 🏆
- Rankings finales
- Insights clave
- Recomendaciones estratégicas

## 🛠️ Tecnologías Utilizadas

- **Python 3.12.7**
- **Pandas**: Manipulación y análisis de datos
- **NumPy**: Operaciones numéricas
- **Jupyter Notebook**: Desarrollo y documentación
- **Power BI**: Visualización de datos (dashboards)

## 📁 Archivos del Proyecto

```
output/evaluacion_bi/
├── analisis_limpieza.ipynb              # Notebook principal de análisis
├── dashboard.txt                        # Especificaciones de dashboards
├── storytelling.txt                     # Contexto del proyecto
├── rotten_tomatoes_movies_limpio.csv    # Dataset procesado
├── directores.csv                       # Lista única de directores
└── README.md                           # Este archivo
```

## 🚀 Cómo Ejecutar el Análisis

### Prerrequisitos
```bash
pip install pandas numpy jupyter
```

### Pasos
1. **Abrir el notebook principal**:
   ```bash
   jupyter notebook analisis_limpieza.ipynb
   ```
2. **Ejecutar las celdas secuencialmente** para reproducir el análisis
3. **Importar `rotten_tomatoes_movies_limpio.csv`** en Power BI para crear dashboards

## 📊 Insights Preliminares

### Estadísticas Generales del Dataset Limpio
- **Total de películas analizadas**: 14,156
- **Duración promedio**: 102.2 minutos
- **Valoración críticos promedio**: 60.9/100
- **Valoración audiencia promedio**: 60.6/100
- **Rango temporal**: 1930 - presente

### Top Rankings
- **Director más prolífico**: Clint Eastwood (38 películas)
- **Guionista más activo**: Woody Allen (33 películas)
- **Clasificación más común**: R (6,377 películas - 36%)
- **Género predominante**: Drama (1,887 películas)
- **Productora líder**: Paramount Pictures (517 películas)

### Patrones Identificados
- **Correlación crítica-audiencia**: Las valoraciones muestran una correlación moderada
- **Variabilidad alta**: Ambas métricas cubren el rango completo (0-100)
- **Distribución por estado**: 
  - Rotten: ~43%
  - Fresh: ~35%
  - Certified-Fresh: ~22%

## 🎯 Próximos Pasos del Análisis

### Fase 2: Dashboards Interactivos
1. **Implementación en Power BI** de los 5 dashboards definidos
2. **Filtros interactivos** por año, género, productora
3. **Análisis comparativo** entre críticas y audiencia

### Fase 3: Análisis Avanzado
1. **Análisis predictivo** para identificar factores de éxito
2. **Segmentación de audiencias** por preferencias
3. **Análisis de tendencias temporales** detallado
4. **Correlaciones entre variables** (duración vs. valoración, etc.)

### Fase 4: Recomendaciones Estratégicas
1. **Perfil de película ideal** según datos históricos
2. **Estrategias de timing** para lanzamientos
3. **Identificación de nichos** de mercado
4. **Optimización de presupuestos** basada en ROI histórico

## 👥 Equipo de Trabajo

| Responsable | Dashboard | Enfoque Principal |
|-------------|-----------|-------------------|
| **Laura** | Introducción | KPIs generales y distribuciones básicas |
| **Auris** | Evolución Temporal | Tendencias históricas y patrones estacionales |
| **Lara** | Participantes | Análisis de talento y preferencias de audiencia |
| **Lucía** | Productoras | Estrategias empresariales y geografía |


## 🎬 Reflexión Final

> *"En el mundo del cine, los datos no mienten. Cada película cuenta una historia, pero los números revelan el secreto de por qué algunas historias perduran en el tiempo y otras se desvanecen en el olvido."*

Este análisis representa el primer paso en nuestro viaje para crear una película que no solo entretenga, sino que también deje una marca indeleble en la historia del cine. Los datos son nuestro mapa, pero la creatividad sigue siendo nuestro destino.

**CineLab Studios** - *Donde los datos encuentran la creatividad*

## 📞 Contacto

Para consultas sobre este análisis o colaboraciones futuras:
- **Proyecto**: Análisis Cinematográfico
- **Equipo**: CineLab Studios Data Analytics Team
- **Ubicación**: `output/evaluacion_bi/`
