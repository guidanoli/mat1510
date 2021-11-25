Primitivas
==========

Definição
---------
Seja `f : U -> C` uma função contínua, onde `U \in C` é um domínio.
Uma função `F : U -> C` é chamada uma primitiva de `f` se
`F` é holomorfa em `U` e `F'(z) = f(z)` para todo ponto `z \in U`.

### Bônus
Além disso, se `F` é uma primitiva de `f` temos `G(z) = F(z) + K`
será uma primitiva também da `f` para todo `K \in C`.

Teorema
-------
Sejam `U \in C` um domínio, `f : U -> C` uma função contínua,
`F` uma primitiva de `f` em `U` e `\gamma` uma caminho suave por partes
em `U` unindo o ponto `z_0` ao ponto `z_1`. Então...
`\int_\gamma f(z) dz = F(z_1) - F(z_0)`.

### Bônus
Em particular, se o caminho é fechado então
`\int_\gamma f(z) dz = 0`.

Proposição
----------
Seja `f(z) = \sum_{n=0}^\infty [a_n * (z - z_0)^n]` definida por uma série de potências
com raio de convergência `R > 0`. Então a função
`F(z) = \sum_{n=0}^\infty [\frac{a_n}{n + 1} * (z - z_0)^{n+1}]`
é uma primitiva de `f` e a série que a define converge para `|z - z_0| < R`.

Lema
----
Sejam `U \in C` um domínio, `f : U -> C` uma função contínua e `\gamma(t)`, `a <= t <= b`,
um caminho suave por partes em `U`, de comprimento `l(\gamma)`. Seja `K >= 0` um número
real tal que `|f(\gamma(t))| <= K` para todo `a <= t <= b`. Então podemos afirmar que
`| \int_\gamma f(z) dz | <= K * l(\gamma)`.

Teorema
-------
Seja `f : U -> C` uma função contínua definida no domínio `U \in C`.
As seguintes afirmativas são equivalentes:
1. `f` tem uma primitiva em `U`
2. `\int_\gamma f(z) dz = 0` para qualquer caminho fechado, suave por partes `\gamma` em `U`
3. `\int_\lambda f(z) dz` só depende dos pontos inicial e terminal de qualquer caminho suave por partes `\lambda` em `U`.
