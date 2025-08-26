# Clases del 25 de agosto

## Probabilidad
- **Suceso mutuamente excluyente** = dos eventos que no pueden ocurrir al mismo tiempo. **P(A ∩ B) = 0**
- **Suceso independiente** = dos eventos cuya ocurrencia no afecta la probabilidad del otro. **P(A ∩ B) = P(A) * P(B)**
- **Espacio muestral** = conjunto de todos los resultados posibles de un experimento aleatorio.
- **Evento** = subconjunto del espacio muestral.
- **Probabilidad** = medida de la posibilidad de que ocurra un evento.
- **Multiplicación de probabilidades** = **P(A ∩ B) = P(A) * P(B)** para eventos independientes.
- **Adición de probabilidades** = **P(A ∪ B) = P(A) + P(B) - P(A ∩ B)** para eventos no mutuamente excluyentes.
- **Complemento de probabilidades** = **P(A') = 1 - P(A)** para el evento complementario A'.
- **Ley de total de probabilidades** = **P(B) = P(B|A)P(A) + P(B|A')P(A')** para eventos A y B.
- **Probabilidad condicional** = **P(A|B) = P(A ∩ B) / P(B)** para eventos A y B.

## Variables aleatorias
- **Variable aleatoria** = función que asigna un valor numérico a cada resultado de un experimento aleatorio.
- **Recorrido de X** = conjunto de todos los valores posibles que puede tomar la variable aleatoria X, Notación: R(X).
- **Variables aleatorias discretas** = variables que solo pueden tomar un número finito o contable de valores (por ejemplo, el número de caras al lanzar un dado).
    - **Función de probabilidad puntual** = asigna una probabilidad a cada valor posible de la variable aleatoria discreta. Notación: P(X = x) ó p(xi) donde xi es cada x dentro de R(X).
    - **Recorrido infinito numerable** = conjunto infinito de valores que se pueden enumerar (por ejemplo, números enteros: 1, 2, 3, ...).
    - **Recorrido finito numerable** = conjunto finito de valores que se pueden enumerar (por ejemplo, el número de caras al lanzar un dado).
    - **Función de distribución acumulada (FDA)** = función que da la probabilidad de que la variable aleatoria sea menor o igual a un valor específico. Notación: F(x) = P(X ≤ x); F(t) = P(X ≤ t).
        - Para una variable aleatoria discreta, la FDA se calcula como la suma de las probabilidades de todos los valores menores o iguales a x: F(x) = Σ_{k ≤ x} P(X = k).
        - **Propiedades de la FDA**:
            - F(x) es no decreciente: si x1 < x2, entonces F(x1) ≤ F(x2).
            - Limites: F(-∞) = 0 y F(∞) = 1.
            - La FDA es una función escalonada, con saltos en los puntos donde la variable aleatoria toma valores específicos.
            - La probabilidad puntual se puede obtener a partir de la FDA: P(X = x) = F(x) - F(x-), donde F(x-) es el límite de F cuando se aproxima a x desde la izquierda.
            - La FDA puede usarse para calcular probabilidades de intervalos: P(a < X ≤ b) = F(b) - F(a).
- **Variables aleatorias continuas** = variables que pueden tomar cualquier valor dentro de un intervalo
    - **Esperanza (media)** = valor promedio ponderado de la variable aleatoria. Notación: E(X) o μ. Estarían cerca de los valores con mayor probabilidad de ocurrir. Para una variable aleatoria discreta, la esperanza se calcula como: E(X) = Σ [x * P(X = x)].
    - **Varianza** = medida de la dispersión de la variable aleatoria. Notación: Var(X) o σ².
        - Para una variable aleatoria discreta, la varianza se calcula como: Var(X) = Σ [(x - μ)² * P(X = x)], donde μ = E(X).
        - Una fórmula alternativa y útil es: Var(X) = E[X²] - (E[X])².
    - **Desviación estándar** = raíz cuadrada de la varianza. Notación: σ.
        - La desviación estándar se calcula como: σ = √Var(X) = √σ².
