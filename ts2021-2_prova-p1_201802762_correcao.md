<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>

#### <p style="text-align: center;">Instituto de Informática</p>

#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>

#### <p style="text-align: center;">Teste de Software - 2021/2</p>

#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>

#### <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201802762
Nome: Fernando Severino Almeida

<p><font color=green>Nota: 9,0.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software? R.: **O objetivo primário do teste de software é revelar a presença de defeitos.** <font color=green>Certo.</font>
   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário? R.: **As chances de se obter um software que não atenda os requisitos e aceitação do cliente são aumentadas.** <font color=red>Errado.</font>
2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível. R.: **Teste exaustivo consiste em testar todas as entradas possíveis para um determinado código. Na maioria das vezes se torna inviável devido ao grande número de entradas possíveis.** <font color=green>Certo.</font>
3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.
**Teste Funcional: 1) Dependente de uma boa especificação de requisitos o que, em geral, não é bem feito. 2) Não é possível garantir que as partes essenciais ou críticas do software sejam executadas.**<br /><font color=green>Certo.</font>
**-Teste Estrutural: 1) Defeitos podem existir mesmo com o fluxo de controle correto. 2) Com o teste exaustivo O número de caminhos pode ser infinito ou muito grande. Cada decisão dobra e cada loop multiplica o número de caminhos.** <font color=green>Certo.</font>
4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada. R.: **Os quatro níveis de teste são: Testes de unidade, Tesdes de integração, Testes de sistema e testes de aceitação.**<br />
**- Testes de unidade: Consiste em validar as menores unidades da aplicação. Neste caso é necessário que se conheça o código para determinar um conjuto de entradas e as saídas correspondentes. Um exemplo é o teste estrutural (caixa-branca).** <font color=green>Certo.</font>
5. (**1.0 ponto**) Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência. R.: **Seu propósito é reduzir o número de caso de teste procurando garantir uma boa cobertura do código do produto em teste.** <font color=orange>Parcialmente correto, Nota 0,5.</font>
6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados. R.: **Sim, existe hierarquia dependendo do nível de cobertura. Ou seja, no nível de cobertura 7 cobrirá todos os níveis abaixo dele (6, 5, 4, 3, 2, 1 e 0) do mesmo modo o nível 6 cobrirá todos os níveis abaixo dele (5, 4, 3, 2, 1 e 0) e assim sucessivamente.** <font color=green>Certo.</font>
7. Considere a especificação, a seguir, de um hipotético programa que objetiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).<br />
   **As condições acima não estão corretas, logo, a definição da tabela de decisão e casos de testes seguirão as seguintes condições, (A + B > C) ou (A + C > B) ou (B + C > A)**
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;<br />
         • Escaleno = quando todos os seus lados têm medidas diferentes<br />
         • Equilátero = quando todos os lados tem a mesma medida;<br />
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).<br />
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).<br />
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.

|R1: A+B>C ou A+C>B ou B+C>A|F|V|V|V|V|V|V|V|V|
|---|---|---|---|---|---|---|---|---|---|
|R3: A=B||F|F|F|F|V|V|V|V|
|R4: B=C||F|F|V|V|F|F|V|V|
|R4: A=C||F|V|F|V|F|V|F|V|
|Não é um triângulo|X|||||||||
|Equilátero|||||||||X|
|Isóceles|||X|X||X||||
|Escaleno||X||||||||

<br/>

<font color=green>Certo.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:<br/>

|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
|01|0|0|0|Não é um triângulo|
|02|3|4|5|Escaleno|
|03|3|2|3|Isóceles|
|04|3|4|4|Isóceles|
|05|3|3|1|Isóceles|
|06|5|5|5|Equilátero|

<font color=green>Certo.</font>

INSTRUÇÕES:

1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
