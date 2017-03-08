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

### Introducción
Mostrando la gráfica de la función vemos que tiene solamente una solución:

![uno](./Imagenes/1.10.1.pdf)

![dos](./Imagenes/1.10.2.pdf)


### Apartado a)
Utilizamos en la ecuación $f(x)=x^3+4x^2-10$ las iteraciones de punto fijo dadas por
$$x_{n+1}=\frac{2x_n^3+4x_n^2+10}{3x_n^2+8x_n}, n\geq 0$$

Sumando y restando $20$ y $\frac{f(x_n)}{f'(x_n)}$ en la primera ecuación obtenemos
$$x_{n+1}=\frac{x_n^3+20}{3x_n^2+8x_n}+\frac{f(x_n)}{f'(x_n)} = \frac{x_n^3+20}{3x_n^2+8x_n} + 2\frac{f(x_n)}{f'(x_n)}-\frac{f(x_n)}{f'(x_n)} = \frac{x_n^3+20+2(x_n^3+4x_n^2-10)}{3x_n^2+8x_n}$$
$$x_{n+1}=x_n-\frac{f(x_n)}{f'(x_n)}$$


### Apartado b)
Para usar la convergencia de Newton global tenemos que reunir una serie de condiciones. $f\in C^2(\mathbb{R})$, en particular es de clase 2 para todo compacto de $\mathbb{R}$.
Usaremos que $f(x^* )=0$, si tomamos $a\in]0,x^* [$, $b>x^{\ast}$ se cumple

* $f(a)f(b)<0$
* $\forall x\in [a,b], f'(x)=3x^2+8x>0$, ya que $a>0$
* $f''(x) = 6x+8$ no cambia de signo en $x\in [a,b]$

El punto $x_0$ buscado debe cumplir
$$x_0 \in [a, b] \text{ tal que } f(x_0) f''(x_0) \geq 0$$
