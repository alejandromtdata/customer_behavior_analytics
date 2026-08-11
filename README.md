# Customer Behavior Analytics

## Descripción del proyecto

Este proyecto analiza el comportamiento de los usuarios de una plataforma digital basada en suscripción utilizando Python y técnicas de análisis exploratorio de datos (EDA).

El objetivo es entender cómo interactúan los usuarios con la plataforma, cómo evoluciona su actividad, cómo se generan los ingresos y cómo cambia la retención de los usuarios a lo largo del tiempo.

El proyecto sigue un flujo completo de análisis de datos, desde la exploración inicial de los datasets hasta el cálculo de métricas, el análisis de ingresos, el estudio del churn y la retención mediante cohortes y la obtención de conclusiones de negocio.

---

## Preguntas de negocio

Durante el análisis se plantean diferentes preguntas relacionadas con el comportamiento de los usuarios:

- ¿Cuántos usuarios utilizan activamente la plataforma?
- ¿Cómo varía el nivel de actividad entre los usuarios?
- ¿Cómo se distribuyen los ingresos entre los usuarios y las transacciones?
- ¿Qué porcentaje de usuarios abandona la plataforma?
- ¿Cómo evoluciona la retención después del registro?
- ¿Existen diferencias de comportamiento entre las distintas cohortes?
- ¿Qué relación existe entre actividad, retención y generación de ingresos?

---

## Dataset

El proyecto utiliza cuatro datasets relacionados entre sí:

| Dataset | Descripción |
|---------|-------------|
| **users.csv** | Información de los usuarios, registro, plan, país y estado de churn |
| **sessions.csv** | Información sobre las sesiones y actividad de los usuarios |
| **transactions.csv** | Información sobre transacciones y generación de ingresos |
| **data_dictionary.csv** | Diccionario con la descripción de las columnas de los datasets |

---

## Tecnologías utilizadas

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**
- **VS Code**

---

## Habilidades aplicadas

Durante el proyecto se han aplicado diferentes técnicas y conceptos de análisis de datos:

- Exploratory Data Analysis (EDA)
- Limpieza y preparación de datos
- Análisis de métricas de usuarios
- Análisis de actividad y engagement
- Análisis de ingresos
- Análisis de churn
- Análisis de retención
- Cohort Analysis
- Data Visualization
- Obtención de insights de negocio

---

## Flujo del proyecto

### 1. Exploración inicial de los datos

En el primer notebook se realiza una exploración inicial de los datasets para conocer su estructura y detectar posibles problemas.

Se analizan aspectos como:

- Número de filas y columnas
- Tipos de datos
- Valores nulos
- Distribución de variables
- Distribución de usuarios por diferentes características
- Evolución de los registros de usuarios

**Notebook:** `01_eda_baseline.ipynb`

---

### 2. Análisis de métricas de usuarios

En este notebook se analizan diferentes métricas relacionadas con la actividad de los usuarios y el uso de la plataforma.

Se estudian aspectos como:

- Número de sesiones por usuario
- Distribución de la actividad
- Sesiones según el plan
- Duración de las sesiones
- Evolución de la actividad diaria

**Notebook:** `02_user_metrics.ipynb`

---

### 3. Análisis de ingresos

En esta parte se analiza la información relacionada con las transacciones y la generación de ingresos.

El análisis permite estudiar:

- Distribución de ingresos
- Ingresos generados por usuario
- Evolución de los ingresos a lo largo del tiempo
- Comportamiento de las transacciones

**Notebook:** `03_revenue_analysis.ipynb`

---

### 4. Análisis de churn y retención mediante cohortes

En esta parte se analiza el comportamiento de los usuarios después de su registro.

Los usuarios se agrupan en cohortes según su mes de registro y se analiza su actividad durante los meses posteriores.

Para ello se calcula:

- Mes de registro de cada usuario
- Mes de cada sesión
- Meses transcurridos desde el registro
- Usuarios activos por cohorte y mes
- Retención de cada cohorte

Finalmente se utiliza un mapa de calor para visualizar la evolución de la retención a lo largo del tiempo.

**Notebook:** `04_cohort_retention.ipynb`

---

### 5. Insights y conclusiones

El último notebook resume los principales resultados obtenidos durante el análisis.

Se recogen los principales patrones observados en:

- Actividad de los usuarios
- Engagement
- Ingresos
- Churn
- Retención
- Comportamiento de las diferentes cohortes

También se plantean algunas posibles líneas de actuación y análisis futuros a partir de los resultados obtenidos.

**Notebook:** `05_insights_conclusions.ipynb`

---

## Principales insights

El análisis permite observar varios patrones relevantes en el comportamiento de los usuarios:

- Los usuarios presentan niveles de actividad muy diferentes.
- La actividad de los usuarios no está distribuida de forma uniforme.
- La generación de ingresos tampoco está repartida de la misma manera entre todos los usuarios.
- Existe una parte de usuarios que abandona la plataforma.
- La retención disminuye conforme aumenta el tiempo desde el registro.
- La mayor pérdida de usuarios se concentra durante los primeros meses.
- Las diferentes cohortes presentan algunas diferencias en sus niveles de retención.
- El análisis conjunto de actividad, retención e ingresos permite obtener una visión más completa del comportamiento de los usuarios.

---

## Recomendaciones

A partir de los resultados obtenidos, se plantean algunas posibles líneas de actuación:

- Mejorar el proceso de onboarding para facilitar los primeros pasos de los nuevos usuarios.
- Analizar con mayor detalle las causas del abandono durante los primeros meses.
- Fomentar el uso recurrente de las principales funcionalidades de la plataforma.
- Estudiar las características de los usuarios con mayor nivel de actividad y valor económico.
- Analizar posibles estrategias para mejorar la retención de los usuarios con menor actividad.

Estas recomendaciones deben considerarse como puntos de partida para futuros análisis y no como conclusiones causales definitivas.

---

## Estructura del repositorio

customer_behavior_analytics/
│
├── data/
├── docs/
├── notebooks/
│   ├── 01_eda_baseline.ipynb
│   ├── 02_user_metrics.ipynb
│   ├── 03_revenue_analysis.ipynb
│   ├── 04_cohort_retention.ipynb
│   └── 05_insights_conclusions.ipynb
│
├── reports/
├── src/
├── tests/
│
├── .gitignore
├── .python-version
├── main.py
├── pyproject.toml
├── README.md
├── requirements.txt
└── uv.lock