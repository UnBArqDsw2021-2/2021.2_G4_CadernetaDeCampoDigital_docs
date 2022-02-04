## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|--|--|--|--|
|1.0|01/02|Abertura do documento|João Pedro Moura|
|1.1|01/02|Confecção da planilha de priorização|João Pedro Moura e Denniel|
|1.2|03/02|Linkagem dos léxicos|Thiago|

## 2. Introdução
<p style="text-align: justify; text-indent: 20px"> A priorização de requisitos deve ser feita de forma mais rigorosa e analítica, segundo Wiegers (2013) [1], quando não há um consenso sobre quais requisitos devem ser os mais importantes. Sendo assim, para priorizar os requisitos analíticamente diversos métodos de priorização podem ser utilizados, sendo um deles e que tem enfoque nesse documento é o chamado <b>First Things First</b>.</p>
<p style="text-align: justify; text-indent: 20px"> Ainda segundo Wiegers (2013) [1], o <b>First Things First</b> é uma técnica que visa ajudar o relacionamento das funcionalidades com um valor estimado definido pelo representante dos clientes e pelo representante da equipe de desenvolvimento. Dessa maneira, para a realização da técnica são necessários os seguintes passos:</p>

- Liste em uma tabela todas as features, casos de uso, histórias de <a href="../../modelagem/lexicos#usuario">usuários</a> ou requisitos funcionais
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
|E08|8|9|25|4,931|4|2,721|5|3,049|1,161|
|I08|8|9|25|4,931|5|3,401|3|1,829|1,142|
|BS14|7|8|22|4,339|4|2,721|4|2,439|1,101|
|I13|9|7|25|4,931|3|2,041|8|4,878|1,101|
|E06|8|9|25|4,931|5|3,401|4|2,439|1,067|
|E07|8|6|22|4,339|4|2,721|5|3,049|1,022|
|BS02|6|6|18|3,550|3|2,041|5|3,049|0,996|
|BS01|5|5|15|2,959|3|2,041|4|2,439|0,907|
|E04|9|9|27|5,325|8|5,442|2|1,220|0,880|
|BS20|8|8|24|4,734|6|4,082|5|3,049|0,844|
|BS21|8|8|24|4,734|6|4,082|6|3,659|0,801|
|E17|8|9|25|4,931|8|5,442|3|1,829|0,776|
|I01|7|8|22|4,339|9|6,122|1|0,610|0,675|
|E11|7|7|21|4,142|7|4,762|5|3,049|0,659|
|BS12|6|7|19|3,748|6|4,082|6|3,659|0,634|
|I12|2|2|6|1,183|1|0,680|4|2,439|0,623|
|I09|5|5|15|2,959|5|3,401|6|3,659|0,566|
|E10|4|2|10|1,972|2|1,361|7|4,268|0,564|
|ST05|4|6|14|2,761|5|3,401|5|3,049|0,561|
|BS03|3|4|10|1,972|3|2,041|5|3,049|0,553|
|BS11|5|5|15|2,959|6|4,082|5|3,049|0,528|
|I16|6|6|18|3,550|7|4,762|8|4,878|0,493|
|ST06|4|4|12|2,367|4|2,721|7|4,268|0,487|
|BS09|2|2|6|1,183|1|0,680|6|3,659|0,472|
|BS10|5|5|15|2,959|8|5,442|4|2,439|0,444|
|I06|2|2|6|1,183|1|0,680|7|4,268|0,420|
|BS08|3|2|8|1,578|3|2,041|6|3,659|0,408|
|I05|3|2|8|1,578|3|2,041|7|4,268|0,378|
|I02|4|3|11|2,170|5|3,401|8|4,878|0,371|
|E13|3|2|8|1,578|5|3,401|7|4,268|0,285|
|BS05|2|2|6|1,183|7|4,762|6|3,659|0,180|
|        Peso Relativo        |         2          |          1          |      -      |    -    |       1        |    -    |      0.5       |    -    |      -     |
|           Totais            |                    |                     |     507     |         |      147       |         |      164       |         |    21,100  |


<h6 align = "center">Tabela 1: Tabela contendo os requisitos priorizados</h6>
<h6 align = "center">Fonte: Autores</h6>

<center>

|Legenda|Descrição|
|:--:|:--:|
|I|Introspecção|
|BS|Brainstorm|
|ST|Storytelling|
|E|Entrevista|

<h6>Tabela 2: Legenda dos acrônimos contidos na Tabela 1</h6>
<h6>Fonte: Autores</h6>

</center>

## 4. Referências

> [1] Wiegers, K.; Beatty, J. Software Requirements. <b>Microsoft Press</b>. ed. 3, 2013.</p>
