EL orden de este Readme segun el contenido de codigo viene dado por TLC sigue CCD Flat Fields para la segunda aprte y para la tercer parte Distribución, curva y Mapeo
# Teorema del Límite Central aplicado a distribuciones de Poisson

## Descripción del proyecto

Este proyecto implementa una simulación numérica del Teorema del Límite Central (TLC) utilizando muestras aleatorias extraídas de una distribución discreta de Poisson. A través de métodos computacionales y visualización estadística, se estudia cómo la distribución de las medias muestrales converge progresivamente hacia una distribución normal conforme aumenta el tamaño de muestra.

El notebook desarrolla una exploración práctica del comportamiento asintótico del TLC, evaluando la relación entre el tamaño muestral, la forma de la distribución subyacente y la aproximación gaussiana resultante.

Además, se estudian propiedades estadísticas como:

* media,
* mediana,
* desviación estándar,
* comportamiento de histogramas,
* técnicas óptimas de binning,
* convergencia estadística,
* ajuste gaussiano.

La simulación utiliza poblaciones sintéticas generadas mediante procesos de Poisson, permitiendo analizar experimentalmente uno de los teoremas fundamentales de la estadística y la teoría de probabilidad.

---

## Objetivo académico y científico

El objetivo principal de este proyecto es demostrar computacionalmente el funcionamiento del Teorema del Límite Central mediante simulaciones Monte Carlo sobre distribuciones de Poisson.

Se busca:

* analizar cómo las medias muestrales convergen hacia una distribución normal,
* estudiar la dependencia de la convergencia con el tamaño muestral,
* explorar las condiciones de aplicabilidad del TLC,
* comparar estadísticos descriptivos durante el proceso de convergencia,
* visualizar experimentalmente propiedades teóricas de inferencia estadística.

El proyecto fue desarrollado como parte de ejercicios académicos de astroestadística y métodos estadísticos aplicados a física y astronomía.

---

## Tecnologías utilizadas

* Python
* NumPy
* SciPy
* Matplotlib
* Seaborn
* tqdm
* Jupyter Notebook

---

## Contenido del notebook

El notebook incluye:

### 1. Generación de poblaciones Poissonianas

* Simulación de variables aleatorias discretas.
* Control del parámetro λ.
* Construcción de poblaciones sintéticas grandes.

### 2. Simulación de medias muestrales

* Extracción aleatoria de muestras.
* Cálculo iterativo de:

  * medias,
  * medianas,
  * desviaciones estándar.

### 3. Verificación experimental del TLC

* Histogramas dinámicos.
* Ajustes gaussianos.
* Comparación visual entre distribuciones.

### 4. Técnicas de binning

* Regla de Scott.
* Análisis del ancho óptimo de bins.
* Visualización estadística robusta.

### 5. Estudio de convergencia

* Comparación entre media y mediana.
* Evaluación numérica de aproximación gaussiana.
* Dependencia con el tamaño de muestra.

---

## Resultados principales

Los resultados muestran que:

* incluso distribuciones discretas y no gaussianas como Poisson convergen hacia una distribución normal en las medias muestrales,
* la convergencia depende del tamaño de muestra y de la forma original de la distribución,
* tamaños muestrales relativamente pequeños pueden producir aproximaciones gaussianas razonables,
* las técnicas adecuadas de binning son importantes para interpretar correctamente histogramas estadísticos.

---

## Requerimientos

Instalar dependencias:

```bash
pip install numpy scipy matplotlib seaborn tqdm
```

---

## Ejecución

Abrir el notebook en Jupyter:

```bash
jupyter notebook
```

y ejecutar las celdas secuencialmente.

---

## Contexto académico

Proyecto desarrollado en cursos de:

* Astroestadística
* Métodos computacionales
* Probabilidad y estadística aplicada

Aplicado a problemas de simulación numérica en física y astronomía.


# Análisis estadístico de Flat Fields CCD

## Descripción del proyecto

Este proyecto desarrolla un análisis estadístico completo sobre imágenes astronómicas tipo flat-field obtenidas mediante detectores CCD. El objetivo es estudiar la distribución de intensidades de píxeles y caracterizar estadísticamente el comportamiento de los datos utilizando herramientas de inferencia estadística y teoría de estimadores.

El notebook implementa:

* cálculo de momentos estadísticos,
* análisis de skewness y curtosis,
* histogramas normalizados,
* selección óptima de bins,
* intervalos de confianza,
* comparación de estimadores,
* análisis de consistencia y sesgo,
* pruebas de hipótesis sobre imágenes CCD.

El trabajo combina estadística matemática, programación científica y análisis de datos astronómicos reales.

---

## Objetivo académico y científico

El proyecto busca aplicar herramientas de astroestadística al análisis de imágenes CCD astronómicas.

