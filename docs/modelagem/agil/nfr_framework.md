## 1. Versionamento

| Versão | Data  | Descrição                              | Autor(es)       |
| ------ | ----- | -------------------------------------- | --------------- |
| 1.0 | 14/02/2022 | Abertura do documento de NFR Framework | João Pedro |

## 2. Introdução
<p style="text-align: justify; text-indent: 20px">Diversas técnicas podem ser utilizadas para a análise e modelagem dos requisitos funcionais, porém poucas delas são capazes de realizar essa função dentro dos requisitos não funcionais. Para isso, a equipe escolheu utilizar o NFR Framework como uma maneira de representar e analisar esses requisitos não funcionais do projeto, permitindo aos desenvolvedores realizar a implementação de uma solução personalizada que faz o uso desses dois tipos possíveis de requisitos, bem como prioridades e cargas de trabalho do domínio [1].</p>
<p style="text-align: justify; text-indent: 20px">Essa metodologia de modelagem tem como principal objetivo decompor os requisitos não funcionais a niveis operacionas. Dessa maneira, facilita-se a compreensão, priorização, implementação e garantia das expectativas dos <i>stakeholders</i> do sistema em questão que necessitam ser atendidos.</p>

## 3. Metodologia
<p style="text-align: justify; text-indent: 20px">Para definir os temas que estarão sendo abordados em cada diagrama NFR, a equipe utilizou a seleção dos requisitos não funcionais já documentados na <a href="../especificacao_suplementar">especificação suplementar</a>. Além desses, com o decorrer da criação do diagrama a equipe identificou novos requisitos não funcionais que ainda não haviam sido elicitados e que podem e devem estar incluídos dentro do projeto.</p>

Para sua construção, portanto, foram utilizados os seguintes relacionamentos entre softgoals [1]: 

* **AND**: Usado caso <b>os</b> softgoals descendentes forem satisfeitos, os seus ascendentes também serão.
* **OR**: Usado caso <b>algum</b> dos softgoals descendentes forem satisfeitos, os seus ascendentes também serão.
* **MAKE (++)**: Usado caso o softgoal descendente for satisfeito, os seus ascendentes serão fortemente satisfeitos.
* **HELP (+)**: Usado caso o softgoal descendente for satisfeito, os seus ascendentes serão fracamente satisfeitos.
* **HURT (-)**: Usado caso o softgoal descendente for satisfeito, os seus ascendentes serão fracamente negados.
* **BREAK (--)**: Usado caso o softgoal descendente for satisfeito, os softgoals ascendentes serão fortemente negados.

E por fim, para a elaboração/propagação serão utilizados os seguintes elementos:

* <img src="https://user-images.githubusercontent.com/74625814/132792024-ea80c111-9026-4d63-a9ea-7d1fcdfa3f67.png" width="50"/> Satisfeito.
* <img src="https://user-images.githubusercontent.com/74625814/132792077-05580cd5-a83f-4437-94fc-67e15b82aafa.png" width="50"/> Negado.
* <img src="https://user-images.githubusercontent.com/74625814/132791951-ffad085e-c92e-47d0-9cdd-e3aedefc58e2.png" width="50"/> Fracamente satisfeito. 
* <img src="https://user-images.githubusercontent.com/74625814/132792526-b64033fa-2bf4-449c-9e96-0263a458c3d4.png" width="50"/> Fracamente negado.

## 4. Gráficos de Interdependência de Softgoal

### 4.1 Usabilidade
#### 4.1.1 Sem progpagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 1: SIG de usabilidade</h6>
<h6 align = "center">Fonte: Autor</h6>

#### 4.1.2 Com propagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 2: SIG de usabilidade com propagaçao</h6>
<h6 align = "center">Fonte: Autor</h6>

### 4.2 Confiabilidade
#### 4.2.1 Sem progpagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 3: SIG de confiabilidade</h6>
<h6 align = "center">Fonte: Autor</h6>

#### 4.2.2 Com propagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 4: SIG de confiabilidade com propagação</h6>
<h6 align = "center">Fonte: Autor</h6>

### 4.5 Desempenho
#### 4.5.1 Sem progpagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 5: SIG de desempenho</h6>
<h6 align = "center">Fonte: Autor</h6>

#### 4.5.2 Com propagação

<!-- <img class="zoom" src="../../asets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 6: SIG de desempenho com propagação</h6>
<h6 align = "center">Fonte: Autor</h6>

### 4.7 Suportabilidade
#### 4.2.1 Sem progpagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 7: SIG de suportabilidade</h6>
<h6 align = "center">Fonte: Autor</h6>

#### 4.2.2 Com propagação

<!-- <img class="zoom" src="../../assets/modelagem/agil/.png"> -->
<h6 align = "center">Figura 8: SIG de suportabilidade com propagação</h6>
<h6 align = "center">Fonte: Autor</h6>

## 5. Referências 

<p style="text-align: justify; text-indent: 20px">[1] SILVA, Reinaldo Antônio da. <b>NFR4ES:Um Catálogo de Requisitos Não-Funcionais para Sistemas Embarcados</b>. Recife, 2019</p>
