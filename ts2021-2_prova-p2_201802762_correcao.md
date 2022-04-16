<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201802762

Nome: Fernando Severino Almeida

<font color="green">Nota 6,73</font>

1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.
   - **Resposta:**  Processo de Software: Um conjunto de fases bem definidas sendo executadas atividades que produzem artefatos que podem servir ou não de entrada para outra atividade do processo de teste software. O principal objetivo é minimizar os riscos e agregar valor ao software; Projeto de Teste de Software: O projeto de teste descreve toda a estrutura dos elementos do teste e como será realizado os casos de teste, ou seja, é um documento que especifica os detalhes da abordagem de teste para um requisito do software ou combinação deles e identifica casos de teste associados; Plano de Teste de Software: Um plano de teste é como uma receita, uma sequencia de passos que serão realizados para que os objetivos do projeto de teste seja cumprido. <font color="red">Nota 0,5</font>

   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.
   - **Resposta:** O plano de teste e projeto de testes são artefatos de saída do processo de software. O projeto de teste descreve como serão realizados os casos de teste e a estrutura dos elementos do teste, enquanto que o plano é uma sequência de passos para a realização dos casos de teste previstos no projeto. <font color="red">Nota 0,4</font>
2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.
- **Resposta:** Software testado em partes ao invés de todo o software ser testado ao fim do desenvolvimento; várias tarefas são executadas simultaneamente, logo uma equipe não fica parada esperando todo o software ser concluído para iniciar o trabalho; é realizado por todos os membros da equipe; maior ênfase em testes exploratórios. <font color="red">Nota 1,0</font>
3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.
- **Resposta:** Execução do teste ao mesmo tempo do design de teste; Tolera documentação limitada do objetivo do teste; e depende da habilidade e conhecimento do testador para orientar o teste. <font color="red">Nota 1,0</font>
4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   1. (2.0 Pontos) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.
   - **Resposta:**

   |ID|Descrição|V/I|
   |---|---|---|
   |CE001|numero da conta menor que 6 digitos|I|
   |CE002|numero da conta maior que 6 digitos|I|
   |CE003|numero da conta igual a 6 digitos|V|
   |CE004|Tipo da conta igual a Corrente|V|
   |CE005|Tipo da conta igual a Poupança|V|
   |CE006|Tipo da conta diferente de Corrente ou Poupança|I|
   |CE007|Número do banco inteiro maior ou igual que 100 e menor que 1000|V|
   |CE008|Número do banco inteiro igual ou menor que 99|I|
   |CE009|Número do banco inteiro maior ou igual a 1000|I|
   |CE010|Nome do banco com tamanho maior ou igual a 5 e menor ou igual a 100 composto somente de letras|V|
   |CE011|Nome do banco composto por letras e números|I|
   |CE012|Nome do banco com tamanho menor que 5|I|
   |CE013|Nome do banco com tamanho maior que 100|I|
   |CE014|Numero da agencia composto por no mínimo 3 números e no máximo 5 números|V|
   |CE015|Número da agencia composto por 2 números ou menos|I|
   |CE016|Número da agencia composto por 6 números ou mais|I|
   |CE017|Nome da agencia composto por letras e números|I|
   |CE018|Nome da agencia com tamanho menor que 5|I|
   |CE019|Nome da agencia com tamanho maior que 100|I|
   |CE020|Nome da cidade da agencia composto por letras e números|I|
   |CE021|Nome da cidade da agencia com tamanho menor que 5|I|
   |CE022|Nome da cidade da agencia com tamanho maior que 100|I|
   |CE023|Nome da agencia com tamanho maior ou igual a 5 e menor ou igual a 100 composto somente de letras|V|
   |CE024|Nome da cidade da agencia com tamanho maior ou igual a 5 e menor ou igual a 100 composto somente de letras|V|

   <font color="red">Nota 1,5</font>

   2. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:

   |CT|Valores de Entrada|Resultado esperado|CE|
   |---|---|---|---|
   |CT001|123|Inválido|CE001|
   |CT002|1234567|Inválido|CE002|
   |CT003|123456|Válido|CE003|
   |CT004|Corrente|Válido|CE004|
   |CT005|Poupança|Válido|CE005|
   |CT006|Salário|Inválido|CE006|
   |CT007|333|Válido|CE007|
   |CT008|99|Inválido|CE008|
   |CT009|1000|Inválido|CE009|
   |CT010|Banco do Brasil|Válido|CE010|
   |CT011|Banco 123|Inválido|CE011|
   |CT012|ABC|Inválido|CE012|
   |CT013|BANCO AAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAAAAAAAAAAAA|Inválido|CE013|
   |CT014|234|Válido|CE014|
   |CT015|12|Inválido|CE015|
   |CT016|4567891|Inválido|CE016|
   |CT017|ABC1234|Inválido|CE017|
   |CT018|ABC|Inválido|CE021|
   |CT019|Agencia AAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAAAAAAAAAAAA|Inválido|CE018|
   |CT020|ABC1234|Inválido|CE020|
   |CT021|ABC|Inválido|CE021|
   |CT022|Cidade AAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAA<br/>AAAAAAAAAAAAAAAAAAAAAAAAAAAAA|Inválido|CE022|
   |CT023|Agencia ABC|Válido|CE023|
   |CT024|Abadia|Válido|CE024|

   <font color="red">Nota 1,0</font>

   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.


INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.
