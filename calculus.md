---
layout: default
title: "Cálculo Numérico"
---

<div class="flex flex-col my-6">
<div class="grid col-6 mb-6">
    <div class="max-w-md mx-auto rounded-xl overflow-hidden md:max-w-2xl p-4 m-2">

    <h1 class="mb-4 font-bold">Lagrange</h1>
    <p class="my-1">O código em Python implementa a função de interpolação de Lagrange, que é usada no cálculo numérico para estimar valores intermediários entre pontos conhecidos.</p>
    <p class="my-1">A função <code>lagrange</code> recebe dois argumentos: <code>x</code>, que é o valor para o qual queremos estimar o resultado, e <code>pontos</code>, que é uma lista de pontos no formato (x, y). A função retorna o valor interpolado para o ponto x.</p>
    <p class="my-1">A implementação utiliza o método de Lagrange, que envolve a construção de polinômios de Lagrange para cada ponto conhecido e, em seguida, somando esses polinômios ponderados. O resultado final é o valor interpolado desejado.</p>
    <p class="my-1">A variável <code class="italic">result</code> é inicializada como zero e será usada para armazenar o resultado final da interpolação. A variável <code>n</code> é definida como o número de pontos conhecidos.</p>
    <p class="my-1">Em seguida, há um loop <code>for</code> que itera sobre cada ponto conhecido. Dentro desse loop, a variável <code>term</code> é inicializada com o valor y do ponto atual.</p>
    <p class="my-1">Em seguida, há um segundo loop <code>for</code> que itera sobre todos os pontos conhecidos novamente. Dentro desse loop, é verificado se o índice <code>i</code> é diferente do índice <code>j</code>. Se forem diferentes, o termo é multiplicado por <code>(x - points[j][0]) / (points[i][0] - points[j][0])</code>. Essa é a fórmula do polinômio de Lagrange para cada ponto.</p>
    <p class="my-1">Por fim, o termo é adicionado ao resultado final <code>result</code>.</p>
    <p class="my-1">Após a definição da função <code>lagrange</code>, há a criação de uma lista de pontos <code>pontos</code> e a definição de um valor <code>x</code> para o qual queremos estimar o resultado interpolado.</p>
    <p class="my-1">Em seguida, a função <code>lagrange</code> é chamada com os argumentos <code>x</code> e <code>pontos</code>, e o resultado é armazenado na variável <code>result</code>.</p>
    <p class="my-1">Por fim, o resultado é impresso na tela usando a função <code>print</code>.</p>
    <p class="my-1">Esse código pode ser usado em uma aula de cálculo numérico para demonstrar o conceito de interpolação de Lagrange e como implementá-lo em Python.</p>

    <h2 class="my-4 font-bold">Código Python</h2>
    <pre><code>
def lagrange(x, points):
    result = 0
    n = len(points)

    for i in range(n):
        term = points[i][1]
        for j in range(n):
            if i != j:
                term *= (x - points[j][0]) / (points[i][0] - points[j][0])
        result += term

    return result

pontos = [(1, 2), (3, 4), (5, 6)]
x = 2

result = lagrange(x, pontos)

print(f"O valor interpolado para x = {x} é {result}.")
    </code></pre>

    <h1 class="my-4 font-bold">Slides</h1>
    <p class="my-1">Resolução dos slides passados na atividade.</p>

    <h2 class="my-4 font-bold">Slide 1</h2>
    <p class="my-1"><em>Exercicio --</em></p>
    <img src="/assets/imgs/images/ex1.png" alt="Slide 1">
    <p class="my-1"><em>Resultado --</em></p>
    <img src="/assets/imgs/images/ex1result.png" alt="Resultado Slide 1">

    <h2 class="my-4 font-bold">Slide 2</h2>
    <p class="my-1"><em>Exercicio --</em></p>
    <img src="/assets/imgs/images/ex2.png" alt="Slide 2">
    <p class="my-1"><em>Resultado --</em></p>
    <img src="/assets/imgs/images/ex2result.png" alt="Resultado Slide 2">

    <h2 class="my-4 font-bold">Slide 3</h2>
    <p class="my-1"><em>Exercicio --</em></p>
    <img src="/assets/imgs/images/ex3.png" alt="Slide 3">
    <p class="my-1"><em>Resultado --</em></p>
    <img src="/assets/imgs/images/ex3result.png" alt="Resultado Slide 3">

    <h1 class="my-4 font-bold">Exercicio da Folha</h1>
    <p class="my-1">Cálculo de interpolação por meio de medidas de uma folha.</p>
    <p class="my-1"><em>Folha</em>:</p>
    <img src="/assets/imgs/images/folhaport.png" alt="Folha">
    <p class="my-1"><em>Representação da Folha</em>:</p>
    <img src="/assets/imgs/images/folha_calc.png" alt="Folha Calc">
    </div>
</div>
</div>
