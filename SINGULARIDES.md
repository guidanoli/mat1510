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

Singularidade removível
-----------------------
É aquela tal que `b_m = 0` para todo `m >= 1`

Polo de ordem k
---------------
É aquele tal que `b_m /= 0` para `m <= k` e `b_m = 0` para todo `m > k`

Singularidade essencial
-----------------------
É aquela tal que `b_m /= 0` para um número infinito de termos `b_m`

Teorema
-------
Seja `f` uma função holomorfa no anel `A(a,0,\rho)`. Então as seguintes afirmações são equivalentes.
1. `a` é singularidade removível de `f`
2. existe o `lim_{z \to a} f(z)`
3. `|f|` é limitado em algum anel `A(a,0,\delta) \in A(a,0,\rho)`

Colorário
---------
Se `b_m /= 0` para algum `m >= 1`, então `|f|` é ilimitado em qualquer disco de centro em `a`.

Teorema
-------
Se `f` é uma função holomorfa no anel `A(a,0,\rho)` então `a` é um polo de ordem `k` de `f`,
se e somente se, `lim_{z \to a} [(z-a)^k * f(z)]` existe e é um número complexo não-nulo.

Colorário
---------
Se `f` é uma função holomorfa no anel `A(a,0,\rho)` e `a` é polo de ordem `k` de `f`,
então `lim_{z \to a} |f(z)| = \infty`.

Teorema de Picard
-----------------
Se `a` é uma singularidade essencial de `f` holomorfa em `A(a,0,\delta)` dado `0 < r < \delta`,
a imagem do disco `A(a,0,r)` em `f` cobrirá todo o plano `C` exceto no máximo um ponto.

Teorema de Casorati-Weierstrass
-------------------------------
Seja `f` uma função holomorfa no anel `A(a,0,\rho)` e suponha que `a` é singularidade essencial de `f`.
Então dados `0 < r < \rho`, `\epsilon > 0` e `\alpha \in C`, existe um número complexo `\beta` tal que
`\beta \in A(a,0,r)` e `|f(\beta) - \alpha| < \epsilon`.
