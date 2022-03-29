# Documento de Arquitetura de Software

## 1. Versionamento

| Versão | Data       | Descrição                                               | Autor(es)                 |
| ------ | ---------- | ----------------------------------------------------    | ------------------------- |
| 1.0    | 22/03/2022 | Abertura do documento                                   | Vitor Lamego e João Moura |
| 1.1    | 22/03/2022 | Adição da Visão Lógica                                  | Vitor Lamego              |
| 1.2    | 22/03/2022 | Adição do tópico de Qualidade                           | João Moura                |
| 1.3    | 23/03/2022 | Adição do tópico de Metas e Restrições Arquiteturais    | Brenno                    |
| 1.4    | 25/03/2022 | Adição do tópico de Visão de Implementação              | Eduardo Afonso            |
| 1.5    | 25/03/2022 | Adição do tópico de Visão de Implantação                | Rafael Ramos              |
| 1.6    | 26/03/2022 | Adição do tópico de Visão de Dados                      | Thiago                    |
| 1.7    | 26/03/2022 | Adição do tópico de Introdução e Tamanho e Performance  | Carlos                    |
| 1.7    | 26/03/2022 | Adição do tópico de Representação Arquitetural  | Paulo                    |
| 1.8    | 27/03/2022 | Adição do tópico de Visão de Casos de Uso  | Denniel William                    |
| 1.9    | 29/03/2022 | Adição do tópico de Visão de processos  | Victor Lima                   |
## 2. Introdução 
### 2.1 Objetivo
<p style="text-align: justify; text-indent: 20px"> Este documento fornece uma visão abrangente da arquitetura do sistema, usando diferentes visões arquiteturais para descrever diferentes aspectos do sistema. Destina-se a capturar e transmitir os fragmentos e decisões arquiteturais significativas que foram feitas no projeto Caderneta de Campo Digital. </p>

### 2.2 Escopo
<p style="text-align: justify; text-indent: 20px">Partindo do conjunto de visões definidas pelo RUP[1] além da visão de dados, este documento permite expor as principais decisões arquiteturais tomadas na construção e implementação do sistema.</p>
<p style="text-align: justify; text-indent: 20px">Por isso apresenta significativos casos de uso, elementos de design, estrutura dos processos do sistema, elementos persistentes e importantes do modelo de dados e as principais dimensões de qualidade do sistema.</p> 

### 2.3 Definições, Acrônimos e Abreviações
<p style="text-align: justify; text-indent: 20px">Termos, acrônimos e abreviações foram identificados e detalhados na tabela abaixo, junto de sua descrição.</p> 

| Termo | Descrição |
|:-----:|-----------|
| RUP | <i>Rational Unified Process</i> |
| iOS | Sistema operacional móvel da Apple Inc. |

### 2.4 Visão Geral
<p style="text-align: justify; text-indent: 20px">Seguindo o template criado para uso com o RUP, temos os seguintes tópicos:</p>

- <a href="#2-introducao">Introdução</a>: Promove uma visão geral do Documento de Arquitetura de Software.
- <a href="#3-representacao-arquitetural">Representação Arquitetural</a>: Descreve qual é a arquitetura de software para o sistema atual e como ela é representada.
- <a href="#4-metas-e-restricoes-arquiteturais">Metas e Restrições Arquiteturais</a>: Esta seção descreve os requisitos e objetivos de software que têm algum impacto significativo na arquitetura.
- <a href="#5-visao-de-casos-de-uso">Visão de Casos de Uso</a>: Lista os casos de uso ou cenários que representam alguma funcionalidade central significativa no sistema final.
- <a href="#6-visao-logica">Visão Lógica</a>: Descreve as partes arquitetonicamente significativas do modelo de design.
- <a href="#7-visao-de-processos">Visão de Processos</a>: Descreve os principais modos de comunicação entre processos.
- <a href="#8-visao-de-implantacao">Visão de Implantação</a>: Descreve as configurações do sistema para disponibilização de uso.
- <a href="#9-visao-da-implementacao">Visão da Implementação</a>: Descreve a decomposição do software em camadas e subsistemas no modelo de implementação.
- <a href="#10-visao-de-dados">Visão de Dados</a>: Descreve a perspectiva de armazenamento de dados persistente do sistema.
- <a href="#11-tamanho-e-performance">Tamanho e Performance</a>: Descreve as características de dimensionamento do software que impactam a arquitetura.
- <a href="#12-qualidade">Qualidade</a>: Descreve como a arquitetura contribui para os quesitos de: extensibilidade, confiabilidade, portabilidade e etc. 
- <a href="#13-referencias">Referências</a>: Lista todas os documentos que foram usados como referência.


