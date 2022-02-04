## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|------|----|---------|---------|
|1.0|28/01/2022|<center>Abertura do documento de entrevista</center>|<center>Thiago</center>|
|1.1|28/01/2022|<center>Adição da entrevista editada</center>|<center>Thiago</center>|
|1.2|28/01/2022|<center>Adição dos resultados</center>|<center>Thiago</center>|
|1.3|28/01/2022|<center>Adição dos requisitos</center>|<center>Thiago</center>|
|1.4|29/01/2022|<center>Adição da introdução</center>|<center>Thiago</center>|
|1.5|30/01/2022|<center>Adição da legenda</center>|<center>Thiago</center>|
|1.6|03/02/2022|<center>Linkagem dos léxicos</center>|<center>Thiago</center>|

## 2. Introdução
<p align = "justify"> &emsp;&emsp; Entre as diversas técnicas apresentadas por Wiegers e Beatty (2013) [1], aquela que se destacada como a forma mais óbvia de obtenção de informações é a metodologia de entrevistas. Por meio de um diálogo, formal ou informal, o entrevistado tem a chance de expressar suas necessidades e permite que o entrevistador faça diversas perguntas, a fim de obter informações sobre a aplicação em questionamento [2]. Essa técnica, portanto, é extremamente flexivel e eficiente, pois encurta o caminho do engenheiro de requisitos com seus <a href="../../modelagem/lexicos#usuario">usuários</a>.</p>

## 3. Entrevista
<p align = "justify"> &emsp;&emsp; A pessoa escolhida para a entrevista é a Engenheira Agrônoma Nadja, que atualmente trabalha na Emater-DF, visto que tem um vasto conhecimento do contexto agrícola do DF e, principalmente, do funcionamento da <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> dos produtos agrícolas pelos <a href="../../modelagem/lexicos#produtor">produtores</a> locais.</p>

<iframe width="800" height="500" src="https://www.youtube.com/embed/UyjA6WF295g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 4. Resultados
### 4.1 Introdução

- O aplicativo deve ser de fácil utilização
- O aplicativo deve ser intuitivo
- O aplicativo deve possuir textos simples
- O aplicativo deve fornecer a <a href="../../modelagem/lexicos#cardeneta_de_campo">Caderneta de Campo</a> para <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> das colheitas
- O aplicativo deve fornecer uma interface simples para o <a href="../../modelagem/lexicos#aplicar_agrotoxico">cadastro da aplicação do agrotóxico</a>
- O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ser capaz de <a href="../../modelagem/lexicos#cadastrar_plantio">cadastrar seu plantio</a>
- O produtor pode escolher em qual <a href="../../modelagem/lexicos#talhao">talhão</a> cadastrar o seu plantio
- O produtor deve ser capaz de cadastrar a aplicação de agrotóxicos
- O produtor pode cadastrar quando <a href="../../modelagem/lexicos#colher_plantio">colheu o plantio</a>
- O produtor deve ser capaz de saber o <a href="../../modelagem/lexicos#periodo_carencia">período de carência</a>
- O <a href="../../modelagem/lexicos#tecnico">técnico</a> deve ser capaz de <a href="../../modelagem/lexicos#supervisionar_propriedade">supervisionar propriedades</a>
- O técnico deve ser capaz de cadastrar <a href="../../modelagem/lexicos#cultura">culturas</a>
- O técnico deve ser capaz de cadastrar <a href="../../modelagem/lexicos#agrotoxico">agrotóxicos</a>
    
### 4.2 Você falou de vários programas, mas o foco é na rastreabilidade?
    
- O aplicativo deve garantir a <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> dos <a href="../../modelagem/lexicos#plantio">plantios</a>

### 4.3 Poderia falar sobre a Caderneta de Campo?

- O aplicativo deve fornecer a <a href="../../modelagem/lexicos#cardeneta_de_campo">Caderneta de Campo</a> para rastreabilidade das colheitas

### 4.4 Poderia falar sobre o Período de Carência?

- O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ser capaz de saber o <a href="../../modelagem/lexicos#periodo_carencia">período de carência</a>

### 4.5 Quais os produtos que são aplicados?

 - O <a href="../../modelagem/lexicos#tecnico">técnico</a> deve ser capaz de cadastrar os <a href="../../modelagem/lexicos#agrotoxico">agrotóxicos</a>
 - O técnico deve ser capaz de cadastrar <a href="../../modelagem/lexicos#tipo_agrotoxico">os tipos dos agrotóxicos</a>
 - O aplicativo deve permitir a <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> das <a href="../../modelagem/lexicos#aplicacao_agrotoxico">aplicações de agrotóxicos</a>

### 4.6 A identificação do agrotóxico é feita pela foto?

