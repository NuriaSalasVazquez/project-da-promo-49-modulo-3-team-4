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

- [Fuente](https://data.ca.gov/dataset/labor-force-participation-rate-by-age-group/resource/d58bfa55-8f7f-438f-9e46-0cae78a80d91)

### 2. Limpieza y preprocesamiento

- Unificación nombre columnas 
- Eliminación de valores nulos
- Codificación de variables categóricas
- Normalización / estandarización
- Detección de outliers
- Filtrado de columnas para el análisis

Para más detalles: click [aquí](https://docs.google.com/spreadsheets/d/1pLfwP7zJ8qAkEuVE2P4qM-kj6z-0E_emVTnwHtOpboE/edit?usp=sharing)

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
![Porcentaje de empleados de cada generación](img/empleados_gen.png) ![Empleados por género](img/empleados_genero.png)

A partir del análisis de datos, visualizaciones y comparativas clave, se identificaron varios factores relevantes que pueden influir directamente en la satisfacción laboral y la retención del talento en la empresa.

- En primer lugar, la **composición generacional** de la plantilla muestra una clara mayoría de empleados Millennials, con menor representación de Baby Boomers, algo esperable por cuestiones demográficas y de jubilación. Si bien los Gen X presentan una distribución bastante equitativa en todos los roles, los Baby Boomers se concentran en puestos altos como directores o ejecutivos, y la Gen Z aún no accede a posiciones de liderazgo por falta de experiencia. Esto refleja una jerarquía laboral lógica basada en la antigüedad y sugiere que la movilidad hacia puestos superiores es más común en generaciones con más años en la empresa.

- En cuanto al **salario**, se observa que quienes poseen títulos de doctorado tienden a ganar más, aunque este patrón no se replica en la Gen Z. En general, los Gen X son quienes tienen los salarios más altos, seguidos por Millennials. Además, se identificó un valor atípico extremo $10^6$ que fue filtrado para evitar distorsiones. Se debe destacar que, a pesar de ciertas excepciones, no se encontró una relación directa entre el salario y la satisfacción laboral, lo que apunta a que factores como el ambiente o las relaciones laborales podrían ser más importantes para los empleados. Sin embargo, tampoco se ha encontrado una relación entre las diferentes escalas de satisfacción y los datos disponibles. 

- Analizando la **distribución de roles** por generación, los Millennials aparecen en una variedad más amplia de puestos, mientras que Gen X y Baby Boomers predominan en roles de liderazgo. Esto abre la puerta a pensar en posibles barreras al ascenso para las generaciones más jóvenes, especialmente si se busca aumentar la retención de talento en estos rangos de edad. La empresa podría beneficiarse de reforzar programas de promoción y capacitación dirigidos a Millennials y Gen Z, especialmente para roles estratégicos como managers o directores de investigación. 

- En cuanto a la **satisfacción laboral**, los niveles generales son positivos, con la mayoría de empleados puntuando entre 3 y 4 en escalas de satisfacción ambiental y relaciones interpersonales. Sin embargo, hay diferencias entre generaciones: los Baby Boomers presentan mayores niveles de insatisfacción, los Millennials se muestran más conformes, y la Gen X aparece polarizada. En términos de puestos, se detectaron focos de insatisfacción entre Sales Executives, Laboratory Technicians y Recursos Humanos, lo cual puede determinar un posible punto de mejora.

- Por último, el **análisis de género** reveló que, aunque las mujeres son mayoría y están presentes incluso en niveles jerárquicos altos, los hombres tienden a tener salarios promedio más elevados, especialmente en niveles educativos superiores. Esto podría generar una sensación de menor valoración profesional entre las mujeres, influyendo en su satisfacción y aumentando el riesgo de rotación. Por ello, se sugiere revisar políticas de igualdad salarial y crecimiento profesional, con el fin de detectar y corregir posibles brechas invisibles.

---

## 📌 Conclusiones y Recomendaciones

## 📌 Conclusiones del Análisis

- La **composición generacional** muestra que existe una mayoría de empleados *Millennials*, mientras que los *Baby Boomers* se concentran en puestos de liderazgo y la *Generación Z* aún no accede a esos niveles, reflejando una jerarquía basada en la antigüedad.

- Aunque los empleados con **títulos de doctorado** tienden a tener salarios más altos (especialmente *Gen X* y *Millennials*), **no se encontró una relación directa entre el salario y la satisfacción laboral**. 

- En la **distribución de roles**, los *Millennials* ocupan una mayor variedad de puestos, mientras que *Gen X* y *Baby Boomers* dominan cargos de liderazgo. Esto podría indicar **barreras al ascenso** para generaciones más jóvenes.

- Se recomienda **impulsar programas de desarrollo profesional y promoción interna** enfocados en *Millennials* y *Gen Z*, especialmente para funciones estratégicas como *managers* y *directores de investigación*.

- Los niveles de **satisfacción laboral** son positivos en general, pero:
  - *Baby Boomers* presentan mayor insatisfacción.
  - *Millennials* se muestran más conformes.
  - *Gen X* presenta polarización en sus niveles de satisfacción.
  - Ciertos puestos como *Sales Executives*, *Laboratory Technicians* y *Recursos Humanos* mostraron mayor insatisfacción, lo que sugiere **focos concretos de mejora**.

- El **análisis de género** reveló que, a pesar de que las mujeres son mayoría y están presentes en niveles jerárquicos altos, **los hombres tienen salarios promedio más altos**, especialmente con mayores niveles educativos.

- Se recomienda **revisar y fortalecer políticas de igualdad salarial y oportunidades de crecimiento profesional** para evitar desigualdades que podrían afectar la satisfacción y aumentar la rotación, especialmente entre mujeres.

---

## 🧾 Anexos

- Documentación: [Detalles de datos originales](https://docs.google.com/spreadsheets/d/1pLfwP7zJ8qAkEuVE2P4qM-kj6z-0E_emVTnwHtOpboE/edit?usp=sharing)
- Bibliografía y fuentes externas: [California Open Data Portal](https://data.ca.gov)

---

## ✍️ Autores

- Amanda Hernández – SCRUM Máster 1. Analista de datos. 
- Nuria Salas – SCRUM Máster 2. Analista de datos. 
- Cristina Martín - Analista de datos.
- Marianela Gómez - Analista de datos. 