## 3. Representação Arquitetural

### 3.1 Frontend

<center>
<img src="../../../assets/arquitetura_reutilizacao/flutter.png" class="zoom"/>
<h6>Figura 1: Imagem Flutter</h6>
<h6>Fonte: Flutter.</h6>
</center>

<p style="text-align: justify; text-indent: 20px"> Flutter é um framework open source, desenvolvido pelo google para aplicações multiplataformas: mobile, desktop e web; permitindo a criação de aplicações nativas a partir de um único código base. A linguagem base do Flutter é o Dart, uma linguagem também criada pelo Google que se assemelha bastante ao JavaScript. </p>

<p style="text-align: justify; text-indent: 20px"> A equipe optou pela escolha do flutter por diversos motivos, o principal deles foi que grande parte dos membros ja tiveram um contato prévio com a tecnologia, além do que, as 3 principais características em que o flutter é baseado (produtivo, rápido e flexivel) já são motivos suficientes para considerar como um forte candidato. Bom salientar que diversas empresas têm investido na ferramenta, desta forma, provocando um grande crescimento no mercado.</p>

### 3.2 Backend

<center>
<img src="../../../assets/arquitetura_reutilizacao/django.png" class="zoom"/>
<h6>Figura 2: Imagem Django</h6>
<h6>Fonte: Django.</h6>
</center>

<p style="text-align: justify; text-indent: 20px"> Django REST Framework ou DRF é um kit de ferramentas poderoso e flexível para construir APIs da Web. Permite a construção de APIs em qualquer plataforma, seja Windows, macOS ou Linux. É um framework muito utilizado por toda a comunidade, pois provê uma forma simples e rápida para a construção de APIs utilizando as facilidades que o Django oferece, como o sistema de rotas e seu ORM para manipulação de banco de dados.</p>

<p style="text-align: justify; text-indent: 20px"> A escolha dessa tecnologia também foi com base na experiência prévia de alguns integrantes da equipe, que estavam dispostos a realizar treinamentos e fornecer ajuda aos demais membros. Sem falar das vantagens que a ferramenta traz, como possibilitar um rápido desenvolvimento e possuir uma excelente documentação.</p>

### 3.3 Banco de dados

<center>
<img src="../../../assets/arquitetura_reutilizacao/postgresql.jpg" class="zoom"/>
<h6>Figura 2: Imagem PostgreSql</h6>
<h6>Fonte: PostgreSql.</h6>
</center>

<p style="text-align: justify; text-indent: 20px"> O PostgreSQL é uma ferramenta open source que atua como sistema de gerenciamento de bancos de dados relacionados. Seu foco é permitir implementação da linguagem SQL em estruturas, garantindo um trabalho com os padrões desse tipo de ordenação dos dados. Será utilizado para armazenar os dados provenientes da API, sendo um dos bancos de dados mais populares da atualidade. </p>

## 4. Metas e Restrições Arquiteturais
### 4.1 Metas
- O aplicativo deve ser de fácil utilização
- O aplicativo deve garantir a rastreabilidade dos plantios
- O aplicativo deve desempenhar suas funções de forma eficiente

### 4.2 Restrições
- O sistema deve permitir o uso apenas de pessoas já cadastradas pelo Instituto de Assistência Técnica e Extensão Rural(EMATER)
- A aplicação deverá ser disponibilizada por meio um aplicativo
- É necessário possuir um smartphone para acessar a aplicação
- É preciso ter uma conexão com a internet para utilizar a aplicação
- Deve ser desenvolvida em Python(Django) e Dart(Flutter)

