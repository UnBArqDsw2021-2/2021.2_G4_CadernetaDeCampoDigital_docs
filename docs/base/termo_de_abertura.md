# Termo de Abertura de Projeto (TAP)

## 1. Versionamento
| Versão | Data | Modificação | Autor |
|--|--|--|--|
|1.0| 30/01/2022| Criação do documento | João Pedro Moura |
|1.1| 30/01/2022| Adição dos riscos | João Pedro Moura |
|1.2| 30/01/2022| Adição dos custos | João Pedro Moura |

## 2. Introdução
<p align="justify">&emsp;&emsp; Esse documento tem como principal objetivo formalizar o início do projeto informando os estudos de viabilidade, prazos e entregas, orçamentos, objetivos e os riscos para a contrução de todos os documentos e softwares desse programa.</p>

## 3. Objetivos
<p align="justify">&emsp;&emsp; O objetivo principal é construir um aplicativo que um <a href=#produtor>produtor</a> possa estar utilizando para realizar o <a href=#envio_fotos>envio de fotos</a> de <a href=#agrotoxico>agrotóxicos</a> para a confecção de sua <a href=#cardeneta_de_campo>cardeneta de campo</a> de um <a href=#talhao>talhão</a> de sua <a href=#propriedade>propriedade</a>, através do preenchimento pós-analise de um <a href=#tecnico>técnico</a> sobre as fotos enviadas e sobre a <a href=#cultura>cultura</a> que está recebendo a aplicação do <a href=#agrotoxico>agrotóxico</a>.</p>

## 4. Justificativa
<p align="justify">&emsp;&emsp; O registro e venda de produtos agrícolas exige um mapeamento preciso e bem feito, de forma que uma cultura possa ser facilmente <a href=#rastreabilidade>rastreável</a>, e caso ocorram problemas, seja de fácil descobrimento a sua causa. Entretanto, é necessário um nível de conhecimento de leitura e escrita elevado para a confecção de uma <a href=#cardeneta_de_campo>cardeneta de campo</a> de acordo com os padrões exigidos.</p>
<p align="justify">&emsp;&emsp; Por esse motivo, os <a href=#tecnico>técnicos</a> que são os responsáveis por realizar o preenchimento desse artefato, visto que muitos <a href=#produtor>produtores</a> são analfabetos e/ou não possuem total conhecimento sobre tal documento. Dessa forma, para criar uma plataforma de fácil utilização tanto para <a href=#produtor>produtores</a> como para <a href=#tecnico>técnicos</a> é que surge a premissa principal desse projeto.</p>

## 5. Prazos e Entregas
<p align="justify">&emsp;&emsp; A entrega desse produto será feita em partes e conforme o que foi definido no plano de ensino da matéria de Arquitetura e Desenho de Software da professora Milene, a seguir se encontram os principais marcos da evolução desse projeto:</p>

<center>

|Entrega|Estimativa de Entrega|
|:-:|:-:|
|Base|04/02/2022|
|Modelagem|21/02/2022|
|Padrões de Projeto|21/03/2022|
|Reutilização de Software|18/04/2022|

</center>

<h6 align = "center">Tabela 1: Tabela de prazos e entregas.</h6>
<h6 align = "center">Fonte: Autor.</h6>

## 6. Riscos
<p align="justify">&emsp;&emsp; Dentro da gerência de um projeto de software, um dos pontos essênciais é realizar a gestão de riscos do produto. Com esse controle, é possível a equipe entender, listar, acompanhar, controlar, previnir e medir os impactos de cada risco dentro de todos os ciclos de vida do software que está sendo construído. Com essa medição, é possível focalizar nos riscos com uma maior prioridade - não ignorando aqueles com prioridade inferior - e tomar medidas para previnir seus acontecimentos [1].</p>

### 6.1 Estrutura Analítica de Riscos (EAR)
<p align="justify">&emsp;&emsp; Uma das ferramentas utilizadas para gerir os riscos desse projeto é a Estrutura Analítica de Riscos (EAR), que corresponde a uma ferramenta de agrupamento e organização dos riscos em categorias [2], a seguir é possível visualizer essa categorização de forma visual para o projeto:</p>
![EAR](../assets/ear/ear.png)
<h6 align = "center">Figura 1: Estrutura Analítica de Riscos.</h6>
<h6 align = "center">Fonte: Autor, baseado no projeto Curumim [3].</h6>

#### 6.1.1 Externo
- Cliente: Diz respeito à critério de aceitação dos clientes desde etapas inicias de elicitação de requisitos até a utilização diária da aplicação.
- Pandemia: Diz respeito à atual situação do mundo, com a pandemia do Covid-19 e da nova gripe H3N2.

