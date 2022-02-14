## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|:------:|:----:|:---------:|:---------:|
|1.1|13/02/2022|Abertura do Product Backlog|Denniel William|
|1.2|13/02/2022|Adição das Histórias de usuário|Denniel William|
|1.3|13/02/2022|Adição da Introdução, Metodologia e Épicos|Eduardo Afonso|
|1.4|13/02/2022|Adição do backlog completo e legenda|Brenno Oliveira|
|1.5|13/02/2022|Adição das Features|Paulo Vitor|
|1.6|14/02/2022|Ajustes e Revisões|Denniel|



## 2. Introdução

<p style="text-align: justify; text-indent: 20px">Product backlog é um importante artefato para a metodologia <a href="https://unbarqdsw2021-2.github.io/2021.2_G4_CadernetaDeCampoDigital_docs/base/metodologia/#31-scrum">Scrum</a>, com ele a equipe é capaz de listar o trabalho de maneira priorizada e escolher os itens que serão trabalhados na Sprint sem a necessidade da participação do proprietário do produto.</p>

<p style="text-align: justify; text-indent: 20px">Foi escolhido, a princípio, três níveis de abstração. Sendo eles: <a href="#4-epicos">Épicos</a>, <a href="#5-features">Features</a> e <a href="#6-historias-de-usuario">Histórias de Usuário</a>.

</p>

## 3. Metodologia

<p style="text-align: justify; text-indent: 20px">A metodologia escolhida para realizar a construção do product backlog foi o Product Backlog Building (PBB). Essa metodologia consiste em realizar a criação do product backlog com os integrantes da equipe trabalhando de forma colaborativa, expondo seus pontos de vista e opiniões, a fim de preencher um quadro chamado PBB Canva.</p>

<p style="text-align: justify; text-indent: 20px">O PBB Canva é uma ferramenta do PBB que cria um fluxo de fácil entendimento para que todos os membros consigam colaborar com seu preenchimento. O fluxo de preenchimento do PBB Canva é o seguinte:</p>

- Nome do Produto
- Problemas
- Expectativas
- Personas
- Features
- Product Backlog Itens (PBIs)

<p style="text-align: justify; text-indent: 20px">O resultado do processo de preenchimento do PBB Canva foi o seguinte:</p>