## 5. Visão de Casos de Uso

<p style="text-align: justify; text-indent: 20px">Seguindo um nível maior de abstração em comparação a outros tópicos tratados no documento, a visão de casos de uso visa auxiliar no entendimento das interações dos atores com o sistema de forma a descrever os cenários de uso da aplicação. Este tópico irá tratar dos casos de uso mais significativos levantados no <a href="../../modelagem/extras/caso_de_uso">documento de caso de uso</a> dando uma breve descrição sobre cada caso.</p> 

### 5.1 Descrição dos casos de uso

- **UC02 - Cadastrar**: Este caso de uso é o ponto inicial do projeto sendo que nessa etapa o <a href="../../requisitos/modelagem/lexicos#usuario">usuário</a> irá optar pelo registro como <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a> ou <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> dentro da aplicação, ficando assim restrito as funcionalidades de cada tipo de <a href="../../requisitos/modelagem/lexicos#usuario">usuário</a>.

- **UC04 - Visualizar propriedade**: Este caso de uso se refere ao <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> visualizar a <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a> no qual faz a supervisão, e também ao <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  visualizar apenas sua própria <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>.

- **UC05 - Gerar caderneta de campo**: Este caso de uso se trata do foco do projeto e é exclusiva do <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a> , sendo ele capaz de gerar uma <a href="../../requisitos/modelagem/lexicos#caderneta_de_campo">caderneta de campo</a> com as informações sobre a <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>, como <a href="../../requisitos/modelagem/lexicos#plantio">plantio</a> e <a href="../../requisitos/modelagem/lexicos#talhao">talhões</a> a fim de gerar uma <a href="../../requisitos/modelagem/lexicos#rastreabilidade">rastreabilidade</a>.

- **UC14 - Visualizar plantações colhidas**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  e consiste em visualizar as <a href="../../requisitos/modelagem/lexicos#plantio">plantações</a> colhidas em uma <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a> com o objetivo de ter controle sobre as <a href="../../requisitos/modelagem/lexicos#plantio">plantações</a> feitas em cada <a href="../../requisitos/modelagem/lexicos#talhao">talhão</a> dentro dessa <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>.

- **UC17 - Registrar aplicação de agrotóxico**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a> e consiste no <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a> registrar uma <a href="../../requisitos/modelagem/lexicos#aplicacao_agrotoxico"><a href="../../requisitos/modelagem/lexicos#aplicacao_agrotoxico">aplicação de agrotóxico</a></a> em cima de uma <a href="../../requisitos/modelagem/lexicos#plantio">plantação</a>, com o objetivo de registrar quando foi feita essa aplicação. 

- **UC19 - Marcar uma plantação como colhida**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  e consiste no <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  marcar que uma <a href="../../requisitos/modelagem/lexicos#plantio">plantação</a> foi colhida em um <a href="../../requisitos/modelagem/lexicos#talhao">talhão</a>. Nesse caso essa marcação servirá para atualizar o histórico sobre um <a href="../../requisitos/modelagem/lexicos#talhao">talhão</a> de <a href="../../requisitos/modelagem/lexicos#plantio">plantações</a> feitas sobre ele.

- **UC21 - visualizar caderneta de campo**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste no <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> visualizar a <a href="../../requisitos/modelagem/lexicos#caderneta_de_campo">caderneta de campo</a> gerada pelo <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  sobre a <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a> supervisionada. Seu objetivo é conectar a interação do <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  e <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> sobre a <a href="../../requisitos/modelagem/lexicos#caderneta_de_campo">caderneta de campo</a> digital, assim que ela for gerada, será disponibilizada para o <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a>. 

- **UC22 - Solicitar alteração na caderneta de campo**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste no <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> conseguir reportar divergências na <a href="../../requisitos/modelagem/lexicos#caderneta_de_campo">caderneta de campo</a>, seu objetivo é manter o padrão atualmente orientado pelos <a href="../../requisitos/modelagem/lexicos#tecnico">técnicos</a> de forma a manter a documentação da <a href="../../requisitos/modelagem/lexicos#caderneta_de_campo">caderneta de campo</a> regularizada.

