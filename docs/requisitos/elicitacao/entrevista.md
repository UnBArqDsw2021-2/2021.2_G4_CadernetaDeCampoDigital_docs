## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|------|----|---------|---------|
|1.0|28/01|<center>Abertura do documento de entrevista</center>|<center>Thiago</center>|
|1.1|28/01|<center>Adição da entrevista editada</center>|<center>Thiago</center>|
|1.2|28/01|<center>Adição dos resultados</center>|<center>Thiago</center>|
|1.3|28/01|<center>Adição dos requisitos</center>|<center>Thiago</center>|
|1.4|29/01|<center>Adição da introdução</center>|<center>Thiago</center>|

## 2. Introdução
<p align = "justify"> &emsp;&emsp; Entre as diversas técnicas apresentadas por Wiegers e Beatty (2013) [1], aquela que se destacada como a forma mais óbvia de obtenção de informações é a metodologia de entrevistas. Por meio de um diálogo, formal ou informal, o entrevistado tem a chance de expressar suas necessidades e permite que o entrevistador faça diversas perguntas, a fim de obter informações sobre a aplicação em questionamento [2]. Essa técnica, portanto, é extremamente flexivel e eficiente, pois encurta o caminho do engenheiro de requisitos com seus usuários.</p>

## 3. Entrevista
<p align = "justify"> &emsp;&emsp; A pessoa escolhida para a entrevista é a Engenheira Agrônoma Nadja, que atualmente trabalha na Emater-DF, visto que tem um vasto conhecimento do contexto agrícola do DF e, principalmente, do funcionamento da rastreabilidade dos produtos agrícolas pelos produtores locais.</p>

<iframe width="800" height="500" src="https://www.youtube.com/embed/UyjA6WF295g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 4. Resultados
### 4.1 Introdução

- O aplicativo deve ser de fácil utilização
- O aplicativo deve ser intuitivo
- O aplicativo deve possuir textos simples
- O aplicativo deve fornecer a Caderneta de Campo para rastreabilidade das colheitas
- O aplicativo deve fornecer uma interface simples para o cadastro da aplicação do agrotóxico
- O produtor deve ser capaz de cadastrar seu plantio
- O produtor pode escolher em qual talhão cadastrar o seu plantio
- O produtor deve ser capaz de cadastrar a aplicação de agrotóxicos
- O produtor pode cadastrar quando colheu o plantio
- O produtor deve ser capaz de saber o período de carência
- O técnico deve ser capaz de supervisionar propriedades
- O técnico deve ser capaz de cadastrar culturas
- O técnico deve ser capaz de cadastrar agrotóxicos
    
### 4.2 Você falou de vários programas, mas o foco é na rastreabilidade?
    
- O aplicativo deve garantir a rastreabilidade dos plantios

### 4.3 Poderia falar sobre a Caderneta de Campo?

- O aplicativo deve fornecer a Caderneta de Campo para rastreabilidade das colheitas

### 4.4 Poderia falar sobre o Período de Carência?

- O produtor deve ser capaz de saber o período de carência

### 4.5 Quais os produtos que são aplicados?

 - O técnico deve ser capaz de cadastrar os agrotóxicos
 - O técnico deve ser capaz de cadastrar os tipos dos agrotóxicos
 - O aplicativo deve permitir a rastreabilidade das aplicações de agrotóxicos

### 4.6 A identificação do agrotóxico é feita pela foto?

- O aplicativo deve fornecer uma interface simples para o cadastro da aplicação do agrotóxico
- O aplicativo deve permitir o cadastro da aplicação do agrotóxico pela foto        

### 4.7 Qual a quantidade de produtor por propriedade?
    
- O produtor pode cadastrar o tamanho da propriedade
- A propriedade pode ter apenas um produtor

### 4.8 O produtor pode plantar diferentes culturas ou apenas uma?

- O produtor pode plantar apenas um tipo em um talhão

### 4.9 Precisa anotar a data de plantio, data da aplicação do agrotóxico e a data da colheita?

- O aplicativo deve possuir um bom desempenho
- O aplicativo deve possuir uma boa usabilidade

### 4.10  Precisa ter algum documento de identificação do produtor?  

- O aplicativo deve guardar a identificação do produtor

### 4.12 Poderia falar um pouco mais como funcionam os talhões?

- A propriedade é dividida em diversos setores chamados de talhões
- Um talhão pode conter apenas um tipo de cultura plantada
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
|E01|O aplicativo deve ser de fácil utilização|Requisito Não Funcional|
|E02|O aplicativo deve ser intuitivo|Requisito Não Funcional|
|E03|O aplicativo deve possuir textos simples|Requisito Não Funcional|
|E04|O aplicativo deve fornecer a Caderneta de Campo para rastreabilidade das colheitas|Requisito Funcional|
|E05|O aplicativo deve fornecer uma interface simples para o cadastro da aplicação do agrotóxico|Requisito Não Funcional|
|E06|O produtor deve ser capaz de cadastrar seu plantio|Requisito Funcional|
|E07|O produtor pode escolher em qual talhão cadastrar o seu plantio|Requisito Funcional|
|E08|O produtor deve ser capaz de cadastrar a aplicação de agrotóxicos|Requisito Funcional|
|E09|O produtor pode cadastrar quando colheu o plantio|Requisito Funcional|
|E10|O produtor deve ser capaz de saber o período de carência|Requisito Funcional|
|E11|O técnico deve ser capaz de supervisionar propriedades|Requisito Funcional|
|E12|O técnico deve ser capaz de cadastrar culturas|Requisito Funcional|
|E13|O técnico deve ser capaz de cadastrar agrotóxicos|Requisito Funcional|
|E14|O técnico deve ser capaz de cadastrar os tipos dos agrotóxicos|Requisito Funcional|
|E15|O aplicativo deve garantir a rastreabilidade dos plantios|Requisito Não Funcional|
|E16|O aplicativo deve fornecer a Caderneta de Campo para rastreabilidade das colheitas|Requisito Funcional|
|E17|O aplicativo deve permitir a rastreabilidade das aplicações de agrotóxicos|Requisito Funcional|
|E18|O aplicativo deve permitir o cadastro da aplicação do agrotóxico pela foto|Requisito Não Funcional|
|E19|O aplicativo deve possuir um bom desempenho|Requisito Não Funcional|
|E20|O aplicativo deve possuir uma boa usabilidade|Requisito Não Funcional|
<h6 align = "center">Tabela 1: Tabela contendo os requisitos levantados pela entrevista</h6>
<h6 align = "center">Fonte: Autor</h6>

## 6. Bibliografia

- [1] Wiegers, K.. Beatty J. Software Requirements. Third Edition. 2013
- [2] Vazquez, C.; Simões, G.; Engenharia de Requisitos: Cap. 7 - Elicitação de Requisitos. Brasport. 2016.