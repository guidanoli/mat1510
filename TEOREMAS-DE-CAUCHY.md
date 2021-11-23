Teoremas de Cauchy
==================

Teorema de Cauchy-Goursat
-------------------------
Sejam `U` um domínio em `C` e `f : U -> C` uma função holomorfa.
Suponha que `\Delta \in U` é um triângulo que limita uma região inteiramente contida em `U`.
Então `\int_\Delta f(z) dz = 0`.

### Consequência
Com esse resultado, podemos mostrar a existência de primitvas em regiões mais gerais chamadas estreladas.

Definição
---------
Seja `U \in C` um domínio. Dizemos que `U` é estrelado se existe um ponto `z_0 \in U` satisfazendo a seguinte propriedade:
dado qualquer ponto `z \in U`, o segmento de reta unindo `z_0` a `z`, esta inteiramente contido em `U`.
O ponto `z_0` é chamado um cnetro do domínio `U`. Alguns exemplos de domínios estrelados:
* O plano complexo `C`
* Regiões convexas
* O plano complexo `C` menos uma semireta
* Uma estrela

Colorário
---------
Sejam `U \in C` um domínio estrelado e `f : U -> C` uma função holomorfa.
Então `f` admite uma primitiva em `U`.

Teorema de Cauchy-Goursat bis
-----------------------------
Sejam `U \in C` um domínio estrelado e `f : U -> C` uma função holomorfa.
Se `\gamma` é um caminho fechado suave por partes em `U` então `\int_\gamma f(z) dz = 0`.

Fórmula Integral de Cauchy
--------------------------
Seja `f : U -> C` uma função holomorfa definida no domínio `U \in C`.
Sejam `\bar{D}(z_0, r_0)` um disco fechado inteiramente contido em `U` e `\Gamma` sua fronteira,
orientada compativelmente. Se `z` é um ponto qualquer no interior de `\bar{D}(z_0, r_0)`, então...
`f(z) = \frac{1}{2 * \pi * i} * \int_\Gamma \frac{f(w)}{w - z} dw`.

Colorário
---------
Seja `f : U -> C` holomorfa, onde `U` é um domínio.
Então `f` tem derivadas de todas as ordens em todos os pontos de `U` e, para todo `z \in U`,
`f^(n)(z) = \frac{n!}{2 * \pi * i} * \int_\gamma \frac{f(w)}{(w - z)^{n+1}} dw`.

Estimativas de Cauchy
---------------------
Seja `f` uma função holomorfa definida no disco `D(z_0, R)` e suponha que `|f| <= K` em `D(z_0, R)`.
Então `|f^(n)(z_0)| <= \frac{n! * K}{R^n}`.

Teorema de Liouville
--------------------
Seja `f : C -> C` uma função inteira. Se existe um número `K >= 0` tal que `|f(z)| <= K` então `f` é uma função constate.

Teorema Fundamental da Álgebra
------------------------------
Seja `P : C -> C` um polinômio não constante. Então existe um número complexo `z_0` tal que `P(z_0) = 0`.

Lema
----
Sejam `D(a, r)` (para `r > 0`) um disco e `f : D(a, r) -> C` uma função holomorfa.
Se a imagem `f(D(a, r))` está contida num círculo `|w| = \alpha` então `f` é constante.

Princípio do Módulo Máximo
--------------------------
Sejam `U` um domínio em `C` e `f : U -> C` uma função holomorfa. Suponha que existe um ponto `a \in U` tal que
`|f(a)| >= |f(z)|` para todo `z \in U`. Então `f` é uma função constante.