- **UC23 - Desassociar uma propriedade**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste no <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> se desassociar da <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>, sendo assim, o <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> não será mais o supervisor dessa <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>. Este caso auxilia na rotatividade de <a href="../../requisitos/modelagem/lexicos#tecnico">técnicos</a> com a <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>.

- **UC24 - Se associar a uma propriedade**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste no <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> se associar a uma <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>, sendo assim, o <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> será o supervisor <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a> associade. Este caso e o caso no tópico anterior se complementam colaborando para a rotatividade de <a href="../../requisitos/modelagem/lexicos#tecnico">técnicos</a> de uma <a href="../../requisitos/modelagem/lexicos#propriedade">propriedade</a>.

- **UC25 - Informar o período de carência**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste em informar o <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a>  sobre o <a href="../../requisitos/modelagem/lexicos#periodo_carencia">período de carência</a> sobre o <a href="../../requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> utilizado na <a href="../../requisitos/modelagem/lexicos#plantio">plantação</a>, ele tem como objetivo a comunicação e regularização das regras sanitárias sobre uma <a href="../../requisitos/modelagem/lexicos#plantio">plantação</a>.

- **UC26 - Cadastrar agrotóxico**: Este caso de uso é exclusivo do <a href="../../requisitos/modelagem/lexicos#tecnico">técnico</a> e consiste em cadastrar um <a href="../../requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> no sistema visando auxiliar ao <a href="../../requisitos/modelagem/lexicos#produtor">produtor</a> quando for registrada uma <a href="../../requisitos/modelagem/lexicos#aplicacao_agrotoxico">aplicação de agrotóxico</a> sobre uma <a href="../../requisitos/modelagem/lexicos#plantio">plantação</a> através de informações pré-definidas e com ilustrações do <a href="../../requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a>. 



## 6. Visão Lógica
### 6.1 Visão Geral
<p style="text-align: justify; text-indent: 20px">As visões de uma determinada arquitetura são abstrações dos modelos já criados para o projeto. Na ocasião da visão lógica o objetivo é decompor os subsistemas e seus respectivos pacotes, apresentando as suas principais características, a fim de melhorar a qualidade de qualquer documento de modelagem já elaborado. O objetivo não é entrar em muitos detalhes por ser responsabilidade da própria modelagem.</p> 

<p style="text-align: justify; text-indent: 20px">Sendo assim, para a discussão da visão lógica serão utilizadas algumas imagens referentes à modelagem de pacotes elaborada pelo grupo. Além disso, as visões serão separadas para o Back-end e para o Mobile, uma vez que possuem estruturas diferentes</p>

### 6.2 Diagrama de Pacotes Mobile

<img src="../../../assets/modelagem/estatica/mobile.png" class="zoom"/>
<h6 align = "center">Figura 1: Diagrama de pacotes mobile</h6>
<h6 align = "center">Fonte: Autor</h6>

<p style="text-align: justify; text-indent: 20px">A parte do Mobile é responsável pelo contato direto com o usuário do aplicativo, onde a partir das interfaces o usuário consegue se comunicar com o sistema desenvolvido. Entrando na explicação a nível lógico dos pacotes do mobile, podemos perceber que existe uma pasta do projeto, que na ocasião está nomeada como <b>Flutter</b>. A partir disso, existe um primeiro nível de profundidade que possui os seguintes pacotes: <b>Android</b>, <b>iOS</b>, <b>assets</b> e <b>lib</b>. Os pacotes: <b>Android</b> e <b>iOS</b> são responsáveis por armazenar configurações e detalhes específicos de cada sistema operacional, onde as informações de build e qualquer necessidade de utilização de recursos nativos são tratados. O pacote <b>assets</b> é responsável por armazenar os recursos externos do projeto, que pela imagem podemos perceber que esses recursos são imagens e fontes para o projeto, sendo armazenados em seus respectivos pacotes. Por fim temos o pacote <b>lib</b> que é responsável por armazenar todo o código fonte desenvolvido para o projeto.</p>

