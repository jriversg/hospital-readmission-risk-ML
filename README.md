# Hospital Readmission Risk Prediction (30 days)

## 1. Problem Definition
- What is hospital readmission?
- Un reingreso hospitalario es condsiderado como tal, cuando un paciente luego de haber egresado de la institución de salud, reingresa a esta por la misma causa a la cual egreso.
- Why does it matter (clinical + economic impact)?
- Un reingreso hospitalario impacta negativamente en el costo de la atención, una reingreso necesita mas examenes, mas laboratorios, mas dias de estancia, lo cual no esta pactado en el PGP incialmente con cada una de las EPS (Entidad Promotora de Salud)
- Who benefits?
- Los beneficios vienen en ambas partes, tanto como la institucion porque se ahorran un dinero el cual no esta presupuestado gastar para un reingreso y el paciente dado que mejora su calidad de vida al ser atendido con precision durante su primera atencion

## 2. Data
- Source: dataset used
- Se utilizara un dataset publico de Keaggle, que cuenta con 25000 filas y 17 columnas. link: https://www.kaggle.com/datasets/dubradave/hospital-readmissions?resource=download
- Este dataset cuenta con las siguientes variables:
* Edad -- > age
* Dias en hospitalización --> time_in_hospital
* Número de procedimientos en la estancia actual --> n_procedures
* Número de laboratorios realizados en la estancia actual --> n_lab_procedures
* Número de medicamentos suministrados en la estancia actual --> n_medications
* Número de visitas ambulatorios el año antes de la estancia actual --> n_outpatient
* Número de visitas hospitalarias el año antes de la estancia actual --> n_inpatient
* Número de visitas a urgencias el año antes de la estancia actual --> n_emergency
* Especialidad del médico que ingresa al paciente en la estancia actual --> medical_specialty
* Diagnostico 1 --> diag_1
* Diagnostico 2 --> diag_2
* Diagnostico 3 --> diag_3
* Test de glucosa en sangre --> glucose_test
* Nivel de A1C --> A1Ctest
* Si hubo cambio en la medicacion de la diabetes --> change
* Si se prescribio un medicamento para diabetes --> diabetes_med
* Reingresado --> readmitted
- Key variables
* readmitted --> Variable objetivo
* age, time_in_hospital, diag_1, diag_2, glucose_test: son variables que serviran para el entrenamiento del modelo
- Limitations
- No cuento con el contacto constante del personal que realiza la revisión de los reingresos, pero puedo pedir apoyo si es necesario en ellos para poder entender un poco mejor este tema

## 3. Approach
- ML models to test
* Regresión logistica
* Arbol de decisión
* Random Forest
- Evaluation metrics
* F1-score
* ROC-AUC
* Matriz de confusión

## 4. Expected Impact
- Examples of decisions improved by risk scores
* Identificar pacientes con alto riesgo de reingreso hospitalario antes del alta
* Optimizar el giro-cama evitando reingresos innecesario o evitables

## 5. Roadmap
- [ ] EDA
- [ ] Baseline model
- [ ] Threshold optimization
- [ ] Interpretability (SHAP)
- [ ] API or dashboard
