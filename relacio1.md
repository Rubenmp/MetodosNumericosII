# Relación 1 de MN

## Ejercicio 7

### Apartado a)

Sea $f: \mathbb{R^+} \longrightarrow \mathbb{R}$ definida por $f(x) = x + log(x)$. Lo que buscamos son soluciones de $f(x)=0$ en $\mathbb{R^+}$. Observamos que $f$ es creciente por ser $f'(x)=1+ \frac{1}{x}$ positiva en $\mathbb{R^+}$. Además, $f(\frac{1}{2}) < 0$ y $f(1)>0$.  Esto y el teorema de Bolzano nos dice que $f(x)$ tiene un solo cero y se encuentra en $(\frac{1}{2},1)$.

### Apartado b)

Divideremos el problema en dos casos, descartado el caso trivial $x_0=x^\ast$. El primer caso se da cuando $x_0 \in [a,x^\ast)$.
Para probar la convergencia por el método de Newton-Raphson basta notar que:

- $f(a)<0$ y $f(1)>0$, luego $f(a)f(1)<0$
- $f'$ nunca se anula
- $f''(x)=\frac{-1}{x^2}$ siempre es negativa
- $f(x)<0 \ \forall x \in [a,x^* )$, luego $f(x_0)f''(x_0)>0$


Resta probar el caso en que $x_0 \in (x^\ast,1]$.


## Ejercicio 10
