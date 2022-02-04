# Introspecção

## 1. Versionamento
Versão|Data|Descrição|Autor(es)
------|----|---------|--------
1.0   | 29/01/2022 | Criação do documento | Rafael
1.1   | 30/01/2022 | Adição da introspecção e da tabela com os requisitos levantados| Rafael
1.2   | 03/02/2022 | Linkagem dos léxicos| Thiago

## 2. Introdução

<p style="text-align: justify; text-indent: 20px">A Introspecção é uma técnica mais voltada para o especialista de requisitos, ele deve abstrair as melhores informações a partir de uma análise de como e quais seriam os melhores requisitos para satisfazer os <a href="../../modelagem/lexicos#usuario">usuários</a> e os stakeholders do sistema, normalmente é uma técnica muito rica e profunda, porém pode não ser adequada quando não é um especialista da área realizando, mesmo assim vamos realizá-la buscando extrair ao máximo suas vantagens. </p>

## 3. Desenvolvimento da Introspecção

<p style="text-align: justify; text-indent: 20px"> O intuito será descrever a perspectiva dos <a href="../../modelagem/lexicos#usuario">usuários</a> que irão fazer o uso do aplicativo.</p>

### 3.1 Acesso inicial:

* Deve haver opção de login e cadastro para ambos os <a href="../../modelagem/lexicos#usuario">usuários</a> (<a href="../../modelagem/lexicos#produtor">produtor</a> e <a href="../../modelagem/lexicos#tecnico">técnico</a>).
* O usuário já cadastrado deve poder recuperar sua senha.
* Aplicativo deve ser limpo, intuitivo e acessível visto que o público alvo pode ter dificuldade com as tecnologias.
* O aplicativo deve ser seguro para garantir o <a href="../../modelagem/lexicos#rastreabilidade">rastreamento</a> das <a href="../../modelagem/lexicos#plantio">plantações</a>.

### 3.2.1 Tela principal (Produtor)

* Deve poder <a href="../../modelagem/lexicos#visualizar_propriedade">visualizar suas propriedades</a>.
* Deve poder <a href="../../modelagem/lexicos#visualizar_plantio">visualizar suas plantações</a>, bem como o <a href="../../modelagem/lexicos#plantio_plantado">status</a> de cada uma.
* Deve poder <a href="../../modelagem/lexicos#cadastrar_plantio">cadastrar uma plantação</a>.
* Deve ter uma área para o <a href="../../modelagem/lexicos#visualizar_plantio">histórico de suas plantações</a> e aplicações.
* Deve ter uma área para visualizar o perfil do(s) <a href="../../modelagem/lexicos#tecnico">técnico</a>(s) responsável(is) pela(s) sua(s) <a href="../../modelagem/lexicos#propriedade">propriedade</a>(s).

### 3.2.2 Tela principal (Técnico)

* Deve poder <a href="../../modelagem/lexicos#analisar_aplicacao_agrotoxico">visualizar as fotos dos agrotóxicos</a> enviadas pelos produtores.
* Deve poder <a href="../../modelagem/lexicos#visualizar_propriedade">visualizar as propriedades</a> que está supervisionando.
* Deve ter uma área para visualizar o perfil dos <a href="../../modelagem/lexicos#produtor">produtores</a> que está sendo responsável.

### 3.3 Tela de plantação:
* Deve poder visualizar as informações de <a href="../../modelagem/lexicos#talhao">talhão</a>, produto, datas, aplicações.
* O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ter acesso a uma área de uso simples para <a href="../../modelagem/lexicos#aplicar_agrotoxico">cadastrar o uso de agrotóxico</a>.
* O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola dessa <a href="../../modelagem/lexicos#plantio">plantação</a>.
* O técnico deve poder editar as informações necessárias (<a href="../../modelagem/lexicos#agrotoxico">agrotóxico</a>, datas).
* Deve poder adicionar data de colheita encerrando essa plantação.

### 3.4 Tela de agrotóxicos

