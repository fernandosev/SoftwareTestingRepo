## Tarefa 004 - 19/01/2022 - Análise do Valor Limte - Definição de casos de testes.

**DEFINIÇÃO**:

1. Considerando o conjunto de classes de equivalência que você definiu em atendimento à **Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência**.

2. Considerando as explicações a respeito do critério de teste funcional **Análise do Valor Limite** disponíveis em:

3. [Análise do Valor Limite 1](https://viniciuspessoni.com/2020/03/15/analise-do-valor-limite/).

4. [Análise do Valor Limite 2](https://www.youtube.com/watch?v=EQU5ODvmwzs).

5. [Análise do Valor Limite 3](https://www.youtube.com/watch?v=jX7uyaTAn-k).

6. Pede-se a definição do conjunto de casos de testes necessários para o teste do mesmo cenário descrito na tarefa 003. Estes casos de teste deverão ser criadas a partir das diretrizes definidas pelo critério funcional "Análise do Valor Limte".

7. O Conjunto de casos de testes derivado deve seguir o seguinte padrão:

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
| CT01 | -1               | Valor Inválido      | CE01                |
| CT02 | 11               | Valor Inválido      | CE02                |
| CT03 | -1               | Valor Inválido      | CE03                |
| CT04 | 11               | Valor Inválido      | CE04                |
| CT05 | 0                | Valor inválido      | CE05                |
| CT06 | -1               | Valor inválido      | CE06                |
| CT07 | 0, 0, 0, 100     | Reprovado por média | CE07                |
| CT08 | 3, 3, 0, 100     | Reprovado por média | CE07                |
| CT09 | 4, 4, 0, 100     | Recuperação         | CE07                |
| CT10 | 5, 5, 0, 100     | Recuperação         | CE07                |
| CT11 | 6, 6, 0, 100     | Aprovado            | CE07                |
| CT12 | 10, 10, 0, 100   | Aprovado            | CE07                |
| CT13 | 3, 3, 25, 100    | Reprovado por falta | CE07                |
| CT14 | 10, 10, 24, 100  | Aprovado            | CE07                |
