## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|------|----|---------|---------|
|1.0|03/02|Abertura do documento de MoSCoW|Victor Lima|
|1.1|03/02|Adição da Priorização e Legenda|Victor Lima|
|1.2|03/02|Adição da Introdução|Victor Lima|
|1.3|03/02|Adição da tabela com os requisitos priorizados|Paulo Vitor, Rafael Ramos, Victor Lima|
|1.4|03/02|Linkagem dos léxicos|Thiago|

## 2. Introdução
<p style="text-align: justify; text-indent: 20px">MoSCoW é uma técnica de priorização de requisitos que serve para definir quais são os requisitos elicitados mais importantes para serem tratados de forma mais urgente [1]. Eles são divididos em grupos de acordo com o anagrama. M significa "must" que seriam os requisitos que o sistema deve ter obrigatoriamente, S significa "should" que são os requisitos que são importantes mas não são vitais para o projeto, C significa "could" que são os requisitos desejáveis mas não são necessários para a entrega e satisfação do cliente e o W significa "would" que são os requisitos menos críticos que não serão feitos pois terão baixo retorno no produto final, ou podem apenas serem deixados para o final do projeto. Temos na seção seguinte a priorização MoSCoW que fizemos relativas ao aplicativo da Caderneta de Campo Digital. </p>


## 3. Priorização:

