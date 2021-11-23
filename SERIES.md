Séries
======

A definição de convergência para sequências e séries segue a mesma ideia trocando o valor absoluto pelo módulo.
Notamos que para uma sequência de números complexos da forma (z_n) cada elemento [zn = a_n + i*b_n] onde (a_n) e (b_n) são sequências reais,
(z_n) -> w = a + i*b <=> (a_n) -> a /\ (b_n) -> b
Essa equivalência pode ser mostrada usando a desigualdade triangular.

Propriedades
============
Sendo (z_n) e (w_n), e lim_{n->∞} z_n = α e lim_{n->∞} w_n = β.
1. lim_{n->∞} c*z_n = c*α onde c ∈ ℂ é um número qualquer
2. lim_{n->∞} (z_n + w_n) = α + β
3. lim_{n->∞} (z_n * w_n) = α * β
4. lim_{n->∞} (1/z_n) = 1/α sempre que α /= 0
Como no caso real, o problema principal para séries será determinar se elas convergem ou não.
Para isto temos vários dos conhecidos critérios desenvolvidos para o caso real.

Teorema 2 (Princípio de Cauchy)
===============================
Uma sequência (z_n) converge se, e somente se, dado qualquer número ϵ > 0 é possível encontrar n_0 natural tal que
n, m >= n_0 -> |z_m - z_n| < ϵ

[[ Nota pessoal ]]
Em outras palavras, lim_{n->∞} |z_n - z_{n-1}| = 0.

Definição 3
===========
Uma série numérica (s_n) é a sequência de somas parciais gerada por uma sequência de números complexos z_n.
Se a série s_n converge (para s) dizemos que a soma de s_n é s. A série é denotada por
\sum_{n=0}^∞ z_n → L <=> (s_n) → L

Como com sequências, para o caso das séries também notamos que [z_n = x_n + i*y_n].
\sum_{n=1}^∞ z_n = \sum_{n=1}^∞ (x_n + i*y_n)
Converge, se e somente se as séries [\sum_{n=1}^∞ x_n] e [\sum_{n=1}^∞ y_n] convergem.
Assim temos versões complexas dos critérios conhecidos para séries de números reais.

Proposição (Critério de Comparação)
===================================
Sejam [\sum a_n] e [\sum b_n] duas séries numéricas onde
[a_n, b_n >= 0 \forall n, para a_n, b_n reais] suponha que [a_n >= b_n].
1. Se [\sum b_n] converge -> [\sum a_n] converge
2. Se [\sum a_n] diverge -> [\sum b_n] diverge

Proposição
==========
Seja [\sum a_n] uma série numérica de números complexos.
Se [\sum a_n] converge então (a_n) → 0.

Demonstração
------------
Pelo critério de Cauchy,
0 = lim_{n->∞} |s_n - s_{n-1}| = lim_{n->∞} |a_n| = 0

Definição
=========
A série numérica [\sum z_n] é dita absolutamente convergente se a série [\sum |z_n|] for convergente.

Proposição
==========
Se a série [\sum z_n] é absolutamente convergente, então ela é convergente.

Lembrete
========
A série geométrica [\sum r^n] converge para \frac{1}{1-r} para 0 < r < 1
                              diverge para valores de r em que |r| >= 1

Séries de Potências
###################

Uma série de funções é uma série definida por sequências tais que para cada n natural associamos uma f_n(z) função de uma variável complexa z.
Vamos estudar principalmente sequências de potências de z, isto é, f_n(z) = a_n*z^n onde a_n é um número complexo.

Definição
=========
Dada uma sequência (a_n*z^n) a série gerada com ela é chamada de série de potência de centro 0 e denotada [\sum_{n=0}^∞ a_n*z^n].
Note-se que
[s_0 = a_0],
[s_1(z) = a_0 + a_1*z],
[s_2(z) = a_0 + a_1*z + a_2*z^2],
...
Para cada n natural, a soma parcial s_n é um polinômio de grau n.
O problema principal será estudar [\sum_{n=0}^∞ a_n*z^n <=> lim_{n->∞} s_n].
A convergência aqui será para uma função na variável z (no caso, f(z)).

