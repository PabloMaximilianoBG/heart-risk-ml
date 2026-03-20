## Clasificación de Riesgo de Ataque al Corazón con Machine Learning

Este proyecto aplica técnicas de Machine Learning para predecir el nivel de riesgo de ataque cardíaco (`Risk_Level`) en pacientes a partir de variables clínicas.

### Enfoque
Se evaluaron 54 modelos combinando:
- 3 algoritmos: Logistic Regression, Random Forest y SVM
- 2 opciones de normalización (con y sin StandardScaler)
- 3 conjuntos de variables (Full, Subset1, Subset2)
- 3 variantes por modelo

### Modelos utilizados
- **Logistic Regression**: Modelo base lineal
- **Random Forest**: Ensamble de árboles, robusto a relaciones no lineales
- **Support Vector Machine (SVM)**: Clasificador potente con distintos kernels

###  Evaluación
Se utilizó **F1-Score ponderado**, ideal para datasets desbalanceados.

### Resultados
El mejor modelo fue:
- **Random Forest (150 árboles, sin límite de profundidad)**
- Usando **todas las variables**
- Sin necesidad de normalización
- **F1-Score ≈ 0.98**

### Conclusiones
- Random Forest capturó mejor las relaciones no lineales del problema
- La normalización no impactó modelos basados en árboles
- Usar todas las variables permitió mejorar el rendimiento

### Visualización
Se generó una comparación gráfica del F1-Score para los 54 modelos evaluados.

---

### Tecnologías utilizadas
- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
<p align="center">
  <img src="maching.png" width="100%" />
</p>
