Residuos
========

Definição
---------
Se `f` é uma função holomorfa no anel `A(a,0,\rho)`, o resíduo de `f` em `a` é o coeficiente `b_1`
do termo `1/(z-a)` da sua série de Laurent com centro em `a`.

Teorema dos Resíduos
--------------------
Seja `f` uma função holomorfa num domínio `U \ {a_1, ..., a_m}`.
Suponha que `\gamma \in U \ {a_1, ..., a_m}` é uma curva de Jordan suave por partes, orientada no sentido anti-horário,
tal que a região fechada e limitada por ela está contida em `U` e contém todos os pontos `a_1, ..., a_m`. Então:
`1/(2\pi * i) * \int_\gamma f(z) dz = Res(f,a_1) + ... + Res(f,a_m)`

Proposição
----------
Seja `f` uma função holomorfa no anel `A(a,0,\rho)` e suponha que `a` é um polo de ordem 1 de `f`.
Então `Res(f,a) = lim_{z \to a} (z-a) * f(z)`.

Proposição
----------
Seja `f` uma função holomorfa no anel `A(a,0,\rho)` e suponha que `a` é um polo de ordem `k > 1` de `f`.
Então seja `g(z) = (z - a)^k * f(z)` e `Res(f,a) = \frac{g^(k-1)(a)}{(k-1)!}`.

Teorema
-------
Seja `f` uma função holomorfa num domínio `U \ {a_1, ..., a_m}`.
Suponha que `\gamma \in U \ {a_1, ..., a_m}` é uma curva de Jordan suave por partes, orientada no sentido anti-horário,
tal que a região fechada e limitada por ela está contida em `U` e contém todos os pontos `a_1, ..., a_m`.
Suponha também que todos esses pontos sejam polos de `f` e que `f` não tem zeros ao longo da curva `\gamma`. Então:
`1/(2\pi * i) \int_\gamma f'(z)/f(z) dz = Z - P`
onde `Z` = número de zeros de `f` no interior de `\gamma` contados com multiplicidades e
`P` = número de polos de `f` no interior de `\gamma` contados tantas vezes como indica sua ordem

Teorema
-------
Com as mesmas hipóteses do teorema anterior, se `f` e `h` são holomorfas em `U` então
`1/(2\pi * i) \int_\gamma h(z) f'(z)/f(z) dz = \sum_{\csi_k} h(\csi_k) m_{\csi_k}(f)`
onde `\csi_k` são os zeros de `f` na região interior a `\gamma` e 
`m_{\csi_k}(f)` sua multiplicidade.

Teorema de Rouché
-----------------
Sejam `f` e `g` duas funções holomorfas definidas no domínio `U \in C`.
Seja `V \in U` uma região fechada e limitada tal que a sua fronteira é uma curva de Jordan suave por partes com `V\dV` um domínio. Se:
`|f(z) - g(z)| <= |f(z)|` para todo `z in dV`
Então `f` e `g` têm o mesmo número de zeros no interior de `V`, cada um deles contado com suas multiplicidades.
