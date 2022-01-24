## Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência.

**DEFINIÇÃO**:

1. Definir um conjunto de classes de Equivalência e um conjunto de casos de testes derivados, para testar a seguinte função de avaliação universitária.

2. A função avalicao, recebe como parâmtros os seguintes dados:

   2.1. **nota1** (numérico de ponto flutuante com duas casas decimais);

   2.2. **nota2** (numérico de ponto flutuante com duas casas decimais);

   2.3. **cargaHoraria** (numérico inteiro, positivo);

   2.4. **faltas** (numérico inteiro, positivo).

3. A forma de calcular a avaliação é a seguinte:

   3.1. Se a quantidade de faltas for superior a 25% da carga horária, o aluno estará reprovado por falta. Neste caso a função retorna a seguinte mensagem "Reprovado por Falta";

   3.2. Estando o aluno reprovado por falta, não haverá a necessidade de se avaliar as notas;

   3.2. Se a média entre nota1 e nota2 for menor que 3.0, o aluno estará reprovado por média. Neste caso a função retorna a seguinte mensagem "Reprovado por Média";

   3.3. Se a média entre nota1 e nota2 for >= 3.0 e < 6.0, o aluno estará em recuperação. Neste caso a função retorna a seguinte mensagem "Recuperação";

   3.4 Em qualquer outra situação o aluno estará aprovado. Então a função retornará a mensagem: "Aprovado".

4. O Conjunto de classes de Equivalência deverá ser definido seguindo o seguinte padrão:

| id   | descrição                                                                                            | V/I |
| ---- | ---------------------------------------------------------------------------------------------------- | --- |
| CE01 | nota1 < 0                                                                                            | I   |
| CE02 | nota1 > 10                                                                                           | I   |
| CE03 | nota2 < 0                                                                                            | I   |
| CE04 | nota2 > 10                                                                                           | I   |
| CE05 | cargaHoraria < 1                                                                                     | I   |
| CE06 | faltas < 0                                                                                           | I   |
| CE07 | nota1 >= 0 e nota1 <= 10, nota2 >= 0 e nota2 <= 10, faltas >= 0 e <= cargaHoraria, cargaHoraria >= 1 | V   |
| CE08 | faltas > cargaHoraria                                                                                | I   |

---

| CT   | Valor de Entrada | Resultado Esperado  | Classe Equivalência |
| ---- | ---------------- | ------------------- | ------------------- |
| CT01 | -2               | Valor Inválido      | CE01                |
| CT01 | 11               | Valor Inválido      | CE02                |
| CT03 | -1               | Valor Inválido      | CE03                |
| CT04 | 13               | Valor Inválido      | CE04                |
| CT08 | 0                | Valor inválido      | CE05                |
| CT09 | -1               | Valor inválido      | CE                  |
| CT10 | 3, 3, 1, 10      | Reprovado por média | CE07                |
| CT11 | 3, 3, 5, 10      | Reprovado por falta | CE07                |
| CT10 | 3, 4, 1, 120     | Recuperação         | CE07                |
| CT10 | 6, 10, 2, 240    | Aprovado            | CE07                |
