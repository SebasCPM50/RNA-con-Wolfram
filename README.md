# Red Neuronal Artificial para Compuertas Lógicas (AND, OR, XOR)  

## Descripción  
Este proyecto implementa **Redes Neuronales Artificiales (RNA)** utilizando **Wolfram Language** para simular el comportamiento de tres compuertas lógicas fundamentales:  

- **AND**  
- **OR**  
- **XOR**  

El objetivo es entrenar una red neuronal que aprenda las salidas correctas a partir de los patrones de entrada, validando la capacidad de las RNA para modelar funciones lógicas básicas.  

---

## Archivos del proyecto  
- `AND.nb` → Implementación y entrenamiento de la red para la compuerta **AND**.  
- `OR.nb` → Implementación y entrenamiento de la red para la compuerta **OR**.  
- `XOR.nb` → Implementación y entrenamiento de la red para la compuerta **XOR**.  

Cada archivo contiene:  
1. Definición de los **datos de entrenamiento** (entradas y salidas esperadas).  
2. Construcción de una **red neuronal simple** con capas lineales y funciones de activación.  
3. Entrenamiento con `NetTrain`.  
4. Validación mediante una **tabla comparativa** entre el valor real y la predicción de la red.  

---

## Tecnologías utilizadas  
- **Lenguaje:** Wolfram Language (Mathematica).  
- **Funciones principales:**  
  - `NetChain` → Construcción de la arquitectura de la red.  
  - `LinearLayer`, `Tanh`, `LogisticSigmoid` → Capas y funciones de activación.  
  - `NetTrain` → Entrenamiento supervisado de la red neuronal.  
  - `TableForm` → Presentación de resultados.  

---

## Resultados esperados  
Tras el entrenamiento, cada red debe ser capaz de **aproximar las funciones lógicas** de la compuerta correspondiente.  

Ejemplo (para XOR):  

| x1,x2   | Salida Real | Predicción |
|---------|-------------|------------|
| {0,0}   | 0           | 0          |
| {0,1}   | 1           | 1          |
| {1,0}   | 1           | 1          |
| {1,1}   | 0           | 0          |

De esta manera, se valida que la red neuronal ha aprendido el comportamiento de la compuerta.  

---

## Conclusión  
Este ejercicio muestra cómo las **Redes Neuronales Artificiales** pueden ser entrenadas para aprender funciones lógicas simples.  
- Las compuertas **AND** y **OR** pueden resolverse con un perceptrón de una sola capa.  
- La compuerta **XOR**, al no ser linealmente separable, requiere al menos una **capa oculta** y una función de activación no lineal (ej. `Tanh`).  

Esto evidencia la importancia de la arquitectura de la red en la capacidad de aprendizaje de las RNA.  