<p style="text-align: justify; text-indent: 20px">No pacote <b>lib</b> existem vários outros pacotes que se relacionam e que serão explicados a seguir: como pacote central temos a pasta <b>pages</b> que é responsável por armazenar as interfaces do aplicativo, além disso essa pasta se relaciona com várias outras, a partir dela o pacote <b>components</b> é importado, já que é responsável por armazenar componentes globais, ou até mesmo locais, do projeto. Portanto, as pages acabam utilizando esses components que são criados ao longo do projeto. Além disso, se relaciona com o pacote de <b>controllers</b> que ficam responsáveis pela estruturação e manipulação de dados que vêm do servidor e que são obtidos diretamente do pacote de <b>services</b>, que é responsável por fazer efetivamente as requisições e aguardar as respostas obtidas. Por sua vez, o pacote de services e de controller acabam utilizando o pacote de <b>models</b> para que os dados vindos do servidor sejam transformados no modelo que a aplicação mobile necessita. Por fim, existe o pacote <b>globals</b> que acaba sendo utilizado por todos os outros pacotes e que é responsável por armazenar informações, variáveis, objetos que precisam ser acessados globalmente de qualquer parte do projeto.</p> 

### 6.3 Diagrama de Pacotes Backend

<img src="../../../assets/modelagem/estatica/backend.png" class="zoom"/>
<h6 align = "center">Figura 2: Diagrama de pacotes backend</h6>
<h6 align = "center">Fonte: Autor</h6>

<p style="text-align: justify; text-indent: 20px">Para a arquitetura do Back-End, temos um pacote <b>Settings</b> que é responsável pelas configurações locais de ambiente e configurações globais do projeto. Além disso, existe uma relação com a base de dados do projeto que na ocasião o banco utilizado foi o PostgreSQL, por fim, nesse primeiro nível, existe um pacote para cada módulo desenvolvido, que na imagem está descrito como <b>Modulo N</b>. A seguir será detalhado como funciona a estrutura de pacotes de cada módulo, que acaba concentrando as principais funcionalidades do back.</p>

<p style="text-align: justify; text-indent: 20px">Pode-se perceber que o pacote centralizado nessa estrutura acaba sendo o pacote <b>view</b> que fica responsável justamente pelas views dos módulos que utilizam o pacote de <b>urls</b>, responsável por detalhar os endpoints daquele determinado módulo, para realizar a comunicação com o Mobile. O pacote de views também acessa o pacote de <b>models</b> para que as informações do banco sejam organizadas de forma que o servidor desenvolvido consiga utilizar, criando então os modelos para esses dados recebidos. Quando existe qualquer mudança em algum modelo dos dados do banco, o pacote <b>migrations</b> fica responsável por implementar essas alterações. Além disso, qualquer manipulação dos dados de algum modelo do projeto é feita dentro do pacote de <b>managers</b>, portanto acaba sendo utilizado pelo pacote de models. Voltando para a centralização do pacote views, ele também acessa o pacote de <b>serializers</b> que possui como finalidade a serialização e deserialização dos objetos JSON que são enviados entre o back e o Mobile. O último relacionamento é com o pacote <b>filters</b> que armazena filtros de querysets utilizados.</p>

<p style="text-align: justify; text-indent: 20px">Por fim, existem três pacotes que não possuem relação direta com o pacote de view, mas que são fundamentais para o bom funcionamento do servidor, sendo eles: pacote <b>tests</b> que possui os testes do módulo em específico, o pacote <b>tasks</b> que são tarefas que executadas de forma assíncrona a partir de um Observer ( Padrão GoF Comportamental ) e por último o pacote <b>admin</b> que são arquivos que armazenam configurações das páginas referentes ao objeto na página do administrador.</p>

## 7. Visão de Processos
### 7.1 Visão Geral
<p align="justify" style="text-indent: 20px">A visão de processos tem como objetivo fornecer uma base para compreensão da organização dos processos dentro do sistema desenvolvido e a vizualização de como esses grupos de processos interagem. De forma intuitiva fica claro por quais processos o sistema deverá passar para que uma atividade seja realizada.</p>

