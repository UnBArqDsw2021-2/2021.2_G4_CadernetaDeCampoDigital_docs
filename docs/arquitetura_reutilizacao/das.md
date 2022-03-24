# Documento de Arquitetura de Software

## 1. Versionamento

| Versão | Data       | Descrição                                            | Autor(es)                    |
| ------ | ---------- | ---------------------------------------------------- | ---------------------------- |
| 1.0    | 22/03/2022 | Abertura do documento                                | Vitor Lamego e João Moura    |
| 1.1    | 22/03/2022 | Adição da Visão Lógica                               | Vitor Lamego                 |
| 1.2    | 22/03/2022 | Adição do tópico de Qualidade                        | João Moura                   |
| 1.3    | 23/03/2022 | Adição do tópico de Metas e Restrições Arquiteturais | Brenno                       |

## 2. Introdução 
### 2.1 Proposta
### 2.2 Escopo
### 2.3 Definições, Acrônimos e Abreviações
### 2.4 Visão Geral

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

### 3.3 Banco de dados

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

## 6. Visão Lógica
### 6.1 Visão Geral
<p style="text-align: justify; text-indent: 20px">As visões de uma determinada arquitetura são abstrações dos modelos já criados para o projeto. Na ocasião da visão lógica o objetivo é decompor os subsistemas e seus respectivos pacotes, apresentando as suas principais características, a fim de melhorar a qualidade de qualquer documento de modelagem já elaborado. O objetivo não é entrar em muitos detalhes por ser responsabilidade da própria modelagem.</p> 

<p style="text-align: justify; text-indent: 20px">Sendo assim, para a discussão da visão lógica serão utilizadas algumas imagens referentes à modelagem de pacotes elaborada pelo grupo. Além disso, as visões serão separadas para o Back-end e para o Mobile, uma vez que possuem estruturas diferentes</p>

### 6.2 Diagrama de Pacotes Mobile

<img src="../../../assets/modelagem/estatica/mobile.png" class="zoom"/>
<h6 align = "center">Figura 1: Diagrama de pacotes mobile</h6>
<h6 align = "center">Fonte: Autor</h6>

<p style="text-align: justify; text-indent: 20px">A parte do Mobile é responsável pelo contato direto com o usuário do aplicativo, onde a partir das interfaces o usuário consegue se comunicar com o sistema desenvolvido. Entrando na explicação a nível lógico dos pacotes do mobile, podemos perceber que existe uma pasta do projeto, que na ocasião está nomeada como <b>Flutter</b>. A partir disso, existe um primeiro nível de profundidade que possui os seguintes pacotes: <b>Android</b>, <b>iOS</b>, <b>assets</b> e <b>lib</b>. Os pacotes: <b>Android</b> e <b>iOS</b> são responsáveis por armazenar configurações e detalhes específicos de cada sistema operacional, onde as informações de build e qualquer necessidade de utilização de recursos nativos são tratados. O pacote <b>assets</b> é responsável por armazenar os recursos externos do projeto, que pela imagem podemos perceber que esses recursos são imagens e fontes para o projeto, sendo armazenados em seus respectivos pacotes. Por fim temos o pacote <b>lib</b> que é responsável por armazenar todo o código fonte desenvolvido para o projeto.</p>

<p style="text-align: justify; text-indent: 20px">No pacote <b>lib</b> existem vários outros pacotes que se relacionam e que serão explicados a seguir: como pacote central temos a pasta <b>pages</b> que é responsável por armazenar as interfaces do aplicativo, além disso essa pasta se relaciona com várias outras, a partir dela o pacote <b>components</b> é importado, já que é responsável por armazenar componentes globais, ou até mesmo locais, do projeto. Portanto, as pages acabam utilizando esses components que são criados ao longo do projeto. Além disso, se relaciona com o pacote de <b>controllers</b> que ficam responsáveis pela estruturação e manipulação de dados que vêm do servidor e que são obtidos diretamente do pacote de <b>services</b>, que é responsável por fazer efetivamente as requisições e aguardar as respostas obtidas. Por sua vez, o pacote de services e de controller acabam utilizando o pacote de <b>models</b> para que os dados vindos do servidor sejam transformados no modelo que a aplicação mobile necessita. Por fim, existe o pacote <b>globals</b> que acaba sendo utilizada por todos os outros pacotes e que é responsável por armazenar informações, variáveis, objetos que precisam ser acessados globalmente de qualquer parte do projeto.</p> 