<center>![PBB Canva](https://user-images.githubusercontent.com/54921791/153761163-f3955b56-577d-4403-aa56-17fabf5f6b6e.jpg)</center>
<center>[Figura 1: Figura contendo PBB Canva desenvolvido pela equipe](https://user-images.githubusercontent.com/54921791/153761163-f3955b56-577d-4403-aa56-17fabf5f6b6e.jpg)
</center>

## 4. Épicos

<p style="text-align: justify; text-indent: 20px">Épico foi o maior nível de granularidade que a equipe definiu na construção do product backlog.</p>

<p style="text-align: justify; text-indent: 20px">Os épicos são uma visão de mais alto nível em relação ao que deve ser implementado. Eles geralmente levam várias sprints para serem concluídos e podem ser divididos em objetivos menores.</p>

<p style="text-align: justify; text-indent: 20px">O projeto foi analisado de uma perspectiva mais ampla com o objetivo de ter uma visão geral sobre o produto e foi possível enxergar os três épicos a seguir.</p>

<center>

|ID|Descrição|
|:------:|:----:|
|**EP1**|Cadastro e Autenticação|
|**EP2**|<a href="/requisitos/modelagem/lexicos#plantio">Plantação</a> e <a href="/requisitos/modelagem/lexicos#agrotoxico">Agrotóxico</a>|
|**EP3**|Detalhes e Histórico|

</center>
<h6 align="center">Tabela 1: Épicos</h6>
<h6 align="center">Fonte: Autores</h6>

## 5. Features

<p style="text-align: justify; text-indent: 20px"></p>

<p style="text-align: justify; text-indent: 20px"> Uma Feature descreve um conjunto de funcionalidades, caracteŕisticas e requisitos para o projeto, agrupam uma ou muitas User Stories e tem como objetivo realizar um Épico. </p>

<p style="text-align: justify; text-indent: 20px"></p>

<center>

| **Épico** | **ID** | **Descrição** |
| :-: | :-: | --- |
| **E1** | **FT01** | Controle de <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> |
| **E2** | **FT02** | Manter <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>|
| **E2** | **FT03** | Manter <a href="/requisitos/modelagem/lexicos#plantio">plantação</a>|
| **E2** | **FT04** | <a href="/requisitos/modelagem/lexicos#aplicar_agrotoxico" > Aplicar agrotóxico </a>|
| **E2** | **FT05** | Gerenciar <a href="/requisitos/modelagem/lexicos#agrotoxico" > agrotóxico </a>|
| **E3** | **FT06** | Gerenciar  <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo" > caderneta de campo </a> |
| **E3** | **FT07** | Manter histórico de <a href="/requisitos/modelagem/lexicos#plantio">plantações</a>|
| **E3** | **FT08** |<a href="/requisitos/modelagem/lexicos#supervisionar_propriedade">Supervisiona propriedade</a>||
| **E3** | **FT09** | Regularizar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo" > caderneta de campo </a>|
                        
</center>
<h6 align="center">Tabela 2: Features</h6>
<h6 align="center">Fonte: Autores</h6>

## 6. Histórias de Usuário

<p style="text-align: justify; text-indent: 20px">As histórias de usuário se trata de descrições curtas e simples de uma funcionalidade contadas da perspectiva de um usuário. Cada história de usuário se refere a implementação de pequena parte do comportamento do sistema.</p>

<p style="text-align: justify; text-indent: 20px">Da perspectiva do usuário, consegue se obter a qual usuário a tarefa se refere, o que será feito e porquê será feito.</p>

<p style="text-align: justify; text-indent: 20px">Seu formato é caracterizado por:</p>

> **"Eu, como [persona], eu [quero], [para que]"**

|Feature|ID|Descrição|
|:------:|:----:|:---------:|
| <a href="#FT01">**FT01**</a> | <span id="US01">**US01**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso me cadastrar na aplicação, para ter acesso as funcionalidades de técnico |
| <a href="#FT01">**FT01**</a> | <span id="US02">**US02**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#usuario">usuário</a>, posso apagar meus dados da aplicação, caso não queira mas usar a aplicação |
| <a href="#FT01">**FT01**</a> | <span id="US03">**US03**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#usuario">usuário</a>, posso editar meus dados de usuário, para desfazer algum possível erro ou atualizar os dados. |
| <a href="#FT01">**FT01**</a> | <span id="US04">**US04**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#usuario">usuário</a>, posso fazer login na aplicação, para ter acesso a minha conta. |
| <a href="#FT01">**FT01**</a> | <span id="US05">**US05**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#usuario">usuário</a>, posso fazer logout, caso não deseje mais estar logado ou mudar de conta. |
| <a href="#FT01">**FT01**</a> | <span id="US06">**US06**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso me cadastrar na aplicação, para poder ter acesso as funcionalidades de produtor |
| <a href="#FT02">**FT02**</a> | <span id="US07">**US07**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso cadastrar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US08">**US08**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso alterar a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US09">**US09**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso adicionar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US10">**US10**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso remover <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US11">**US11**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso atribuir <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US12">**US12**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso alterar <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT02">**FT02**</a> | <span id="US13">**US13**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso remover <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
| <a href="#FT03">**FT03**</a> | <span id="US14">**US14**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso adicionar <a href="/requisitos/modelagem/lexicos#plantio">plantação</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> |
| <a href="#FT03">**FT03**</a> | <span id="US15">**US15**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso alterar <a href="/requisitos/modelagem/lexicos#plantio">plantação</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> |
| <a href="#FT03">**FT03**</a> | <span id="US16">**US16**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso marcar <a href="/requisitos/modelagem/lexicos#colher_plantio">plantação como colhida</a> para ter controle sobre a <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> |
| <a href="#FT04">**FT04**</a> | <span id="US17">**US17**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso registrar <a href="/requisitos/modelagem/lexicos#aplicar_agrotoxico">aplicação de agrotóxico</a> para ter controle de <a href="/requisitos/modelagem/lexicos#aplicar_agrotoxico">aplicação de agrotóxico</a> |
| <a href="#FT04">**FT04**</a> | <span id="US18">**US18**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso enviar foto do <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> para o <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> para ter controle de <a href="/requisitos/modelagem/lexicos#aplicar_agrotoxico">aplicação de agrotóxico</a> |
| <a href="#FT05">**FT05**</a> | <span id="US19">**US19**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso identificar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> aplicado na <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> para gerenciar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> |
| <a href="#FT05">**FT05**</a> | <span id="US20">**US20**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso informar <a href="/requisitos/modelagem/lexicos#periodo_carencia">período de carência</a> para gerenciar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> |
| <a href="#FT05">**FT05**</a> | <span id="US21">**US21**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso cadastrar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> para gerenciar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> |
| <a href="#FT05">**FT05**</a> | <span id="US22">**US22**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso remover <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> para gerenciar <a href="/requisitos/modelagem/lexicos#agrotoxico">agrotóxico</a> |
| <a href="#FT06">**FT06**</a> | <span id="US23">**US23**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso gerar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> para gerenciar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
| <a href="#FT06">**FT06**</a> | <span id="US24">**US24**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso visualizar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> para gerenciar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
| <a href="#FT07">**FT07**</a> | <span id="US25">**US25**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso visualizar <a href="/requisitos/modelagem/lexicos#plantio_finalizado">plantações colhidas</a> na <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> para ter manter histórico de <a href="/requisitos/modelagem/lexicos#plantações">plantações</a> |
| <a href="#FT07">**FT07**</a> | <span id="US26">**US26**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, posso visualizar <a href="/requisitos/modelagem/lexicos#plantio_finalizado">plantações colhidas</a> em um <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> para ter manter histórico de <a href="/requisitos/modelagem/lexicos#plantações">plantações</a> |
| <a href="#FT08">**FT08**</a> | <span id="US27">**US27**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso visualizar uma <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> para <a href="/requisitos/modelagem/lexicos#supervisionar_propriedade">supervisionar propriedade</a> |
| <a href="#FT09">**FT09**</a> | <span id="US28">**US28**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso visualizar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> para regularizar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
| <a href="#FT09">**FT09**</a> | <span id="US29">**US29**</span> | Eu, como <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a>, posso solicitar alteração da <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> para regularizar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |

<h6 align="center">Tabela 3: Histórias de Usuários</h6>
<h6 align="center">Fonte: Autores</h6>

## 7. Backlog Completo
<p style="text-align: justify; text-indent: 20px">A partir de todos os <a href="/modelagem/agil/product_backlog/#4-epicos">épicos</a>, <a href="/modelagem/agil/product_backlog/#5-features">features</a> e <a href="/modelagem/agil/product_backlog/#6-historias-de-usuario">histórias de usuários</a> documentados foi possível fazer uma tabela completa com cada nível de granularidade relacionando-as com os devidos requisitos.</p>
<p style="text-align: justify; text-indent: 20px">A priorização não está constando por todos as histórias criadas derivam de algum requisito previamente classificado como <i>Must</i> em nossa priorização por <a href="/requisitos/priorizacao/moscow/">Moscow</a>.</p>

<center>

|Épico|Feature|User Story|Requisito|
|--|--|--|--|
|EP1|FT01|US01|<a href="/requisitos/elicitacao/introspeccao/">I01</a>|
|EP1|FT01|US02|<a href="/requisitos/elicitacao/introspeccao/">I16</a>|
|EP1|FT01|US03|<a href="/requisitos/elicitacao/introspeccao/">I16</a>|
|EP1|FT01|US04|<a href="/requisitos/elicitacao/introspeccao/">I01</a>|
|EP1|FT01|US05|<a href="/requisitos/elicitacao/introspeccao/">I01</a>|
|EP1|FT01|US06|<a href="/requisitos/elicitacao/introspeccao/">I01</a>|
|EP2|FT02|US07|<a href="/requisitos/elicitacao/introspeccao/">I02</a>|
|EP2|FT02|US08|<a href="/requisitos/elicitacao/introspeccao/">I02</a>|
|EP2|FT02|US09|<a href="/requisitos/elicitacao/introspeccao/">I02</a>|
|EP2|FT02|US10|<a href="/requisitos/elicitacao/introspeccao/">I02</a>|
|EP2|FT02|US11|<a href="/requisitos/elicitacao/introspeccao/">I09</a>|
|EP2|FT02|US12|<a href="/requisitos/elicitacao/introspeccao/">I09</a>|
|EP2|FT02|US13|<a href="/requisitos/elicitacao/introspeccao/">I09</a>|
|EP2|FT03|US14|<a href="/requisitos/elicitacao/entrevista/">E06</a>|
|EP2|FT03|US15|<a href="/requisitos/elicitacao/entrevista/">E06</a>|
|EP2|FT03|US16|<a href="/requisitos/elicitacao/entrevista/">E06</a>, <a href="/requisitos/elicitacao/introspeccao/">I13</a>|
|EP2|FT04|US17|<a href="/requisitos/elicitacao/entrevista/">E08</a>, <a href="/requisitos/elicitacao/entrevista/">E17</a>, <a href="/requisitos/elicitacao/brainstorming/">BS21</a>|
|EP2|FT04|US18|<a href="/requisitos/elicitacao/entrevista/">E08</a>, <a href="/requisitos/elicitacao/entrevista/">E17</a>, <a href="/requisitos/elicitacao/brainstorming/">BS21</a>|
|EP2|FT05|US19|<a href="/requisitos/elicitacao/entrevista/">E17</a>, <a href="/requisitos/elicitacao/introspeccao/">I08</a>|
|EP2|FT05|US20|<a href="/requisitos/elicitacao/brainstorming/">BS08</a>|
|EP2|FT05|US21|<a href="/requisitos/elicitacao/entrevista/">E13</a>, <a href="/requisitos/elicitacao/brainstorming/">BS08</a>|
|EP2|FT05|US22|<a href="/requisitos/elicitacao/entrevista/">E13</a>, <a href="/requisitos/elicitacao/brainstorming/">BS08</a>|
|EP3|FT06|US23|<a href="/requisitos/elicitacao/entrevista/">E04</a>|
|EP3|FT06|US24|<a href="/requisitos/elicitacao/entrevista/">E04</a>|
|EP3|FT07|US25|<a href="/requisitos/elicitacao/entrevista/">E04</a>|
|EP3|FT07|US26|<a href="/requisitos/elicitacao/brainstorming/">BS20</a>|
|EP3|FT08|US27|<a href="/requisitos/elicitacao/introspeccao/">I09</a>|
|EP3|FT09|US28|<a href="/requisitos/elicitacao/entrevista/">E04</a>|
|EP3|FT09|US29|<a href="/requisitos/elicitacao/entrevista/">E04</a>|

</center>
<h6 align="center">Tabela 4: Backlog completo</h6>
<h6 align="center">Fonte: Autores</h6>

## 8. Legenda
<center>

|Legenda|Significado| 
|:--:|:--:|
|EP|Épico|
|FT|Feature|
|US|User Story|
|E|Entrevista|
|I|Introspecção|
|BS|Brainstorming|

</center>

<h6 align="center">Tabela 5: Legenda</h6>
<h6 align="center">Fonte: Autores</h6>

## 9. Referências

> [1] RADIGAN, Dan. **O backlog do produto: sua lista de tarefas definitiva**. Atlassian. Disponível em: <a href="https://www.atlassian.com/br/agile/scrum/backlogs" target="_blanck">https://www.atlassian.com/br/agile/scrum/backlogs</a>. Acesso em: 13/02/2022.

> [2] **Seja colaborativo e efetivo na criação do Product Backlog**. Product Backlog Building. Disponível em: <a href="http://www.productbacklogbuilding.com/overview.php" target="_blanck">http://www.productbacklogbuilding.com/overview.php</a>. Acesso em: 13/02/2022.

> [3] REHKOPF, Max. **Epics ágeis: definição, exemplos e templates**. Atlassian. Disponível em: <a href="https://www.atlassian.com/br/agile/project-management/epics" target="_blanck">https://www.atlassian.com/br/agile/project-management/epics</a>. Acesso em: 13/02/2022.

> [4] REHKOPF, Max. **Histórias de usuário com exemplos e template**. Atlassian. Disponível em: <a href="https://www.atlassian.com/br/agile/project-management/user-stories" target="_blanck">https://www.atlassian.com/br/agile/project-management/user-stories</a>. Acesso em: 13/02/2022.

> [5]- Ventura, Plínio. **Epic, Feature e User Story: O que são e como se relacionam estes três artefatos no contexto de um product backlog**. Até o momento. Disponível em <https://www.ateomomento.com.br/epic-feature-e-user-story/>. Acesso em: 13/02/2022.