[[ Nota pessoal ]]
Por exemplo, lembre-se que a função seno pode ser definida por uma série de potências.

A pergunta aqui é [\sum a_n*z^n → f(z)]?
Poderia acontecer que a convergência se tem para todo z complexo ou só para algum subconjunto contido nos complexos.

Proposição
==========
Seja [\sum_{n=0}^∞ a_n*z^n] uma série de potências.
1. Suponha que exista um número complexo [z_1 /= 0] para o qual a série converge, isto é, [lim_{n->∞} S_n(z_1)] existe.
   Então a série converge absolutamente para qualquer que seja o número z sempre que |z| < |z_1|.
2. Suponha que exista um número complexo [z_2 /= 0] para o qual a série diverge, isto é, [lim_{n->∞} S_n(z_1)] não existe.
   Então a série diverge para qualquer que seja o número z sempre que |z| > |z_2|.

[[ Nota pessoal ]]
Estamos usando aqui o Princípio da Comparação de séries, usando o módulo de números complexos como critério.
No caso de séries de potências, cada termo é da forma a_n*z^n. Como z pode variar, a convergência de f(z) depende de z.

[[ Nota pessoal ]]
Aqui fica evidente a introdução do conceito de raio de convergência, porque se para alguns z distantes de r<R da origem, a série de potências converge,
e para outros, em que r>R, diverge, então fica delineado um círculo de raio R que delimita os números complexos para os quais a série converge ou não.

Demonstração (1)
----------------
Se [\sum a_n*z_1^n] converge, então (a_n*z_1^n) → 0 para n → ∞.
Essa sequência é limitada por K > 0. Ou seja, para todo n, |a_n*z_1^n| < K, seja z complexo tal que |z| < |z_1|, ponha r = |z|/|z_1| < 1.
|a_n*z^n| = |a_n|*|z|^n = |a_n|*|z_1|^n*(\frac{|z|^n}{|z_1|^n}) = |a_n|*|z_1|^n*r^n < K*r^n
A série [\sum K*r^n] é uma série geométrica. Essa série converge para \frac{K}{1-r}.
Então [\sum a_n*z^n] < [\sum K*r^n] como a série da direita converge temos que pelo critério de comparação a série
[\sum a_n*z^n] converge absolutamente, e assim tabém converge.

Demonstração (2)
----------------
Dica: escolha z_2 tal que |z_1| < |z_2|.
Lema: Dada uma série de potências [\sum a_n*z^n] existe um disco fechado de centro 0 tal que a série é convergente dentro e divergente fora.

Definição
=========
O raio R do disco dado pelo lema anterior é chamado de raio de convergência da série [\sum a_n*z^n].

Proposição
==========
Considere uma série de potências [\sum a_n*z^n] tal que [a_n /= 0] para todo natural n.
Então seu raio de convergência R é dado pelas expressões
R = lim_{n→∞} |\frac{a_n}{a_{n+1}}|
R = \frac{1}{lim_{n→∞} |a_n|^{1/n}}
sempre que esses limites existem.

Demonstração
------------
Seja z tal que 0 < |z| < R
|\frac{a_{n+1}*z^{n+1}}{a_n*z^n}| = \frac{|a_{n+1}|*|z^{n+1}|}{|a_n|*|z^n|} = |\frac{a_{n+1}}{a_n}|*|z|
Temos que lim_{n→∞} |\frac{a_{n+1}}{a_n}|*|z| = |z|/R < 1
Seja α > 0 tal que |z|/R < α < 1
Podemos achar um n_0 tal que (|\frac{a_{n+1}}{a_n}|*|z|) < α \forall n >= n_0
|a_{n_0+1}|*|z|^{n_0+1} < |a_{n_0}|*|z|^{n_0}*α
|a_{n_0+2}|*|z|^{n_0+2} < |a_{n_0+1}|*|z|^{n_0+1}*α < |a_{n_0}|*|z|^{n_0}*α^2
...
|a_{n_0+k}|*|z|^{n_0+k} < ... < |a_{n_0}|*|z|^{n_0}*α^k
\sum_{k=0}^∞ |a_{n_0+k}|*|z|^{n_0+k} < \sum_{k=0}^∞ |a_{n_0}|*|z|^{n_0}*α^k
                                           ^ é uma série geométrica como α < 1
                                             a série da direita converge e pelo critério
                                             de comparação a série da esquerda também converge