### 6.3 Diagrama de Pacotes Backend

<img src="../../../assets/modelagem/estatica/backend.png" class="zoom"/>
<h6 align = "center">Figura 2: Diagrama de pacotes backend</h6>
<h6 align = "center">Fonte: Autor</h6>

<p style="text-align: justify; text-indent: 20px">Para a arquitetura do Back-End, temos um pacote <b>Settings</b> que é responsável pelas configurações locais de ambiente e configurações globais do projeto. Além disso, existe uma relação com a base de dados do projeto que na ocasião o banco utilizado foi o PostgreSQL, por fim, nesse primeiro nível, existe um pacote para cada módulo desenvolvido, que na imagem está descrito como <b>Modulo N</b>. A seguir será detalhado como funciona a estrutura de pacotes de cada módulo, que acaba concentrando as principais funcionalidades do back.</p>

<p style="text-align: justify; text-indent: 20px">Pode-se perceber que o pacote centralizado nessa estrutura acaba sendo o pacote <b>view</b> que fica responsável justamente pelas views dos módulos que utilizam o pacote de <b>urls</b>, responsável por detalhar os endpoints daquele determinado módulo, para realizar a comunicação com o Mobile. O pacote de views também acessa o pacote de <b>models</b> para que as informações do banco sejam organizadas de forma que o servidor desenvolvido consiga utilizar, criando então os modelos para esses dados recebidos. Quando existe qualquer mudança em algum modelo dos dados do banco, o pacote <b>migrations</b> fica responsável por implementar essas alterações. Além disso, qualquer manipulação dos dados de algum modelo do projeto é feita dentro do pacote de <b>managers</b>, portanto acaba sendo utilizado pelo pacote de models. Voltando para a centralização do pacote views, ele também acessa o pacote de <b>serializers</b> que possui como finalidade a serialização e deserialização dos objetos JSON que são enviados entre o back e o Mobile. O último relacionamento é com o pacote <b>filters</b> que armazena filtros de querysets utilizados.</p>

<p style="text-align: justify; text-indent: 20px">Por fim, existem três pacotes que não possuem relação direta com o pacote de view, mas que são fundamentais para o bom funcionamento do servidor, sendo eles: pacote <b>tests</b> que possui os testes do módulo em específico, o pacote <b>tasks</b> que são tarefas que executadas de forma assíncrona a partir de um Observer ( Padrão GoF Comportamental ) e por último o pacote <b>admin</b> que são arquivos que armazenam configurações das páginas referentes ao objeto na página do administrador.</p>

## 7. Visão de Processos

## 8. Visão de _Deploy_

## 9. Visão da Implementação
### 9.1 Visão Geral
### 9.2 Camadas

## 10. Visão do Banco de Dados

## 11. Tamanho e _Performance_

## 12. Qualidade
<p align="justify" style="text-indent: 20px">Por fim, o último tópico que será abordado nesse documento de Arquitetura de Software, é sobre os quesitos de qualidade da aplicação. Para tanto, serão utilizadas as visões tanto do usuário final como dos programadores sobre o produto desenvolvido, avaliando alguns pontos essênciais destacados pelo modelo de qualidade proposto por McCall's []. Esse modelo, define diversos fatores de qualidades e seus critérios de qualidades, que serão utilizados para classificar e demonstrar os principais pontos de qualidade da Caderneta Digital de Campo.</p>
<p align="justify" style="text-indent: 20px">Além disso, é importante ressaltar que para atingir os objetivos de qualidade de código, foram seguidos diversos padrões definidos ao longo dos tópicos de Padrões de Projeto. Vários critérios de qualidade, como: consitência, tolerância a erros, eficiência de execução e de armazenamento, modularidade, entre outros, foram capazes de serem alcançados graças à utilização dos diversos <a href="../../padroes_projetos/estudos/grasp/">GRASP(s)</a>, sendo eles: o <a href="../../padroes_projetos/estudos/grasp/#41-polimorfismo">Polimorfismo</a>, a <a href="../../padroes_projetos/estudos/grasp/#44-coesao">Coesão</a> e o <a href="../../padroes_projetos/estudos/grasp/#45-acoplamento">Acoplamento</a> e os <a href="../../padroes_projetos/estudos/grasp/#46-controlador">Controladores</a>.</p>