<p align="justify" style="text-indent: 20px">Durante a etapa de modelagem dinâmica foram criados os <a href="../../modelagem/dinamica/diagrama_de_sequencia"> diagramas de sequência</a> que são utilizados para ilustrar os processos existentes no nosso projeto</p>

### 7.2 Cadastro de usuário

<img src="../../../assets/modelagem/diagramaSequencia1.svg" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de cadastro de usuário</h6>
<h6 align = "center">Fonte: Autores</h6>

### 7.3 Adicionar plantação

<img src="../../../assets/modelagem/diagramaSequencia2.svg" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de adição de plantação</h6>
<h6 align = "center">Fonte: Autores</h6>

### 7.4 Aplicar agrotóxico

<img src="../../../assets/modelagem/diagramaSequencia3.svg" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de aplicação de agrotóxico</h6>
<h6 align = "center">Fonte: Autores</h6>

### 7.5 Atribuir técnico à propriedade

<img src="../../../assets/modelagem/diagramaSequencia4.svg" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de atribuição de técnico à propriedade</h6>
<h6 align = "center">Fonte: Autores</h6>

## 8. Visão de Implantação

### 8.1 Visão Geral
<p align="justify" style="text-indent: 20px">A visão de implantação objetiva a representação física tanto a nível dos processos e/ou dos componentes, é estabelecida uma configuração física do sistema a partir dos nós representados nos diagramas. O diagrama abaixo busca essa representação física da implantação de uma maneira um pouco generalista, porém com os processos e componentes necessários para tal implantação.</p>

### 8.2 Diagrama de Implantação
<img src="../../../assets/das/diagrama_de_implantacao.png" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de implantação</h6>
<h6 align = "center">Fonte: Autor</h6>

## 9. Visão da Implementação
### 9.1 Visão Geral
<p align="justify" style="text-indent: 20px">Esta visão tem como objetivo apresentar as decisões arquiteturais feitas pela equipe para realizar a implementação do produto, tais como os sistemas e subsistemas da implementação com suas dependências.</p>

<p align="justify" style="text-indent: 20px">A equipe ao longo do projeto confeccionou o <a href="../../modelagem/estatica/diagrama_de_componentes">diagrama de componentes</a> que retrata o esse escopo de sistemas e subsistemas, além disso, diagramas que também foram confeccionados e trazem uma ideia melhor das camadas das implementações tanto do back-end como do front-end são os <a href="../../modelagem/estatica/diagrama_de_pacotes">diagramas de pacotes</a>.</p>

### 9.2 Diagrama de Componentes
<img src="../../../assets/modelagem/diagramaComponentes.svg" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de pacotes componentes</h6>
<h6 align = "center">Fonte: Autor</h6>

### 9.3 Diagrama de Pacotes Backend
<img src="../../../assets/modelagem/estatica/backend.png" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de pacotes backend</h6>
<h6 align = "center">Fonte: Autor</h6>

### 9.4 Diagrama de Pacotes Frontend
<img src="../../../assets/modelagem/estatica/mobile.png" class="zoom"/>
<h6 align = "center">Figura X: Diagrama de pacotes frontend</h6>
<h6 align = "center">Fonte: Autor</h6>

## 10. Visão de Dados
### 10.1 Visão Geral

<p align="justify" style="text-indent: 20px">A Visão de Dados trata dos dados que são salvos e que podem ser recuperados quando necessário no futuro, ou seja, daqueles dados que são precisam ser persistidos pela aplicação em um Bancos de Dados Relacional. Vale ressaltar que essa parte é muito importante, uma vez que a sua modelagem impacta diretamente na implementação do projeto.</p>   
<p align="justify" style="text-indent: 20px">A modelagem de dados na Caderneta de Campo Digital teve como objetivo garantir que as entidades e seus relacionamentos conseguissem atender todas as necessidades especificadas no <a href="../../modelagem/agil/product_backlog">Product Backlog</a>, garantindo a proteção dos dados, a alta coesão e tornar o bancos de dados mais flexível, eliminando a redundância e dependência inconsistente.</p>
<p align="justify" style="text-indent: 20px">Dessa forma, a equipe começou a modelagem de uma forma mais abstrata pelo <a href="../../modelagem/extras/mer">Modelo Entidade-Relacionamento (MER)</a> que permitiu, de forma simples e eficiente, a identificação e modelagem das entidades, dos atributos e de seus relacionamentos. Posteriormente, as entidades, os atributos e seus relacionamentos foram representados em forma gráfica no <a href="../../modelagem/extras/der">Diagrama Entidade-Relacionamento (DER)</a>, como mostra a Figura X.</p>

