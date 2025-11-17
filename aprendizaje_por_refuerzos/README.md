# Aprendizaje por Refuerzo – SARSA, Q-Learning y Softmax
### Diplomatura en Ciencia de Datos – FAMAF 2025

---

## 🧠 Descripción del proyecto

Este repositorio contiene el Trabajo Práctico de Aprendizaje por Refuerzo, donde se implementaron y analizaron los algoritmos:

- SARSA (on-policy)
- Q-Learning (off-policy)
- Política de exploración Softmax
- Ajuste de hiperparámetros α, ε y γ
- Visualización de políticas aprendidas en el entorno CliffWalking-v1

También se exploraron los entornos CartPole y MountainCar para observar cómo interactúa un agente con el entorno en episodios aleatorios.

### ✔ CartPole-v0  
Un carrito que debe balancear un palo vertical durante el mayor tiempo posible.

<img width="588" height="390" alt="image" src="https://github.com/user-attachments/assets/7ba277e9-0682-4b37-84a9-b11899e993ee" />

### ✔️ MountainCar-v0

Un auto atrapado en un valle que debe tomar impulso para subir la montaña.

<img width="585" height="379" alt="image" src="https://github.com/user-attachments/assets/287a1d89-3cf6-4080-92bf-c60df8933af4" />

---
# 🧩 Implementaciones realizadas

## ✔ Política ε-greedy

El agente elige la mejor acción conocida con probabilidad (1−ε), y una acción aleatoria con probabilidad ε.

```python
def choose_action_e_greedy(state, actions, q, hyperparameters, random_state):
    ...
```
## ✔ Política Softmax

Se implementó la política Softmax:

​

```python
def choose_action_softmax(state, actions, q, hyperparameters, random_state):
    ...
```

## 🔧 Algoritmos implementados
- **SARSA** con política *ε-greedy*  
- **Q-Learning** con política *ε-greedy*  
- **Softmax** implementado sobre **SARSA** (porque es un algoritmo *on-policy* y la política afecta directamente el aprendizaje)

---
##  👩‍💻 Autora
Micaela Zamorano

Diplomatura en Ciencia de Datos – FAMAF

2025
