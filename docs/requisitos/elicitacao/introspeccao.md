# Introspecção

## 1. Versionamento
Versão|Data|Descrição|Autor(es)
------|----|---------|--------
1.0   | 29/01/2022 | Criação do documento | Rafael
1.1   | 30/01/2022 | Adição da introspecção e da tabela com os requisitos levantados| Rafael

## 2. Introdução

<p style="text-align: justify; text-indent: 20px">A Introspecção é uma técnica mais voltada para o especialista de requisitos, ele deve abstrair as melhores informações a partir de uma análise de como e quais seriam os melhores requisitos para satisfazer os usuários e os stakeholders do sistema, normalmente é uma técnica muito rica e profunda, porém pode não ser adequada quando não é um especialista da área realizando, mesmo assim vamos realizá-la buscando extrair ao máximo suas vantagens. </p>

## 3. Desenvolvimento da Introspecção

<p style="text-align: justify; text-indent: 20px"> O intuito será descrever a perspectiva dos usuários que irão fazer o uso do aplicativo.</p>

### 3.1 Acesso inicial:

* Deve haver opção de login e cadastro para ambos os usuários (produtor e técnico).
* O usuário já cadastrado deve poder recuperar sua senha.
* Aplicativo deve ser limpo, intuitivo e acessível visto que o público alvo pode ter dificuldade com as tecnologias.
* O aplicativo deve ser seguro para garantir o rastreamento das plantações.

### 3.2.1 Tela principal (Produtor)

* Deve poder visualizar suas propriedades.
* Deve poder visualizar suas plantações, bem como o status de cada uma.
* Deve poder cadastrar uma plantação.
* Deve ter uma área para o histórico de suas plantações e aplicações.
* Deve ter uma área para visualizar o perfil do(s) técnico(s) responsável(is) pela(s) sua(s) propriedade(s).

### 3.2.2 Tela principal (Técnico)

* Deve poder visualizar as fotos dos agrotóxicos enviadas pelos produtores.
* Deve poder visualizar as propriedades que está supervisionando.
* Deve ter uma área para visualizar o perfil dos produtores que está sendo responsável.

### 3.3 Tela de plantação:
* Deve poder visualizar as informações de talhão, produto, datas, aplicações.
* O produtor deve ter acesso a uma área de uso simples para cadastrar o uso de agrotóxico.
* O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola dessa plantação.
* O técnico deve poder editar as informações necessárias (agrotóxico, datas).
* Deve poder adicionar data de colheita encerrando essa plantação.

### 3.4 Tela de agrotóxicos

* O produtor deve ter a opção de cadastrar apenas a foto do agrotóxico e a data da aplicação.
* O produtor pode programar o uso de um agrotóxico.
* O técnico deve pode editar todas as informações, exceto a foto cadastrada.
* A interface deve ter boa usabilidade para garantir uma boa rastreabilidade.

### 3.5 Tela de perfil
* O usuário deve poder editar suas informações pessoas.
* O usuário deve ter acesso a informações pertinentes ao uso do app (plantações concluídas, agrotóxicos utilizados)


## 4. Requisitos levantados
|ID|Descrição|Tipo de Requisito
|--|--|--|
|I01|Cadastro e login de usuário com opção de recuperar senha|RF|
|I02|O produtor deve visualizar suas propriedades|RF|
|I03|O produtor deve cadastrar uma plantação|RF|
|I04|O produtor pode visualizar o histórico de suas plantações e agrotóxicos|RF|
|I05|O produtor pode visualizar o perfil do técnico que está monitorando sua propriedade|RF|
|I06|O produtor pode visualizar o status de cada plantação|RF|
|I07|O produtor deve cadastrar o uso do agrotóxico com foto e data apenas|RF|
|I08|O técnico deve ter acesso a foto dos agrotóxicos enviadas pelos produtores|RF|
|I09|O técnico deve visualizar as propriedades supervisionadas por ele|RF|
|I10|O aplicativo deve ter uso simples|RNF|
|I11|O usuário deve visualizar as informações das plantações responsáveis|RF|
|I12|O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola plantado.|RF|
|I13|O produtor deve adcionar a data de colheita encerrando a plantação |RF|
|I14|O produtor pode programar o uso de um agrotóxico |RF|
|I15|O técnico deve  editar as informações necessárias da plantação e do agrotóxico |RF|
|I16|O usuário pode editar suas informações pessoais|RF|
|I17|O usuário deve ter acesso a informações pertinentes ao uso do app (plantações concluídas, agrotóxicos utilizados)|RF|
|I18|O aplicativo deve ser seguro para garantir o rastreamento das plantações|RNF| 
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