#### 6.1.2 Organizacional
- Depêndencias de Projeto: Se refere à possíveis riscos advindo de depêndencias utilizadas dentro do projeto, sendo aplicável também aos riscos técnicos.
- Financiamento: Referente à riscos em relação aos custos do projeto e possíveis financiamentos de interessados.
- Recursos: Similar aos riscos de financiamento e também diretamente ligado aos custos do projeto.
- Priorização: Riscos influênciados pelo cliente e possíveis priorizações equivocadas dos requisitos.

#### 6.1.3 Técnico
- Framework: Diz respeito à riscos de software em relação à frameworks utilizados.
- Qualidade: Referente a modelagem FURPS+ dos requisitos dentro de todo o escopo do projeto e sua utilização.
- Infraestrutura: Riscos advindos de plataformas que fornecem serviços de hospedagem.
- Desempenho: Diretamente relacionados à velocidade e eficiência da aplicação construida.

#### 6.1.4 Gerencial
- Estimativas: Riscos relacionados aos prazos de entregas e estimativas.
- Comunicação: Diz respeito à comunicação entre membros de equipe.
- Planejamento: Referentes aos riscos de um planejamento mal feito ou equivocado.

### 6.2 Strength, Weakness, Opportunity, and Threat (SWOT)
<p align="justify">&emsp;&emsp; Framework de gerência de riscos usado para avaliação competitiva e planejamento estratégico. Essa análise, busca projetar uma visão realista baseada em fatos e orientada por dados dos pontos fortes e fracos de uma organização [4].</p>

<style>
    #celula {
        vertical-align: middle;
        text-align: center;
        border: 0.5px solid rgba(0,0,0,0.2);
    }
</style>

<center>
<table>
<tr>
    <td id="celula">Forças</td>
    <td id="celula">Comprometimento da equipe, experiências prévias dentros dos frameworks escolhidos, comunicação eficaz entre membros.</td>
</tr>
<tr>
    <td id="celula">Fraquezas</td>
    <td id="celula">Falta de conhecimento, atraso de entregas indivudais.</td>
</tr>
<tr>
    <td id="celula">Oportunidades</td>
    <td id="celula">Possibilidade de continuidade do projeto, capacitação em novas linguagens/frameworks, aquisição de conhecimentos em novas áreas do desenvolvimento de softwares.</td>
</tr>
<tr>
    <td id="celula">Ameaças</td>
    <td id="celula">Greves da faculdade, doenças.</td>
</tr>
</table>
</center>

<h6 align = "center">Tabela 2: Tabela SWOT.</h6>
<h6 align = "center">Fonte: Autor.</h6>

### 6.3 Análise Quantitativa de Riscos
<p align="justify">&emsp;&emsp; Partindo agora para uma análise dos riscos através de dados mensuráveis e numéricos, a equipe optou por utilizar a Análise Quantitativa de Riscos [5]. Para realizar esse levantamento, utilizou-se a matriz de probabilidade e impacto que especifica as possíveis combinações e permite uma classificação dos riscos de acordo com uma prioridade. A seguir se encontram as tabelas:</p>

#### 6.3.1 Probabilidade
<center>

|Peso|Atributo|Probabilidade|
|:-:|:-:|:-:|
|5|Esperado|81 ~ 100%|
|4|Muito Provável|61 ~ 80%|
|3|Provável|41 ~ 60%|
|2|Pouco Provável|21 ~ 40%|
|1|Quase Nulo|0 ~ 20%|

</center>

<h6 align = "center">Tabela 3: Tabela de probabilidades.</h6>
<h6 align = "center">Fonte: Autor.</h6>

#### 6.3.2 Impacto
<center>

|Peso|Impacto|Descrição|
|:-:|:-:|:-:|
|5|Alto|Impossibilita a continuação do projeto|
|4|Elevado|Alto impacto no andamento do projeto|
|3|Moderado|Afeta o projeto, mas tem solução|
|2|Baixo|Influência baixa dentro do projeto|
|1|Limitado|Impacto quase nulo|

</center>

<h6 align = "center">Tabela 4: Tabela de impacto.</h6>
<h6 align = "center">Fonte: Autor.</h6>

#### 6.3.3 Prioridade (Probabilidade x Impacto)
<center>

|P/I|Limitado|Baixo|Moderado|Elevado|Alto|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Quase Nulo|1|2|3|4|5|
|Pouco Provável|2|4|6|8|10|
|Provável|3|6|9|12|15|
|Muito Provável|4|8|12|16|20|
|Esperado|5|10|15|20|25|

</center>

<h6 align = "center">Tabela 5: Tabela de prioridade.</h6>
<h6 align = "center">Fonte: Autor.</h6>

#### 6.3.4 Riscos Identificados
##### 6.3.4.1 Riscos Externos
<center>