|ID|Descrição|Tipo de Requisito|Priorização| 
|:--:|:--:|:-----:|: -----:| 
|E04| O aplicativo deve fornecer a <a href="../../modelagem/lexicos#cardeneta_de_campo">Caderneta de Campo</a> para <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> das <a href="../../modelagem/lexicos#colher_plantio">colheitas</a> | RF | <b>MUST</b> | 
|E06| O <a href="../../modelagem/lexicos#produtor">produtor</a> deve ser capaz de <a href="../../modelagem/lexicos#cadastrar_plantio">cadastrar seu plantio</a> | RF | <b>MUST</b> | 
|E07| O produtor pode escolher em qual <a href="../../modelagem/lexicos#talhao">talhão</a> cadastrar o seu plantio | RF | <b>SHOULD</b> | 
|E08| O produtor deve ser capaz de cadastrar a <a href="../../modelagem/lexicos#aplicar_agrotoxico">aplicação de agrotóxicos</a> | RF | <b>MUST</b> | 
|E10| O produtor deve ser capaz de saber o <a href="../../modelagem/lexicos#periodo_carencia">período de carência</a> | RF | <b>COULD</b> | 
|E13| O <a href="../../modelagem/lexicos#tecnico">técnico</a> deve ser capaz de cadastrar <a href="../../modelagem/lexicos#agrotoxico">agrotóxicos</a> | RF | <b>MUST</b> | 
|E17| O aplicativo deve permitir a <a href="../../modelagem/lexicos#rastreabilidade">rastreabilidade</a> das <a href="../../modelagem/lexicos#aplicacao_agrotoxico">aplicações de agrotóxicos</a> | RF | <b>MUST</b> | 
|I01| Cadastro e login de <a href="../../modelagem/lexicos#usuario">usuário</a> com opção de recuperar senha | RF | <b>MUST</b> | 
|I02|O produtor deve <a href="../../modelagem/lexicos#visualizar_propriedade">visualizar suas propriedades</a> | RF | <b>MUST</b> | 
|I05| O produtor pode visualizar o perfil do <a href="../../modelagem/lexicos#tecnico">técnico</a> que está <a href="../../modelagem/lexicos#supervisionar_propriedade">monitorando sua propriedade</a> | RF | <b>SHOULD</b> | 
|I06| O produtor pode visualizar o <a href="../../modelagem/lexicos#plantio_plantado">status</a> de cada <a href="../../modelagem/lexicos#plantio">plantação</a> | RF | <b>COULD</b> | 
|I08| O técnico deve ter <a href="../../modelagem/lexicos#analisar_aplicacao_agrotoxico">acesso a foto dos agrotóxicos</a> enviadas pelos produtores | RF | <b>MUST</b> | 
|I09| O técnico deve visualizar as <a href="../../modelagem/lexicos#supervisionar_propriedade">propriedades supervisionadas</a> por ele | RF | <b>MUST</b> | 
|I12| O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola plantado | RF | <b>WOULD</b> | 
|I13| O produtor deve adicionar a data de colheita <a href="../../modelagem/lexicos#plantio_finalizado">encerrando a plantação</a> | RF | <b>MUST</b> | 
|I16| O usuário pode editar suas informações pessoais | RF | <b>MUST</b> | 
|ST05| A partir do sistema deve ser possível ao produtor enviar informações sobre as <a href="../../modelagem/lexicos#cultura">culturas</a> presentes nos <a href="../../modelagem/lexicos#talhao">talhões</a> | RF | <b>SHOULD</b> | 
|ST06| O sistema deve informar ao técnico as informações dos produtores designados | RF | <b>SHOULD</b> |
|BS01| O técnico deve ser capaz de cadastrar um produtor | RF | <b>WOULD</b> | 
|BS02| O técnico deve ser capaz de cadastrar uma propriedade | RF | <b>WOULD</b> | 
|BS03| O técnico deve ser capaz de cadastrar uma plantação | RF | <b>WOULD</b> | 
|BS05| O técnico deve ser capaz de gerenciar conta do produtor | RF | <b>WOULD</b> | 
|BS08| O técnico deve ser capaz de gerenciar o uso de agrotoxico | RF | <b>MUST</b> | 
|BS09| O técnico deve ser capaz de gerar uma caderneta de campo | RF | <b>WOULD</b> | 
|BS11| O técnico deve ser capaz de visualizar histórico de propriedades | RF | <b>SHOULD</b> | 
|BS12| O técnico deve ser capaz de visualizar histórico de plantações | RF | <b>SHOULD</b> | 
|BS14| O usuário deve ser capaz de usar o redirecionamento para o <a href="../../modelagem/lexicos#whatsapp">whatsapp</a> | RF | <b>COULD</b> |  
|BS20| O produtor deve ser capaz de visualizar <a href="../../modelagem/lexicos#visualizar_plantio">histórico de suas plantações</a> | RF | <b>MUST</b> | 
|BS21| O produtor deve ser capaz de <a href="../../modelagem/lexicos#visualizar_aplicacao_agrotoxico">visualizar histórico de uso de agrotóxicos</a> | RF | <b>MUST</b> |
|E02|O aplicativo deve ser intuitivo| RNF | <b>MUST</b> |
|E03|O aplicativo deve possuir textos simples| RNF | <b>SHOULD</b> |
|E19|O aplicativo deve possuir um bom desempenho| RNF | <b>SHOULD</b> |
|E20|O aplicativo deve possuir uma boa usabilidade| RNF | <b>MUST</b> |
|I18|O aplicativo deve ser seguro para garantir o rastreamento das plantações| RNF | <b>MUST</b> |
|I20|O aplicativo deve ser acessível| RNF | <b>SHOULD</b> |
|ST01|A aplicação deve proporcionar uma interface com elementos visuais autoexplicativos| RNF | <b>MUST</b> |
|ST02|A aplicação deve permitir aos usuários acesso às propriedades com poucas etapas| RNF | <b>SHOULD</b> |
|ST03|O sistema deve permitir o uso apenas de pessoas já cadastradas pelo Instituto de Assistência Técnica e Extensão Rural(EMATER)| RNF | <b>COULD</b> |
|ST07|O sistema precisará ter acesso à camera do celular| RNF | <b>MUST</b> |
|ST08|A aplicação deverá ser disponibilizada por meio um aplicativo| RNF | <b>MUST</b> |


<h6 align="center">Tabela 1: Requisitos priorizados utilizando MoSCoW</h6>
<h6 align="center">Fonte: Autores</h6>

### 3.1 Legenda
<center>

|Legenda|Significado| 
|:--:|:--:|
|RF|Requisito Funcional|
|RNF|Requisito Não Funcional|
|E|Entrevista|
|I|Introspecção|
|BS|Brainstorming|
|ST|Storytelling|

</center>

<h6 align="center">Tabela 2: Legenda referente à Tabela 1</h6>
<h6 align="center">Fonte: Autores</h6>


## 4. Conclusões

<p style="text-align: justify; text-indent: 20px">Após feita a priorização, os resultados obtidos referente à quantidade de requisitos em cada nível de prioridade foi:</p>

<center>

|Prioridade|Quantidade| 
|:--:|:--:|
|MUST|20|
|SHOULD|10|
|COULD|4|
|WOULD|6|


</center>


## 5. Referências
> [1] <b>Aprenda como o método MoSCoW poderá ajudá-lo a priorizar tarefas da sua empresa</b>. Disponível em: <a href="https://www.voitto.com.br/blog/artigo/metodo-moscow" target="_blanck">https://www.voitto.com.br/blog/artigo/metodo-moscow</a>. Acesso em: 2 de fev. de 2022.