Los objetivos incluyen:

* caracterizar distribuciones de intensidad de píxeles,
* inferir propiedades estadísticas de imágenes flat-field,
* construir intervalos de confianza sin asumir distribuciones analíticas,
* comparar estimadores estadísticos,
* evaluar consistencia, sesgo y varianza,
* implementar pruebas de hipótesis entre datasets astronómicos.

---

## Tecnologías utilizadas

* Python
* NumPy
* SciPy
* Pandas
* Matplotlib
* Jupyter Notebook
* gdown

---

## Contenido del notebook

### 1. Lectura y procesamiento de datos CCD

* Importación de archivos `.pix.gz`
* Manejo de datos astronómicos
* Extracción de intensidades y coordenadas

### 2. Cálculo de momentos estadísticos

* Media
* Varianza
* Skewness
* Curtosis
* Estimadores sesgados e insesgados

### 3. Inferencia estadística

* Interpretación física de momentos
* Análisis de simetría
* Comportamiento asintótico de colas

### 4. Histogramas y densidades

* Histogramas normalizados
* Técnicas de binning:

  * Scott
  * Sturges
  * Rice
* Evaluación mediante MISE

### 5. Intervalos de confianza

* Construcción empírica usando CDF
* Nivel de confianza del 90%
* Métodos no paramétricos

### 6. Estudio de estimadores

* Consistencia
* Bias
* Varianza
* Comparación entre estimadores

### 7. Pruebas de hipótesis

* Test Z
* Test t de Student
* Comparación entre flat-fields
* Validación estadística de observaciones astronómicas

---

## Resultados principales

El análisis muestra:

* distribuciones no gaussianas en intensidades CCD,
* presencia de asimetría y curtosis elevada,
* diferencias entre estimadores estadísticos,
* consistencia de métodos inferenciales aplicados a datos astronómicos reales,
* aplicación efectiva de pruebas estadísticas para clasificación de imágenes.

---

## Requerimientos

```bash
pip install numpy scipy pandas matplotlib gdown
```

---

## Ejecución

Ejecutar el notebook en Jupyter Notebook o Google Colab.

---

## Contexto académico

Proyecto desarrollado para cursos de:

* Astroestadística
* Análisis de datos astronómicos
* Inferencia estadística
* Métodos computacionales en astronomía

# Inferencia Bayesiana aplicada a curvas de rotación galáctica

## Descripción del proyecto

Este proyecto implementa métodos de inferencia bayesiana aplicados al estudio de curvas de rotación galáctica. Utilizando datos observacionales y modelos físicos para componentes de disco y halo de materia oscura, se estiman distribuciones posteriores y probabilidades marginalizadas para parámetros astrofísicos relevantes.

El notebook desarrolla:

* modelado dinámico galáctico,
* funciones de likelihood,
* inferencia bayesiana,
* integración Monte Carlo,
* marginalización de parámetros,
* análisis probabilístico de parámetros físicos.

---

## Objetivo académico y científico

El objetivo principal es aplicar técnicas estadísticas bayesianas al modelado de curvas de rotación galáctica y estudiar la estimación probabilística de parámetros físicos asociados al disco galáctico y al halo de materia oscura.

Se busca:

* construir funciones posteriores,
* estimar parámetros físicos,
* obtener distribuciones marginalizadas,
* analizar incertidumbres,
* aplicar integración numérica Monte Carlo en astrofísica.

---

## Tecnologías utilizadas

* Python
* NumPy
* SciPy
* Pandas
* Matplotlib
* tqdm
* Google Colab

---

## Contenido del notebook

### 1. Lectura de datos observacionales

* Curvas de rotación
* Errores experimentales
* Procesamiento de datos astronómicos

### 2. Modelado físico

* Componentes de disco galáctico
* Halo de materia oscura
* Velocidad circular

### 3. Inferencia Bayesiana

* Construcción de likelihood
* Distribuciones posteriores
* Evaluación probabilística

### 4. Marginalización numérica

* Integración Monte Carlo
* Parámetros:

  * masa del disco,
  * masa del halo,
  * radio de escala.

### 5. Visualización estadística

* Distribuciones marginales
* Comparación de probabilidades
* Análisis de incertidumbre

---

## Resultados principales

El notebook permite:

* estimar parámetros físicos galácticos,
* visualizar distribuciones posteriores,
* estudiar incertidumbres bayesianas,
* aplicar métodos computacionales modernos en astrofísica observacional.

---

## Requerimientos

```bash
pip install numpy scipy pandas matplotlib tqdm
```

---

## Contexto académico

Proyecto desarrollado en cursos de:

* Astroestadística
* Dinámica galáctica
* Métodos bayesianos
* Astrofísica computacional