Notamos que
\sum_{n=0}^∞ |a_n|*|z|^n = |a_0| + |a_1|*|z| + ... + |a_{n_0-1}|*|z|^{n_0-1} + \sum_{k=0}^∞ |a_{n_0+k}|*|z|^{n_0+k}
Portanto [\sum a_n*z^n] converge absolutamente e isto implica que também converge de maneira condicional.
Para terminar considere |z|>R e escolha |z|/R > β > 1 e mostre que [\sum a_n*z^n] diverge.

[[ Nota pessoal ]]
Note que o valor de R dado pela fórmula é o limite superior para o módulo de z.
Isto é, para algumas séries de potência, existem valores de z tal que |z| = R e a série diverge.
Em outras palavras, a série garantidamente converge no *interior* do disco de raio R centrado na origem.

Proposição
==========
Seja [f(z) = \sum a_n*z^n] uma série de potência com raio de convergência R > 0. Então a série
[g(z) = \sum n*a_n*z^{n-1}] converge absolutamente para |z| < R.

[[ Nota de aula ]]
g(z) = f'(z)

Demonstração
------------
Seja 0 < r < 1 então a série [\sum n*r^{n-1}] converge para \frac{1}{(1-r)^2}.
Seja z complexo tal que |z| < R, escolha α tal que |z| < α < R.
Como [\sum a_n*z^n] converge absolutamente para |z| < R, a sequência |a_n*α^n| é limitada, isto é
existe K > 0 tal que |a_n*α^n| = |a_n|*α^n < K => |a_n| < K/α^n para todo n natural.
Note que |n * a_n * z^{n-1}| = n * |a_n| * |\frac{z}{α}|^{n-1} * α^{n-1}
                             < n * (K/α^n) * |\frac{z/α}|^{n-1} * α^{n-1}
                             = n * K/α * |z/α|^{n-1}
Denotamos |z/α| = r < 1
|n * a_n * z^{n-1}| < n * (K/α) * r^{n-1}
Temos agora [\sum n * |a_n*z^{n-1}| <= K/α \sum n*r^{n-1} onde r<1
Essa série da direita converge pelo lema e assim conclui a demonstração.

Teorema
=======
Seja [f(z) = \sum a_n*z^n] uma série de potência com raio de convergência R > 0. Então a série
[g(z) = \sum n*a_n*z^{n-1}] converge absolutamente para |z| < R. Isto é, podemos derivar termo
a termo uma série de potências no interior de seu disco de convergência!

Proposição
==========
Sejam [\sum a_n*z^n] e [\sum b_n*z^n] duas séries de potências com raios R1 e R2 respectivamente então
1) [\sum c*a_n*z^n] tem o mesmo raio de convergência R1, para qualquer [c] complexo.
2) [\sum (a_n+b_n)*z^n = \sum a_n*z^n + \sum b_n*z^n]. Aqui o raio de convergência será [R = min{R1, R2}].
3) [\sum c_n*z^n = (\sum a_n*z^n)*(\sum b_n*z^n)] tem raio de convergência [R = min{R1, R2}].

Colorário
=========
Seja f(z) = [\sum a_n*z^n] uma série de potências com raio de convergência de R. Então f(z) tem derivadas
de todas as ordens no disco D(0, R).

[[ Nota pessoal ]]
É fácil notar isso por indução na derivada de f.

Proposição
==========
Seja f(z) definida pela série de potências [\sum a_n*z^n] com raio R > 0 então f é dada pela sua série de Taylor de centro 0
f(z) = \sum_{n=0}^∞ \frac{f^(n) (0)}{n!}*z^n para todo z tal que |z| < R

Demonstração
------------
Sabemos que S_n(z_0) = 0.
S_n(z) é um polinômio em z. Portanto esse polinômio é contínuo em z_0 e assim podemos achar um δ > 0 tal que
0 < |z - z_0| < δ => |S_n(z) - Sn(z_0)| < ϵ/2 => |S_n(z)| < ϵ/2
Colocando tudo junto, usando desigualdade triangular
|F(z)| <= |S_n(z)| + |F(z) - S_n(z)|
       <  ϵ/2 + ϵ/2 = ϵ
