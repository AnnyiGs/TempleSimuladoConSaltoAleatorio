# 🧬 Optimización con Algoritmo Genético con Mutación y vuelo de Levy

Este proyecto implementa un algoritmo genético para minimizar la función de Rastrigin en una dimensión. Se utiliza una estrategia de mutación basada en vuelos de Levy para mejorar la exploración del espacio de búsqueda.

## 📌 Descripción

La función de Rastrigin es una función no convexa comúnmente utilizada como benchmark en problemas de optimización. Este script busca encontrar el mínimo global de dicha función utilizando:

- Selección por torneo
- Cruce promedio entre padres
- Mutación basada en vuelos de Levy

## 🧠 Algoritmo

El flujo general del algoritmo es:

1. **Inicialización** de una población aleatoria dentro de los límites definidos.
2. **Evaluación** de cada individuo usando la función de Rastrigin.
3. **Selección** de padres mediante torneo.
4. **Cruce** para generar descendencia.
5. **Mutación** con vuelos de Levy.
6. Repetición del proceso por un número definido de generaciones.
7. Retorno del mejor individuo encontrado.

## 📈 Función objetivo

```python
def objective_function(x):
    return 10 + x**2 - 10 * math.cos(2 * math.pi * x)
El mínimo global es 0 en 𝑥 = 0
```

## ⚙️ Parámetros
Puedes ajustar los siguientes parámetros para experimentar:

Parámetro	Valor por defecto	Descripción
population_size	50	Número de individuos en la población
lower_bound	-5.12	Límite inferior del espacio de búsqueda
upper_bound	5.12	Límite superior del espacio de búsqueda
generations	100	Número de generaciones
mutation_rate	0.1	Probabilidad de aplicar mutación
## 🚀 Ejecución
Para correr el script, simplemente ejecuta:

bash
python templeModificado.py
Verás en consola la evolución de la mejor solución por generación y el resultado final.

## 📚 Requisitos
Python 3.x

Numpy

Instalación de dependencias:

bash
pip install numpy

## 🧪 Ejemplo de salida
Código
Generation 1: Best solution = -0.23, Best fitness = 0.53
---
Resultado final:
Mejor solución encontrada: x = -0.0001
Valor mínimo de f(x) = 0.00002

---
👨‍💻 *Autor: OCHOA ORTEGA ANDREA JOSELYN #2*  
📅 *TEMPLE SIMULADO CON SALTOS ALEATORIOS* 
