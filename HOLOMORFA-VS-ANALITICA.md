Holomorfa vs Analítica
======================

Teorema
-------
Sejam `f : U -> C` uma função holomorfa, onde `U` é um domínio em `C` e `z_0 \in U` um ponto qualquer. Então
`f(z) = \sum_{n=0}^\infty \frac{f^(n)(z_0)}{n!} * (z - z_0)^n`. Isto é, a `f` é analítica. Essa série converge
em qualquer disco aberto `D(z_0, r) \in U` onde `r` é a menor distância do `z_0` até a fronteira de `U`.

Teorema de Morera
-----------------
Sejam `U \in C` um domínio e `f : U -> C` uma função contínua. Se `\int_\Delta f(z) dz = 0` para todo caminho
triangular `\Delta \in U` então `f` é holomorfa em `U`.
