# ModelosyAprendizajes
Tema: Breast Cancer Wisconsin (Diagnostic) Data Set
Proyecto Final
Materia: Modelos y aprendizajes JUN22
Creado por: Alexis Correa
Profesor: Rafael Nogales


Datos importantes:

Los creaores del set de datos son:

	Dr. William H. Wolberg, General Surgery Dept., University of
	Wisconsin,  Clinical Sciences Center, Madison, WI 53792
	wolberg@eagle.surgery.wisc.edu

	W. Nick Street, Computer Sciences Dept., University of
	Wisconsin, 1210 West Dayton St., Madison, WI 53706
	street@cs.wisc.edu  608-262-6619

	Olvi L. Mangasarian, Computer Sciences Dept., University of
	Wisconsin, 1210 West Dayton St., Madison, WI 53706
	olvi@cs.wisc.edu 
Puedes encontrar el set completo en la siguiente dirección https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

La base está compuesta de 569 registros y 32 columnas y en el detalle indica que la información recolectada describe
las caracteristicas presentes en las imagenes de nucleos celulares que fueron tomados de una masa mamaria de cada paciente. 
Se utilizó  un método de clasificación (árbol de decisión)
Para hacer una mejor lectura se agregó encabezado que se detalla a continuación:
id
diagnosis (M = malignant, B = benign)
radius_mean
texture_mean
perimeter_mean
area_mean
smoothness_mean
compactness_mean
concavity_mean
concave points_mean
symmetry_mean
fractal_dimension_mean
radius_se
texture_se
perimeter_se
area_se
smoothness_se
compactness_se
concavity_se
concave points_se
symmetry_se
fractal_dimension_se
radius_worst
texture_worst
perimeter_worst
area_worst
smoothness_worst
compactness_worst
concavity_worst
concave points_worst
symmetry_worst
fractal_dimension_worst

El tema principal del proyecto es evaluar diferentes modelos y desde los resultados que muestren, elegir el mejor.
Para evitar la repetición de sintaxis en cada modelo, creé una función que evalua cada modelo, enviando el nombre 
del modelo y las variables independiente (X) y la dependiente (y) que fue definida como evalua_modelo (model, X, y)
y como resultado un Dataframe con los valores de accuracy, f1_score, precision, recall, balanced_accuracy y
la respectiva matriz de confusión.
Para una mejor visualización de los resultados y selección del modelo más conveniente, se muestra al final gráficos 
lineales de cada valor guardado en el Dataframe (eval_df).
Según los resultados obtenidos, el mejor modelo es el RandomForestClassifer, debido a que la precisión 
fue del 99%. Teniendo 98% de precisión en los casos predichos correctamente como verdaderos positivos 

La carpeta contiene:
Base de datos (wdbc.DATA)
