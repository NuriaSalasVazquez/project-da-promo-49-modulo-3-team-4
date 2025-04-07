# Informe del Proyecto: Retención y Satisfacción Laboral en ABC Corporation

## 🎯 Objetivo del Proyecto

Con el objetivo de reducir la rotación de empleados y mejorar la satisfacción en el trabajo, la empresa **ABC Corporation** nos ha contratado para desarrollar un proyecto de análisis de datos. Nuestra misión es identificar los **factores clave** que influyen en la **satisfacción laboral** y, en última instancia, en la **retención de empleados**.

---

## 📊 Descripción General del Proyecto

- **Cliente**: ABC Corporation  
- **Equipo de trabajo**: 4ward Thinkers 
- **Duración estimada**: 18/03/2025 - 09/04/2025
- **Herramientas y tecnologías**: Python, Numpy, Pandas, Seaborn, Matplotlib

---

## 🗂️ Fuente y Preparación de Datos

### 1. Origen de los datos

DataFrame `hr_raw_data.csv`

- Age: Edad del empleado.

- Attrition: Indica si el empleado dejó la empresa (Yes/No).

- BusinessTravel: Frecuencia de viajes laborales (e.g., travel_rarely).

- DailyRate: Tarifa diaria estimada para clientes, calculada en base al salario.

- Department: Departamento en el que trabaja el empleado.

- DistanceFromHome: Distancia en millas o kilómetros desde el hogar al trabajo.

- Education: Nivel educativo del empleado en escala numérica.

- EducationField: Campo de estudio académico del empleado.

- employeecount: Valor constante de "1", indicando un solo empleado por registro.

- employeenumber: Número de identificación del empleado.

- EnvironmentSatisfaction: Nivel de satisfacción con el ambiente laboral.

- Gender: Género del empleado.

- HourlyRate: Tarifa por hora calculada.

- JobInvolvement: Nivel de compromiso del empleado en el trabajo.

- JobLevel: Nivel jerárquico del puesto del empleado.

- JobRole: Función o rol específico del empleado.

- JobSatisfaction: Satisfacción general en el puesto.

- MaritalStatus: Estado civil (e.g., Single, Married).

- MonthlyIncome: Ingreso mensual estimado en base al salario anual.

- MonthlyRate: Tarifa mensual estimada en función de la tarifa diaria.

- NUMCOMPANIESWORKED: Número de empresas previas en las que ha trabajado.

- OverTime: Indica si el empleado trabaja horas extras (Yes/No).

- PercentSalaryHike: Incremento porcentual en el salario.

- PerformanceRating: Evaluación de desempeño en una escala numérica.

- RelationshipSatisfaction: Satisfacción con relaciones interpersonales en el trabajo.

- StandardHours: Clasificación de jornada (Full Time/Part Time).

- StockOptionLevel: Nivel de opciones sobre acciones asignadas.

- TOTALWORKINGYEARS: Años totales de experiencia laboral.

- TrainingTimesLastYear: Número de sesiones de entrenamiento en el último año.

- WORKLIFEBALANCE: Nivel de balance entre vida personal y laboral.

- YearsAtCompany: Años en la empresa actual.

- YearsInCurrentRole: Años en el rol actual.

- YearsSinceLastPromotion: Años desde la última promoción recibida.

- YEARSWITHCURRMANAGER: Años trabajando con el mismo gerente.

- DateBirth: Año de nacimiento del empleado.

- Salary: Salario anual calculado para el empleado.

- RoleDepartament: Combinación de rol y departamento.

- NUMBERCHILDREN: Número de hijos del empleado (si está disponible).

- RemoteWork: Indica si el empleado trabaja de forma remota (Yes/No).

DataFrame `labor_force_participation_rate_by_age_group.csv`

- Fuente: https://data.ca.gov/dataset/labor-force-participation-rate-by-age-group/resource/d58bfa55-8f7f-438f-9e46-0cae78a80d91

### 2. Limpieza y preprocesamiento

- Unificación nombre columnas 
- Eliminación de valores nulos
- Codificación de variables categóricas
- Normalización / estandarización
- Detección de outliers
- Filtrado de columnas para el análisis

Para más detalles: https://docs.google.com/spreadsheets/d/1pLfwP7zJ8qAkEuVE2P4qM-kj6z-0E_emVTnwHtOpboE/edit?usp=sharing

---

## 🔍 Análisis Exploratorio de Datos (EDA)

- Distribución de variables clave (edad, antigüedad, departamento, salario, etc.)
- Análisis de correlaciones
- Visualización de insights relevantes (histogramas, gráficos de barras, gráficos de tarta, gráfico de líneas, gráfico de puntos)
- Comparativas entre empleados satisfechos y no satisfechos
- Clasificación de edad de los empleados en función de la generación (Baby Boomers, Gen X, Millennials, Gen Z)
- Comparativas centradas en género y edad 

---

## 🧠 Análisis Basado en Visualizaciones

### 1. Enfoque del análisis
Dado que el alcance inicial del proyecto se centra en **identificar patrones y factores clave** relacionados con la satisfacción y la rotación de empleados,  se optó por un enfoque exploratorio y descriptivo basado en visualizaciones y análisis de correlaciones. El análisis se centra en identificar patrones o tendencias por edad y por género dentro de ABC corporation con el objetivo de determinar si la igualdad es un factor clave de satisfacción en el trabajo.

### 2. Principales visualizaciones generadas
- Distribuciones de satisfacción laboral según departamento, edad, nivel de salario y género
- Identificación de roles menos satisfechos 
- Identificación de segmentos de edad con mayor riesgo de rotación o baja satisfacción
- Comparación de nivel salarial según género y edad 

### 3. Insights extraídos
- [Ejemplo: Los empleados con menos de 2 años en la empresa mostraron una mayor tasa de rotación]
- [Ejemplo: La satisfacción laboral tiene una fuerte relación con la percepción del salario y el equilibrio vida-trabajo]
- [Agrega aquí cualquier otro insight relevante del análisis]

---

## 📌 Conclusiones y Recomendaciones

- Principales hallazgos del análisis
- Recomendaciones para reducir la rotación
- Acciones sugeridas para mejorar la satisfacción

---

## 🧾 Anexos

- Código fuente
- Documentación técnica
- Manual del dashboard
- Bibliografía y fuentes externas (si aplica)

---

## ✍️ Autores

- [Nombre 1] – [Rol]  
- [Nombre 2] – [Rol]  
- [Fecha del informe]