<img src="../../../assets/modelagem/extras/derV2.png" class="zoom"/>
<h6 align = "center">Figura X: Diagrama Entidade-Relacionamento</h6>
<h6 align = "center">Fonte: Autores</h6>

<p align="justify" style="text-indent: 20px">Por conseguinte, no <a href="../../modelagem/extras/dld">Diagrama Lógico de Dados (DLD)</a>, a modelagem se aproximou da representação física em um banco de dados, onde o tipo dos atributos foi definido e os relacionamentos convertidos em tabelas ou campos de chave estrangeira. Por fim, todas as entidades, seus atributos e seus relacionamentos foram documentados no <a href="../../modelagem/extras/dicionario_dados">Dicionário de Dados</a>.</p>


## 11. Tamanho e _Performance_
<p style="text-align: justify; text-indent: 20px">Tendo em vista o tamanho descrito nos repositórios de backend e frontend, o sistema como um todo conta com menos de 1 gigabyte de tamanho.</p>
<p style="text-align: justify; text-indent: 20px">Para a execução da aplicação, se tratando de aplicativo móvel, é necessário um <i>smartphone</i> com sistema operacional Android ou iOS com acesso à internet. Por ter como o objetivo a conexão de vários agricultores e técnicos é possível seu uso simultâneo com várias pessoas.</p>

## 12. Qualidade
<p align="justify" style="text-indent: 20px">Por fim, o último tópico que será abordado nesse documento de Arquitetura de Software, é sobre os quesitos de qualidade da aplicação. Para tanto, serão utilizadas as visões tanto do usuário final como dos programadores sobre o produto desenvolvido, avaliando alguns pontos essenciais destacados pelo modelo de qualidade proposto por McCall's []. Esse modelo, define diversos fatores de qualidades e seus critérios de qualidades, que serão utilizados para classificar e demonstrar os principais pontos de qualidade da Caderneta de Campo Digital.</p>
<p align="justify" style="text-indent: 20px">Além disso, é importante ressaltar que para atingir os objetivos de qualidade de código, foram seguidos diversos padrões definidos ao longo dos tópicos de Padrões de Projeto. Vários critérios de qualidade, como: consistência, tolerância a erros, eficiência de execução e de armazenamento, modularidade, entre outros, foram capazes de serem alcançados graças à utilização dos diversos <a href="../../padroes_projetos/estudos/grasp/">GRASP(s)</a>, sendo eles: o <a href="../../padroes_projetos/estudos/grasp/#41-polimorfismo">Polimorfismo</a>, a <a href="../../padroes_projetos/estudos/grasp/#44-coesao">Coesão</a> e o <a href="../../padroes_projetos/estudos/grasp/#45-acoplamento">Acoplamento</a> e os <a href="../../padroes_projetos/estudos/grasp/#46-controlador">Controladores</a>.</p>

<center>

