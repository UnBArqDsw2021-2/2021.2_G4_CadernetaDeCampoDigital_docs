## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|--|--|--|--|
|1.0|01/02|Abertura do documento|João Pedro Moura|

## 2. Introdução
<p style="text-align: justify; text-indent: 20px"> A priorização de requisitos deve ser feita de forma mais rigorosa e analítica, segundo Wiegers (2013) [1], quando não há um consenso sobre quais requisitos devem ser os mais importantes. Sendo assim, para priorizar os requisitos analíticamente diversos métodos de priorização podem ser utilizados, sendo um deles e que tem enfoque nesse documento é o chamado <b>First Things First</b>.</p>
<p style="text-align: justify; text-indent: 20px"> Ainda segundo Wiegers (2013) [1], o <b>First Things First</b> é uma técnica que visa ajudar o relacionamento das funcionalidades com um valor estimado definido pelo representante dos clientes e pelo representante da equipe de desenvolvimento. Dessa maneira, para a realização da técnica são necessários os segunties passos:</p>

- Liste em uma tabela todas as features, casos de uso, histórias de usuários ou requisitos funcionais
- Estime o benefício relativo que cada requisito fornece ao cliente em uma escala de 1 a 9.
- Estime a penalidade relativa que o cliente sofreria caso a funcionalidade não fosse incluída em uma escala de 1 a 9.
- Adicione uma coluna que será a soma do benefício multiplicado pelo peso e da penalidade multiplicada pelo peso para cada requisito.
- Estime o custo de implementação de cada funcionalidade em uma escala de 1 a 9.
- Estime o risco da funcionalidade não ser entregue na primeira tentativa em uma escala de 1 a 9.
- Use a seguinte fórmula, para calcular a prioridade de cada requisito:

$$
prioridade = \dfrac{valor\%} {custo\% * pesoCusto + risco\% * pesoRisco}
$$

- E por fim, ordene em ordem decrescente de prioridade a tabela dos requisitos

## 3. First Things First
| Códigos das Funcionalidades | Benefício Relativo | Penalidade relativa | Valor Total | Valor % | Custo Relativo | Custo % | Risco Relativo | Risco % | Prioridade |
| :-------------------------: | :----------------: | :-----------------: | :---------: | :-----: | :------------: | :-----: | :------------: | :-----: | :--------: |
|        Peso Relativo        |         2          |          1          |      -      |    -    |       1        |    -    |      0.5       |    -    |      -     |
|                             |                    |                     |             |         |                |         |                |         |            |
|           Totais            |                    |                     |             |         |                |         |                |         |            |


## 4. Referências

> [1] Wiegers, K.; Beatty, J. Software Requirements. <b>Microsoft Press</b>. ed. 3, 2013.</p>