<center>

|Fatores de Qualidade|Aplicação no Programa|
|:-:|--|
|Eficiência|A API e o Frontend, para alcançarem essa meta, utilizaram os padrões GoF's de <a href="../../padroes_projetos/aplicacao/gofs_criacionais/#41-factory-method">Método de Fábrica</a>, <a href="../../padroes_projetos/aplicacao/gofs_comportamentais/#41-state">State</a>, <a href="../../padroes_projetos/aplicacao/gofs_estruturais/#42-decorator">Decorator</a> e outros identificados nos documentos de aplicação.|
|Usabilidade|Como forma de alcançar a usabilidade, a equipe desenvolveu uma arquitetura simples e eficiente com a <a href="../../base/prototipacao/alta_fidelidade/">prototipação</a>, de forma a definir um modelo usável para o usuário, conforme métricas definidas no documento de <a href="../../modelagem/agil/especificacao_suplementar/">Especificação Suplementar</a> e na <a href="../../modelagem/agil/nfr_framework/">Modelagem NFR</a>|
|Confiabilidade|Para atingir a confiabilidade, também descrita na <a href="../../modelagem/agil/especificacao_suplementar/">Especificação Suplementar</a>, foi necessário a <a href="../../modelagem/extras/dld/">modelagem de um banco de dados</a> que atendesse as necessidades expostas por esse fator de qualidade. Com isso, tanto o backend e o frontend conseguem cumprir com as metas de confiabilidade esperadas para a aplicação.|
|Testabilidade|A testabilidade também foi um princípio definido e utilizado desde o início das implementações do backend e do frontend. Isso, principalmente na visão do backend, se deve ao formato escolhido para o desenvolvimento da aplicação, o <i>Test Driven Development</i> (TDD) [].|
|Manutenabilidade|Em relação a meta de manutenabilidade, a equipe buscou criar uma arquitetura que utiliza de <i>frameworks</i> conhecidos e com grande suporte da comunidade. Dessa forma, esse fator de qualidade é fácilmente atingido permitindo a equipe manter o software por muito tempo. Além disso, é importante ressaltar que essa meta facilitou as pesquisas sobre os padrões de projeto que podem ser utilizados no projeto.|
|Portabilidade|Por fim, a meta de portabilidade foi destacada principalmente pelas vantagens provindas dos Padrões de Projetos utilizados, que auxiliam diretamente essa meta. Outro ponto muito importante, é que a API foi desenvolvida para poder ser utilizada independente do Frontend feito para o projeto.|

</center>

## 13. Referências
<!-- > [] ****. -->
<!-- usado no topico de qualidade (não explicitamente) -->
> [] **Diretriz: Documento de Arquitetura de Software**. Disponível em: <a href="https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/software_architecture_document_F4C93435.html">https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/software_architecture_document_F4C93435.html</a>.Acesso em: 22 de mar. de 2022.

<!-- topico de qualidade -->
> [] SINGH, **Jagannath - User's Perspective of Software Quality**. 2018.

<!-- topico de qualidade -->
> [] DevMedia, **Test Driven Development: TDD Simples e Prático**. Disponível em: <a href="https://www.devmedia.com.br/test-driven-development-tdd-simples-e-pratico/18533">https://www.devmedia.com.br/test-driven-development-tdd-simples-e-pratico/18533</a>. Acesso em: 22 de mar. de 2022.