- O aplicativo deve fornecer uma interface simples para o cadastro da <a href="../../modelagem/lexicos#aplicacao_agrotoxico">aplicação do agrotóxico</a>
- O aplicativo deve permitir o cadastro da aplicação do agrotóxico pela foto        

### 4.7 Qual a quantidade de produtor por propriedade?
    
- O produtor pode cadastrar o tamanho da propriedade
- A propriedade pode ter apenas um produtor

### 4.8 O produtor pode plantar diferentes culturas ou apenas uma?

- O produtor pode plantar apenas um tipo em um <a href="../../modelagem/lexicos#talhao">talhão</a>

### 4.9 Precisa anotar a data de plantio, data da aplicação do agrotóxico e a data da colheita?

- O aplicativo deve possuir um bom desempenho
- O aplicativo deve possuir uma boa usabilidade

### 4.10  Precisa ter algum documento de identificação do produtor?  

- O aplicativo deve guardar a identificação do produtor

### 4.12 Poderia falar um pouco mais como funcionam os talhões?

- A propriedade é dividida em diversos setores chamados de talhões
- Um talhão pode conter apenas um tipo de <a href="../../modelagem/lexicos#cultura">cultura</a> plantada
- Em um talhão pode ser plantado diversas culturas em épocas diferentes

### 4.13 Como funcionam as épocas de plantio?

- Um talhão pode conter em média 3 plantios em um ano

### 4.14 Como o produtor informa onde ele plantou determinada cultura?

- Presencialmente, o técnico conhece o campo e as divisões feitas pelo produtor

### 4.15 Como é identificada uma cultura?

- A cultura é separada em espécies mas tratadas pelo nome vulgar

## 5. Requisitos

|ID|Descrição|Tipo de Requisito
|--|--|--|
|E01|O aplicativo deve ser de fácil utilização|RNF|
|E02|O aplicativo deve ser intuitivo|RNF|
|E03|O aplicativo deve possuir textos simples|RNF|
|E04|O aplicativo deve fornecer a <a href="../../modelagem/lexicos#cardeneta_de_campo">Caderneta de Campo</a> para <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> das colheitas|RF|
|E05|O aplicativo deve fornecer uma interface simples para o <a href="../../modelagem/lexicos#aplicar_agrotoxico">cadastro da aplicação do agrotóxico</a>|RNF|
|E06|O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ser capaz de cadastrar seu <a href="../../modelagem/lexicos#plantio">plantio</a>|RF|
|E07|O produtor pode escolher em qual <a href="../../modelagem/lexicos#talhao">talhão</a> cadastrar o seu <a href="../../modelagem/lexicos#plantio">plantio</a>|RF|
|E08|O produtor deve ser capaz de cadastrar a aplicação de agrotóxicos|RF|
|E09|O produtor pode cadastrar quando <a href="../../modelagem/lexicos#colher_plantio">colheu o plantio</a>|RF|
|E10|O produtor deve ser capaz de saber o <a href="../../modelagem/lexicos#periodo_carencia">período de carência</a>|RF|
|E11|O <a href="../../modelagem/lexicos#tecnico">técnico</a> deve ser capaz de <a href="../../modelagem/lexicos#supervisionar_propriedade">supervisionar propriedades</a>|RF|
|E12|O técnico deve ser capaz de cadastrar <a href="../../modelagem/lexicos#cultura">culturas</a>|RF|
|E13|O técnico deve ser capaz de cadastrar <a href="../../modelagem/lexicos#agrotoxico">agrotóxicos</a>|RF|
|E14|O técnico deve ser capaz de cadastrar os <a href="../../modelagem/lexicos#tipo_agrotoxico">tipos dos agrotóxicos</a>|RF|
|E15|O aplicativo deve garantir a rastreabilidade dos plantios|RNF|
|E16|O aplicativo deve fornecer a Caderneta de Campo para rastreabilidade das colheitas|RF|
|E17|O aplicativo deve permitir a rastreabilidade das aplicações de agrotóxicos|RF|
|E18|O aplicativo deve permitir o cadastro da aplicação do agrotóxico pela foto|RNF|
|E19|O aplicativo deve possuir um bom desempenho|RNF|
|E20|O aplicativo deve possuir uma boa usabilidade|RNF|
<h6 align = "center">Tabela 1: Tabela contendo os requisitos levantados pela entrevista</h6>
<h6 align = "center">Fonte: Autor</h6>

#### Legenda:
- E - Entrevista
- RF - Requisito Funcional
- RNF - Requisito Não Funcional

## 6. Referências

> [1] Wiegers, K.. Beatty J. Software Requirements. Third Edition. 2013

> [2] Vazquez, C.; Simões, G.; Engenharia de Requisitos: Cap. 7 - Elicitação de Requisitos. Brasport. 2016.