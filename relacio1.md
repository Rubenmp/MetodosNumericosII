# Relación 1 de MN

## Ejercicio 7

### Apartado a)

Sea $f: \mathbb{R^+} \longrightarrow \mathbb{R}$ definida por $f(x) = x + log(x)$. Lo que buscamos son soluciones de $f(x)=0$ en $\mathbb{R^+}$. Observamos que $f$ es creciente por ser $f'(x)=1+ \frac{1}{x}$ positiva en $\mathbb{R^+}$. Además, $f(\frac{1}{2}) < 0$ y $f(1)>0$.  Esto y el teorema de Bolzano nos dice que $f(x)$ tiene un solo cero y se encuentra en $(\frac{1}{2},1)$.

### Apartado b)

Divideremos el problema en tres casos, descartado el caso trivial $x_0=x^\ast$. El primer caso se da cuando $x_0 \in [a,x^\ast)$.
Para probar la convergencia por el método de Newton-Raphson basta notar que:

- $f \in C^\infty(\mathbb{R^+})$
- $f(a)<0$ y $f(1)>0$, luego $f(a)f(1)<0$
- $f'$ nunca se anula
- $f''(x)=\frac{-1}{x^2}$ siempre es negativa
- $f(x)<0 \ \forall x \in [a,x^* )$, luego $f(x_0)f''(x_0)>0$


Resta probar la convergencia en el segundo caso, cuando $x_0 \in (x^\ast,1)$. Sea $g: \mathbb{R^+} \longrightarrow \mathbb{R}$ definida por $g(x)=x-\frac{f(x)}{f'(x)}$. Tenemos que $g(x_n)=x_{n+1}$. Por otro lado,
$$g'(x)=\frac{f(x)f''(x)}{(f''(x))^2}$$

Sabemos que $f'>0$, que $f''<0$ y que $f(x)>0\ \forall x>x^\ast$. Por tanto, $g'(x)<0\ \forall x>x^\ast$. Además, $g$ es claramente continua. Entonces,

$$x^\ast<x_0 \leq 1 \Rightarrow g(1)=\frac{1}{2} \leq g(x_0)<g(x^\ast)=x^\ast \Rightarrow x_1 \in \left[ \frac{1}{2}, x^\ast \right) $$

Y, por el caso anterior, tenemos la convergencia.

## Ejercicio 10