lim_{z→z_0} F(z) = 0
F(z) = \frac{f(z)-f(z_0)}{z-z_0} - g(z_0)
Implica que f'(z_0) = g(z_0) para todo z tal que |z| < R.

Séries de potências não centradas no zero
=========================================

Para séries não centradas na origem, isto é, onde aparece (z - z_0)^n em vez de z^n,
a análise feita até agora se aplica aqui, agora os conjuntos onde as séries convergem serão
{ z ∈ ℂ : |z - z_0| < R } onde R é o raio de convergência.

Vamos estudar os zeros de funções holomorfas começando com polinômios. Seja
P(z) = b_0 + b_1 * z + b_2 * z^2 + ... + b_n * z^n
Se, para algum [z_0 ∈ ℂ], [P(z_0) = 0], esse número z_0 é chamado de zero de P(z).

Considere a série de Taylor do polinômio centrada em z_0.
P(z) = a_0 + a_1 * (z - z_0) + ... + a_n * (z - z_0)^n
Como [P(z_0) = 0], é fácil ver que [a_0 = 0].
Podemos assim fatorar P(z) como P(z) = (z - z_0) * (a_1 + a_2 * (z - z_0) + ... + a_n * (z - z_0)^{n-1})
Se a_1 for 0, podemos ainda fatorar P(z) como P(z) = (z - z_0)^2 * (a_2 + a_3 * (z - z_0) + ... + a_n * (z - z_0)^{n-2})
Poderiamos fazer isso até um a_i não ser 0, ou então todos a_i seriam zeros e P(z) = 0 para todo z.
No primeiro caso, existe um k <= n tal que a_i = 0 para i <= k mas a_k /= 0.
Dizemos nesse caso que z_0 é zero de P de ordem k ou de multiplicidade k.
Isto quer dizer que P(z) = (z - z_0)^k * Q(z) sendo a_k = Q(z_0) != 0
Como polinômios são contínuos, se ϵ = |a_k|/2 existe um δ > 0 tal que
0 < |z - z_0| < δ => |Q(z) - a_k| < |a_k|/2 => |Q(z)| > |a_k|/2 > 0
Tal que Q(z) /= 0 para z contido em D(z_0, δ)

Proposição
==========
Seja [f(z) = \sum a_n * (z - z_0)^n] uma série de potências com raio de convergência [R > 0] e não identicamente nula.

[[ Nota pessoal ]]
Uma série de potências é identicamente nula se a_i = 0 para todo i.

Se [f(z_0) = a_0 = 0] então existe um disco aberto de raio [δ <= R], de centro [z_0] tal que [f(z) /= 0] para todo [z] nesse disco.

[[ Nota pessoal ]]
Note que se [f(z_0) = 0], isso quer dizer que z_0 é zero da função f(z).

[[ Nota pessoal ]]
Chamamos assim z_0 de um zero isolado.

Teorema
=======
Seja [f(z) = \sum a_n * (z - z_0)^n] uma série de potências com raio de convergência R > 0.
Suponha que exista uma sequência não constante (α_m) tal que [lim_{m→∞} α_m = z_0] e [f(α_m) = 0] para todo [m].
Então a série de potências é identicamente nula, ou seja, [a_n = 0] para todo [n].
Em outras palavras, isso significa que [z_0] não é um zero isolado.

Proposição
==========
Seja [\sum_{n=0}^∞ a_n*z^n] uma série com raio de convergência R > 0 e tal que [a_0 /= 0].
Então existe um [δ > 0] e uma série [\sum_{n=0}^∞ b_n*z^n], absolutamente convergente para [|z| < δ] e verificando
[(\sum a_n*z^n)*(\sum b_n*z^n) = 1].

Definição
=========
Sejam U um domínio nos complexos e f uma função de U nos complexos.
Suponha que f é analítica em U se, para todo ponto z_0 em U, f se expressa como uma série de potências de centro em z_0 com raio de convergência R_{z_0} > 0.
Formalmente, f é analítica em U <=> f(z) = \sum a_n*(z - z_0)^n para todo z_0 em U.