|Risco|Impacto|Probabilidade|Prevenção|Resposta|Prioridade|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Desistência do cliente|Elevado|Pouco Provável|Sempre estar em sincronia com os desejos do cliente e com o que está sendo produzido|Buscar novo cliente com ideias similares e adaptar o projeto|8|
|Indiponibilidade de um integrante por doença|Moderado|Provável|Buscar sempre atender as prevenções para o Covid-19 e a nova gripe H3N2|Alocação de membros para as issues que ficarem desfalcadas|9|

</center>

<h6 align = "center">Tabela 6: Tabela de riscos externos.</h6>
<h6 align = "center">Fonte: Autor.</h6>

##### 6.3.4.2 Riscos Organizacionais
<center>

|Risco|Impacto|Probabilidade|Prevenção|Resposta|Prioridade|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Desistência de integrante da matéria|Alto|Pouco Provável|Manter motivação dos membros sempre alta e uma boa gerência de equipe|Realocação das issues para os membros restantes|10|
|Priorização equivocada de requisitos|Elevado|Pouco Provável|Realizar uma elicitação e priorização condizente com as necessidades dos clientes|Realizar nova elicitação e priorização de requisitos|8|
|Falta de recursos e financiamento|Limitado|Quase Nulo|Buscar atender as necessidades do cliente para que se mantenham os financiamentos|Por se tratar de um projeto open source para uma disciplina, não será procurado novas fontes de financiamento|1|

</center>

<h6 align = "center">Tabela 7: Tabela de riscos organizacionais.</h6>
<h6 align = "center">Fonte: Autor.</h6>

##### 6.3.4.3 Riscos Técnicos
<center>

|Risco|Impacto|Probabilidade|Prevenção|Resposta|Prioridade|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Dificuldades com as tecnologias utilizadas|Moderado|Pouco Provável|Treinamentos e pareamentos|Buscar treinamentos e troca de conhecimentos na equipe|6|
|Falhas na infraestrutura do sistema|Alto|Provável|Utilização de boas plataformas de hospedagens para a infraestrutura do projeto|Alterar a plataforma responsável pela hospedagem do projeto|15|
|Baixo desempenho da aplicação|Alto|Provável|Criação/utilização de programas eficientes|Procurar novas implementações mais eficientes para determinado problema|15|
|Descontinuidade de Frameworks|Alto|Quase Nulo|Utilização de frameworks famosos e em constante desenvolvimento|Alteração de framework e em casos extremos da linguagem de programação|5|

</center>

<h6 align = "center">Tabela 8: Tabela de riscos técnicos.</h6>
<h6 align = "center">Fonte: Autor.</h6>

##### 6.3.4.4 Riscos Gerenciais
<center>

|Risco|Impacto|Probabilidade|Prevenção|Resposta|Prioridade|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Falta de planejamento|Alto|Pouco Provável|Planejar bem sempre previamente às entregas|Buscar alcançar um replanejamento para o tempo restante|10|
|Falhas de comunicação entre a equipe|Elevado|Quase Nulo|Utilizar formas de engajar e aumentar a comunicação entre a equipe|Alocar issues em pares e usar atividades de enganjamento|4|
|Falta de atenção nas datas de entrega|Alto|Quase Nulo|Sempre estar preparado previamente e ler o plano de ensino da matéria|Realocar membros para realizar as tarefas restantes|5|

</center>

<h6 align = "center">Tabela 9: Tabela de riscos gerenciais.</h6>
<h6 align = "center">Fonte: Autor.</h6>


## 7. Custos

## 8. Referências
> [1] **Gerenciando os riscos do projeto com a matriz de probabilidade e impacto**. Disponível em: <a href=https://danielettinger.com/2011/06/14/gerenciando-os-riscos-do-projeto-com-a-matriz-de-probabilidade-e-impacto/ target="_blanck">https://danielettinger.com/2011/06/14/gerenciando-os-riscos-do-projeto-com-a-matriz-de-probabilidade-e-impacto/</a>. Acesso em: 30 de jan. de 2022.</p>
> [2] **Gerenciando os riscos do projeto com a matriz de probabilidade e impacto**. Disponível em: <a href=https://glicfas.com.br/estrutura-analitica-de-riscos-2/ target="_blanck">https://glicfas.com.br/estrutura-analitica-de-riscos-2/</a>. Acesso em: 30 de jan. de 2022.</p>
> [3] **Termo de Abertura de Projeto**, Projeto Curumin. Disponível em: <a href=https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/base/tap/tap/#introducao target="_blanck">https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/base/tap/tap/#introducao</a>. Acesso em: 30 de jan. de 2022.</p>
> [4] **Strength, Weakness, Opportunity, and Threat (SWOT) Analysis**, Investopedia. Disponível em: <a href=https://www.investopedia.com/terms/s/swot.asp target="_blanck">https://www.investopedia.com/terms/s/swot.asp</a>. Acesso em: 30 de jan. de 2022.</p>
