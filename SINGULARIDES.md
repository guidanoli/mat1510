Singularidades
==============

Definição de anel
-----------------
O anel `A(a, \delta_1, \delta_2)` é o conjunto aberto definido por
`A(a, \delta_1, \delta_2) = { z \in C : \delta_1 < |z| < \delta_2 }`.

### Casos particulares
`A(a, \delta, \infty)` é um anel ilimitado
`A(a, 0, r) = D(a, r) \ {a}`

Teorema de Laurent
------------------
Seja `f` uma função holomorfa no anel `A(a, \rho_1, \rho_2)` então
`f(z) = \sum_{m=1}^\infty [\frac{b_m}{(z - a)^m}] + \sum_{n=0}^\infty [a_n * (z - a)^n]`
onde a primeira série converge absolutamente fora do disco `\bar{D}(a, \rho_1)` e
a segunda série converge absolutamente no disco `D(a, \rho_2)`. Os coeficientes das séries
são dados de maneira única por
`a_m = \frac{1}{2 * \pi * i} * \int_\gamma \frac{f(w)}{(w - a)^{n+1}} dw,  n >= 1`
`b_m = \frac{1}{2 * \pi * i} * \int_\gamma f(z) * (z - a)^{m-1} dz,        m >= 1`
onde `\gamma` é um círculo de centro `a`, orienado no sentido anti-horário e contido
no anel `A(a, \rho_1, \rho_2)`.

Definição
---------
Seja `f` uma função holomorfa no anel `A(a, \rho_1, \rho_2)` e seja a expansão de Laurent
da `f` dada por `f(z) = \sum_{m=1}^\infty [\frac{b_m}{(z - a)^m}] + \sum_{n=0}^\infty [a_n * (z - a)^n]`
o número `a` é então...
* uma singularidade removível, se `b_m = 0` para `m >= 1`
* um polo de ordem `k` se `b_m /= 0` para `m <= k` e `b_m = 0` para `m > k`
* uma singularidade essencial se `b_m /= 0` para um número infinito de termos `b_m`
