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
- **Registros finales**: 14.560 películas (después de limpieza)

### Columnas del Dataset
- **Título pelicula**: Nombre de la película
- **Sinopsis**: Descripción de la película
- **Clasificación edad**: Rating de edad (G, PG, PG-13, R, NR)
- **Géneros**: Género principal de la película
- **Directores**: Director principal
- **Guionistas**: Guionista principal
- **Actores**: Dos actores principales
- **Fecha estreno original**: Fecha de estreno inicial
- **Fecha estreno streaming**: Fecha de estreno en streaming
- **Duración**: Duración en minutos
- **Productora**: Casa productora
- **Estado**: Estado en Rotten Tomatoes (Fresh, Rotten, Certified-Fresh)
- **Valoración criticos**: Puntuación de críticos (0-100)
- **Número críticas**: Número de reseñas de críticos
- **Valoración audiencia**: Puntuación de audiencia (0-100)
- **Número valoraciones audiencia**: Número de valoraciones de audiencia

## 🔧 Proceso de Limpieza de Datos

### Transformaciones Realizadas

1. **Traducción de columnas** al español para mejorar la comprensión
2. **Eliminación de columnas irrelevantes**:
   - `rotten_tomatoes_link`
   - `Consenso críticos` (48% valores nulos)
   - `Estado audiencia`
   - `Número top criticos`
   - `Número criticas favorables`
   - `Número criticas negativas`

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
- Duración: 1.77%
- Valoración audiencia: 1.67%

## 📈 Estructura de Dashboards

### 1. Dashboard de Introducción 📊
- **KPIs principales**: 
  - Número total de películas
  - Géneros únicos
  - Número de productoras
  - Duración media de las películas
  - Valoración promedio crítica
  - Valoración promedio audiencia
- **Visualizaciones**:
  - Distribución de las películas por género
  - Análisis por clasificación de edad

### 2. Dashboard de Evolución Temporal ⏰
- **Análisis cronológico**:
  - Número de estrenos por año.
  - Evolución de géneros a lo largo del tiempo.

### 3. Dashboard de Películas 🎭
- **Análisis de valoraciones**:
  - Comparación valoración críticos vs. audiencia.
  - Identificación de películas mejor valoradas de las 4 etapas cinematográficas.

### 4. Dashboard de Productoras 🏢
- **Análisis empresarial**:
  - Evolución de las productoras con mayor número de películas y valoraciones promedio obtenidas a lo largo de la historia.
  - Ubicación geográfica de las productoras principales.

### 5. Dashboard de Artistas 🏢
- **Análisis talento**:
  - Ranking de los directores y guionistas mejor valorados a lo largo de la historia.
  - Top 3 de actores en la epoca actual según su popularidad y según las valoraciones obtenidas.
 
### 6. Dashboard de Géneros 🎭
- **Análisis talento**:
  - Top 4 de los géneros más populares y sus valoraciones medias.
    
### 7. Dashboard de Conclusiones 🏆
- Insights clave.
- Desvelamineto de la película elaborada.

## 🛠️ Tecnologías Utilizadas

- **Python 3.12.7**
- **Pandas**: Manipulación y análisis de datos
- **NumPy**: Operaciones numéricas
- **Jupyter Notebook**: Desarrollo y documentación
- **Power BI**: Visualización de datos (dashboards)

## 👥 Equipo de Trabajo

| Responsable | Dashboard |
|-------------|-----------|
| **Laura** | Introducción y análisis general |
| **Lara**  | Evolución temporal y análisis de las valoraciones | 
| **Lucía** | Análisis de las productoras |
| **Auris** | Análisis de talento y preferencias de audiencia |

## 🎬 Reflexión Final

> *"En el mundo del cine, los datos no mienten. Cada película cuenta una historia, pero los números revelan el secreto de por qué algunas historias perduran en el tiempo y otras se desvanecen en el olvido."*

Este análisis representa el primer paso en nuestro viaje para crear una película que no solo entretenga, sino que también deje una marca indeleble en la historia del cine. Los datos son nuestro mapa, pero la creatividad sigue siendo nuestro destino.

**CineLab Studios** - *Donde los datos encuentran la creatividad*
