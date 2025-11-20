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
- El dataset utilizado en la medida de lo posible, se usara uno de la FCV, de no ser posible, se buscaran datasets publicos
- Key variables
- Las principales variables son el diagnostico de ingreso y el diagnostico de egreso, actualmente no cuento con mas información referente a la clasificación para un reingreso
- Limitations
- No cuento con el contacto constante del personal que realiza la revisión de los reingresos, pero puedo pedir apoyo si es necesario en ellos para poder entender un poco mejor este tema

## 3. Approach
- ML models to test
- Regresión lineal
- Arboles de decision
- Bosques aleatorios
- Evaluation metrics
- F1 score

## 4. Expected Impact
- Examples of decisions improved by risk scores

## 5. Roadmap
- [ ] EDA
- [ ] Baseline model
- [ ] Threshold optimization
- [ ] Interpretability (SHAP)
- [ ] API or dashboard
