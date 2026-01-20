Análisis Matemático Avanzado en Python
Autor: Dr. Ignacio Sánchez Cohen
Lenguaje: Python 3
Interfaz gráfica: Tkinter
Enfoque: Cálculo simbólico, visualización matemática, ajuste de modelos y cálculos hidráulicos
Descripción general
Este software es una aplicación de escritorio desarrollada en Python que integra herramientas de:
•	Cálculo simbólico (derivadas, segundas derivadas e integrales).
•	Visualización gráfica de funciones 2D y superficies 3D.
•	Ajuste de modelos matemáticos a datos experimentales (2D y 3D).
•	Cálculos hidráulicos en canales abiertos mediante la ecuación de Manning.
Está orientado a docencia, investigación y aplicación ingenieril, particularmente en áreas como matemáticas aplicadas, ingeniería hidráulica y análisis de datos.
Funcionalidades principales
1. Derivadas e Integrales (2D y 3D)
•	Derivada primera
•	Derivada segunda
•	Integral indefinida
•	Gráficas comparativas de la función original y el resultado
•	Superficies 3D para funciones del tipo z = f(x, y)
2. Ajuste de Modelos Matemáticos
•	Lectura de datos desde archivos Excel (.xlsx)
•	Selección dinámica de variables
•	Modelos 2D disponibles:
o	Lineal
o	Cuadrático
o	Exponencial
o	Logarítmico
•	Modelo 3D:
o	Plano: z = a·x + b·y + c
•	Cálculo automático de métricas:
o	RMSE
o	R²
•	Identificación y graficación del mejor modelo de ajuste
3. Cálculos Hidráulicos (Canales Abiertos)
•	Geometrías disponibles:
o	Rectangular
o	Trapezoidal
o	Triangular
•	Cálculo de:
o	Área hidráulica
o	Perímetro mojado
o	Radio hidráulico
o	Velocidad media (Manning)
o	Gasto (Q)
•	Visualización esquemática de la geometría del canal
•	Panel de ayuda con valores típicos del coeficiente de Manning
Expresiones matemáticas soportadas
Funciones permitidas
sqrt(x), sin(x), cos(x), tan(x)
asin(x), acos(x), atan(x)
exp(x), log(x)
Constantes
pi, E
Ejemplos válidos
x^2 + 3*x + 5
sin(x)
exp(-x^2)
x*sin(x) + log(x)
x^2 + y^2
Errores comunes
2x        ❌ → 2*x        ✔
sin x     ❌ → sin(x)     ✔
log10(x)  ❌ → log(x)     ✔

Estructura general del programa
•	Cálculo simbólico: sympy
•	Análisis numérico: numpy, scipy
•	Gráficos: matplotlib (2D y 3D)
•	Interfaz gráfica: tkinter
•	Lectura de datos: pandas
•	Recursos visuales: GIF animado y logotipo rotatorio
Requisitos del sistema
Instalar previamente las siguientes librerías:
pip install sympy numpy matplotlib scipy pandas pillow
Tkinter viene incluido por defecto en la mayoría de las instalaciones de Python.
Ejecución
Desde la carpeta del proyecto:
python main.py
(Renombra el archivo según corresponda)
Entrada de datos para ajuste de modelos
•	Archivos Excel (.xlsx)
•	Columnas numéricas
•	Para ajuste 3D es necesario seleccionar X, Y y Z
