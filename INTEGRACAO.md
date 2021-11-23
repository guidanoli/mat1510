Integração
==========

Lema
----
Sejam `U \in C` um domínio e `f : U -> C` holomorfa.
Se `f'(z) = 0 \forall z \in U`, então `f` é constante.

Definição
---------
A integração da função `f` ao longo do caminho `\gamma` é um número complexo.
`\int_\gamma f(z) dz = \int_a^b f(\gamma(t)) * \gamma'(t) dt`.

Comprimento de um caminho
-------------------------
Se `\gamma(t) = x(t) + i * y(t)`, então
`l(\gamma) = \int_a^b |\gamma'(t)| dt = \int_a^b \sqrt{x'(t)^2 + y'(t)^2} dt`

Orientação do caminho
---------------------
Como a integral `\int_\gamma f(z) dz` depende do caminho, será sensível
da orientação e teremos que `\int_\gamma f(z) dz = -\int_\bar{\gamma} f(z) dz`.
Essa definição pode ser extendida para caminhos suaves por partes.

Integral de caminho suave por partes
------------------------------------
Sejam `f : U -> C` como antes e `\gamma = \gamma_1 * ... * \gamma_n` um caminho suave
por partes em `U`. A integral no caminho `\gamma` será o número complexo a seguir:
`\int_\gamma f(z) dz = \int_{\gamma_1} f(z) dz + ... + \int_{\gamma_n} f(z) dz`.
Analogamente para o comprimento do caminho....
`l(\gamma) = l(\gamma_1) + ... + l(\gamma_n)`

Propriedades de integrais complexas
-----------------------------------
1. `\int_\gamma c*f(z) dz = c * \int_\gamma f(z) dz \forall c \in C`
2. `\int_\gamma [f(z) + g(z)] dz = \int_\gamma f(z) dz + \int_\gamma g(z) dz`