* O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ter a opção de cadastrar apenas a foto do agrotóxico e a data da aplicação.
* O produtor pode programar o uso de um agrotóxico.
* O técnico deve poder editar todas as informações, exceto a foto cadastrada.
* A interface deve ter boa usabilidade para garantir uma boa rastreabilidade.

### 3.5 Tela de perfil
* O <a href="../../modelagem/lexicos#usuario">usuário</a> deve poder editar suas informações pessoais.
* O usuário deve ter acesso a informações pertinentes ao uso do app (<a href="../../modelagem/lexicos#plantio_finalizado">plantações concluídas</a>, <a href="../../modelagem/lexicos#aplicacao_agrotoxico">agrotóxicos utilizados</a>).


## 4. Requisitos levantados
|ID|Descrição|Tipo de Requisito
|--|--|--|
|I01|Cadastro e login de <a href="../../modelagem/lexicos#usuario">usuário</a> com opção de recuperar senha|RF|
|I02|O <a href="../../modelagem/lexicos#produtor">produtor</a> deve visualizar suas <a href="../../modelagem/lexicos#propriedade">propriedades</a>|RF|
|I03|O produtor deve <a href="../../modelagem/lexicos#cadastrar_plantio">cadastrar uma plantação</a>|RF|
|I04|O produtor pode visualizar o histórico de suas <a href="../../modelagem/lexicos#visualizar_plantio">plantações</a> e <a href="../../modelagem/lexicos#visualizar_aplicacao_agrotoxico">agrotóxicos</a>|RF|
|I05|O produtor pode visualizar o perfil do <a href="../../modelagem/lexicos#tecnico">técnico</a> que está monitorando sua propriedade|RF|
|I06|O produtor pode visualizar o <a href="../../modelagem/lexicos#plantio_plantado">status de cada plantação</a>|RF|
|I07|O produtor deve <a href="../../modelagem/lexicos#aplicar_agrotoxico">cadastrar o uso do agrotóxico</a> com foto e data apenas|RF|
|I08|O técnico deve ter <a href="../../modelagem/lexicos#analisar_aplicacao_agrotoxico">acesso a foto dos agrotóxicos</a> enviadas pelos produtores|RF|
|I09|O técnico deve <a href="../../modelagem/lexicos#visualizar_propriedade">visualizar as propriedades</a> supervisionadas por ele|RF|
|I10|O aplicativo deve ter uso simples|RNF|
|I11|O usuário deve <a href="../../modelagem/lexicos#visualizar_plantio">visualizar as informações das plantações</a> responsáveis|RF|
|I12|O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola plantado|RF|
|I13|O produtor deve adicionar a data de colheita <a href="../../modelagem/lexicos#plantio_finalizado">encerrando a plantação</a>|RF|
|I14|O produtor pode programar o uso de um agrotóxico |RF|
|I15|O técnico deve  editar as informações necessárias da plantação e do agrotóxico |RF|
|I16|O usuário pode editar suas informações pessoais|RF|
|I17|O usuário deve ter acesso a informações pertinentes ao uso do app (<a href="../../modelagem/lexicos#plantio_finalizado">plantações concluídas</a>, <a href="../../modelagem/lexicos#aplicacao_agrotoxico">agrotóxicos utilizados</a>)|RF|
|I18|O aplicativo deve ser seguro para garantir o <a href="../../modelagem/lexicos#cardeneta_de_campo">rastreamento das plantações</a>|RNF| 
|I19|O aplicativo deve ser intuitivo|RNF|
|I20|O aplicativo deve ser acessível|RNF|
<h6 align = "center">Tabela 1: Tabela contendo os requisitos levantados pela introspecção</h6>
<h6 align = "center">Fonte: Autor</h6>


<center>

|Legenda|Descrição|
|:--:|:--:|
|I|Introspecção|
|RF|Requisito Funcional|
|RNF|Requisito Não Funcional|
<h6>Tabela 2: Legenda dos acrônimos contidos na Tabela 1</h6>
<h6>Fonte: Autor</h6>

</center>


## 5. Bibliografia
> SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 07. 1º/2019. 50 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.