| Fatores de Qualidade | Aplicação no Programa                                                                                                                                                                                                                                                                                                                                                                                                                  |
| :------------------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|      Eficiência      | A API e o Frontend, para alcançarem essa meta, utilizaram os padrões GoF's de <a href="../../padroes_projetos/aplicacao/gofs_criacionais/#41-factory-method">Método de Fábrica</a>, <a href="../../padroes_projetos/aplicacao/gofs_comportamentais/#41-state">State</a>, <a href="../../padroes_projetos/aplicacao/gofs_estruturais/#42-decorator">Decorator</a> e outros identificados nos documentos de aplicação.                   |
|     Usabilidade      | Como forma de alcançar a usabilidade, a equipe desenvolveu uma arquitetura simples e eficiente com a <a href="../../base/prototipacao/alta_fidelidade/">prototipação</a>, de forma a definir um modelo usável para o usuário, conforme métricas definidas no documento de <a href="../../modelagem/agil/especificacao_suplementar/">Especificação Suplementar</a> e na <a href="../../modelagem/agil/nfr_framework/">Modelagem NFR</a> |
|    Confiabilidade    | Para atingir a confiabilidade, também descrita na <a href="../../modelagem/agil/especificacao_suplementar/">Especificação Suplementar</a>, foi necessário a <a href="../../modelagem/extras/dld/">modelagem de um banco de dados</a> que atendesse as necessidades expostas por esse fator de qualidade. Com isso, tanto o backend quanto o frontend conseguem cumprir com as metas de confiabilidade esperadas para a aplicação.           |
|    Testabilidade     | A testabilidade também foi um princípio definido e utilizado desde o início das implementações do backend e do frontend. Isso, principalmente na visão do backend, se deve ao formato escolhido para o desenvolvimento da aplicação, o <i>Test Driven Development</i> (TDD) [].                                                                                                                                                        |
|   Manutenabilidade   | Em relação a meta de manutenabilidade, a equipe buscou criar uma arquitetura que utiliza de <i>frameworks</i> conhecidos e com grande suporte da comunidade. Dessa forma, esse fator de qualidade é facilmente atingido permitindo a equipe manter o software por muito tempo. Além disso, é importante ressaltar que essa meta facilitou as pesquisas sobre os padrões de projeto que podem ser utilizados no projeto.                |
|    Portabilidade     | Por fim, a meta de portabilidade foi destacada principalmente pelas vantagens provindas dos Padrões de Projetos utilizados, que auxiliam diretamente essa meta. Outro ponto muito importante, é que a API foi desenvolvida para poder ser utilizada independente do Frontend feito para o projeto.                                                                                                                                     |

</center>

## 13. Referências
<!-- > [] ****. -->

> [1] SERRANO, Milene. Arquitetura e Desenho de Software. **AULA - ARQUITETURA & DAS – PARTE II**. Acesso em: 26 mar. 2022.
<!-- usado no topico de qualidade (não explicitamente) -->
> [] **Diretriz: Documento de Arquitetura de Software**. Disponível em: <a href="https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/software_architecture_document_F4C93435.html">https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/software_architecture_document_F4C93435.html</a>.Acesso em: 22 de mar. de 2022.

<!-- topico de qualidade -->
> [] SINGH, **Jagannath - User's Perspective of Software Quality**. 2018.

<!-- topico de qualidade -->
> [] DevMedia, **Test Driven Development: TDD Simples e Prático**. Disponível em: <a href="https://www.devmedia.com.br/test-driven-development-tdd-simples-e-pratico/18533">https://www.devmedia.com.br/test-driven-development-tdd-simples-e-pratico/18533</a>. Acesso em: 22 de mar. de 2022.

<!-- Representação Arquitetural -->
> [] Treina Web **O que é Flutter?**. Disponivel em <a href= "https://www.treinaweb.com.br/blog/o-que-e-flutter">https://www.treinaweb.com.br/blog/o-que-e-flutter </a>  Acesso em 25 de mar. de 2022

> [] Flutter **Documentação Flutter**. Disponivel em <a href= "https://flutter.dev/">https://flutter.dev/</a>  Acesso em 25 de mar. de 2022

> [] Django Rest Framework **Documentação Django Rest Framework**. Disponivel em <a href= "https://www.django-rest-framework.org/">https://www.django-rest-framework.org/</a>  Acesso em 25 de mar. de 2022

> [] Rock Content **PostgreSQL: saiba o que é, para que serve e como instalar**. Disponivel em <a href= "https://rockcontent.com/br/blog/postgresql/#5">https://rockcontent.com/br/blog/postgresql/#5</a>  Acesso em 26 de mar. de 2022
