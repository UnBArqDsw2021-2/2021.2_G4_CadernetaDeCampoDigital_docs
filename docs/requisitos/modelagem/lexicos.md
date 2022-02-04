## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|:------:|:----:|:---------:|:---------:|
|1.0|27/07|Abertura do documento de léxicos|João, Rafael e Thiago|
|1.1|03/02|Documentação e especificação dos léxicos|Thiago|
|1.2|03/02|Linkagem dos léxicos|Thiago|

## 2. Introdução

<p style="text-align: justify; text-indent: 20px">O Léxico é uma técnica de modelagem que permite a descrição dos símbolos de uma linguagem, ele funciona como um dicionário que auxilia na identificação de palavras ou frases peculiares relativas ao meio social da aplicação que está sob estudo [1].</p>

<p style="text-align: justify; text-indent: 20px">Os símbolos da linguagem são descritos com noção e impacto, onde noção traz a tona o significado do símbolo (denotação) e impacto, como o nome já diz, descreve o efeito do símbolo na aplicação ou o efeito de algo na aplicação sobre o símbolo. É importante estar atento a algumas regras gerais, por exemplo, um símbolo pode ter ou não sinônimos, e um símbolo pode ter uma ou mais noções, bem como um ou mais impactos [1].</p>


## 3. Metodologia

<p style="text-align: justify;">Para representar os léxicos, foram definidas tabelas contendo o seguinte formato:</p>

|LCXX|**Nome do léxico**|
|----|--------------------|
|**Sinônimos**|Sinônimos do léxico|
|**Noção**|Explicação ou noção do léxico|
|**Impacto**|Ocorrência ou impacto do léxico na aplicação|

|Legenda||
|----|--------------------|
|**L**|Léxico|
|**C**|Classificação (estado, verbo ou objeto)|
|**XX**|Numeração|

## 4. Léxicos
### 4.1 Objetos

<div id="cardeneta_de_campo"/>
|LO01|Descrição|
|----|--------------------|
|**Nome**|**Caderneta de Campo**|
|**Sinônimos**||
|**Noção**|Caderneta utilizada para anotações sobre <a href="#aplicacao_agrotoxico">aplicações de agrotóxico</a>, entre outras informações sobre a <a href="#propriedade">propriedade</a>. Permite a <a href="#rastreabilidade">rastreabilidade</a> de um <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode gerar uma <a href="#cardeneta_de_campo">caderneta de campo</a>|

<div id="produtor"/>
|LO02|Descrição|
|----|--------------------|
|**Nome**|**Produtor**|
|**Sinônimos**|Fazendeiro|
|**Noção**|O produtor que planta um <a href="#plantio">plantio</a> em sua <a href="#propriedade">propriedade</a>|
|**Impacto**|O produtor pode <a href="#cadastrar_plantio">cadastrar plantio</a>, <a href="#aplicar_agrotoxico">aplicar agrotóxico</a>, enviar foto, <a href="#colher_plantio">colher plantio</a>, <a href="#visualizar_plantio">visualizar plantio</a>, <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a> e <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a>|

<div id="tecnico"/>
|LO03|Descrição|
|----|--------------------|
|**Nome**|**Técnico**|
|**Sinônimos**|Agrônomo|
|**Noção**|O técnico que auxilia o <a href="#produtor">produtor</a> na <a href="#plantio">plantação</a>|
|**Impacto**|O técnico pode supervisionar uma <a href="#propriedade">propriedade</a>, <a href="#analisar_aplicacao_agrotoxico">analisar aplicação de agrotóxico</a>, <a href="#visualizar_propriedade">visualizar propriedade</a>, <a href="#visualizar_plantio">visualizar plantios</a>, <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a> e <a href="#notificar_erro">notificar erro</a>|

<div id="usuario"/>
|LO04|Descrição|
|----|--------------------|
|**Nome**|**Usuário**|
|**Sinônimos**|Cliente|
|**Noção**|A união do <a href="#tecnico">técnico</a> e do <a href="#produtor">produtor</a>|
|**Impacto**|O usuário pode <a href="#visualizar_propriedade">visualizar propriedade</a>, <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a>, <a href="#visualizar_plantio">visualizar plantio</a> e <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a>|

<div id="propriedade"/>
|LO05|Descrição|
|----|--------------------|
|**Nome**|**Propriedade**|
|**Sinônimos**|Chácara e Fazenda|
|**Noção**|Local onde o <a href="#produtor">produtor</a> planta suas <a href="#cultura">culturas</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode <a href="#visualizar_propriedade">visualizar propriedade</a><br>O <a href="#produtor">produtor</a> pode <a href="#cadastrar_plantio">cadastrar um plantio</a><br>O <a href="#tecnico">técnico</a> pode <a href="#supervisionar_propriedade">supervisionar a propriedade</a>|

<div id="cultura"/>
|LO06|Descrição|
|----|--------------------|
|**Nome**|**Cultura**|
|**Sinônimos**|Alimento e/ou Vegetal|
|**Noção**|O tipo de alimento que o <a href="#produtor">produtor</a> planta|
|**Impacto**|O <a href="#produtor">produtor</a> pode plantar uma cultura|

<div id="plantio"/>
|LO07|Descrição|
|----|--------------------|
|**Nome**|**Plantio**|
|**Sinônimos**|Plantação|
|**Noção**|O ato do <a href="#produtor">produtor</a> plantar uma <a href="#cultura">cultura</a> resulta em um plantio|
|**Impacto**|O usuário pode <a href="#visualizar_plantio">visualizar plantio</a><br>O produtor pode <a href="#cadastrar_plantio">cadastrar plantio</a>, <a href="#aplicar_agrotoxico">aplicar agrotóxico</a> sobre um plantio, <a href="#colher_plantio">colher plantio</a> e <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a>|

<div id="talhao"/>
|LO08|Descrição|
|----|--------------------|
|**Nome**|**Talhão**|
|**Sinônimos**|Porção do Terreno|
|**Noção**|A <a href="#propriedade">propriedade</a> é dividida em diversos setores chamados de talhão, é a porção do terreno onde o <a href="#produtor">produtor</a> planta uma <a href="#cultura">cultura</a>|
|**Impacto**|O produtor pode <a href="#cadastrar_plantio">cadastrar plantio</a> em um talhão|

<div id="agrotoxico"/>
|LO09|Descrição|
|----|--------------------|
|**Nome**|**Agrotóxico**|
|**Sinônimos**|Produto Químico|
|**Noção**|Produto químico aplicado sobre um <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#produtor">produtor</a> pode <a href="#aplicar_agrotoxico">aplicar agrotóxico</a>|

<div id="tipo_agrotoxico"/>
|LO10|Descrição|
|----|--------------------|
|**Nome**|**Tipo de Agrotóxico**|
|**Sinônimos**|Classe Agrotóxico|
|**Noção**|Tipo do <a href="#agrotoxico">agrotóxico</a>, por exemplo, herbicida ou fungicida|
|**Impacto**|O <a href="#tecnico">técnico</a> pode diferenciar o agrotóxico pelo tipo|

<div id="periodo_carencia"/>
|LO11|Descrição|
|----|--------------------|
|**Nome**|**Período de Carência**|
|**Sinônimos**|Dias de Carência|
|**Noção**|Período recomendado de dias que se deve colher após a <a href="#aplicacao_agrotoxico">aplicação de agrotóxico</a>|
|**Impacto**|O técnico pode <a href="#notificar_erro">notificar erro</a> na <a href="#rastreabilidade">rastreabilidade</a>|

<div id="aplicacao_agrotoxico"/>
|LO12|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico**|
|**Sinônimos**||
|**Noção**|O registro da aplicação do <a href="#agrotoxico">agrotóxico</a> aplicado no <a href="#plantio">plantio</a>|
|**Impacto**|O usuário pode <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a><br>O <a href="#produtor">produtor</a> pode aplicar agrotóxico e enviar foto agrotóxico<br>|

<div id="rastreabilidade"/>
|LO13|Descrição|
|----|--------------------|
|**Nome**|**Rastreabilidade**|
|**Sinônimos**|Rastro|
|**Noção**|Aquilo que possui um rastro de forma a facilitar a identificação/localização de algo|
|**Impacto**|O usuário pode <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a>|

<div id="whatsapp"/>
|LO14|Descrição|
|----|--------------------|
|**Nome**|**WhatsApp**|
|**Sinônimos**|Aplicativo de comunicação|
|**Noção**|Aplicação de comunicação utilizada por muitos <a href="#produtor">produtores</a> para entrar em contato com seus <a href="#tecnico">técnicos</a> e tirarem dúvidas/validarem suas <a href="#plantio">plantações</a>|
|**Impacto**|O técnico pode <a href="#notificar_erro">notificar erro</a> na <a href="#rastreabilidade">rastreabilidade</a>|

## 4.2 Verbos

<div id="cadastrar_plantio"/>
|LV01|Descrição|
|----|--------------------|
|**Nome**|**Cadastrar Plantio**|
|**Sinônimos**|Registrar Plantio; Plantar Cultura|
|**Noção**|O <a href="#produtor">produtor</a> pode registrar um plantio|
|**Impacto**|O <a href="#usuario">usuário</a> pode <a href="#visualizar_plantio">visualizar plantio</a> e <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a><br>O produtor pode <a href="#aplicar_agrotoxico">aplicar agrotóxico</a> e <a href="#colher_plantio">colher plantio</a>|

<div id="aplicar_agrotoxico"/>
|LV02|Descrição|
|----|--------------------|
|**Nome**|**Aplicar Agrotóxico**|
|**Sinônimos**||
|**Noção**|O <a href="#usuario">usuário</a> pode cadastrar uma aplicação de <a href="#agrotoxico">agrotóxico</a>|
|**Impacto**|O usuário pode <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a><br>O <a href="#tecnico">técnico</a> pode analisar aplicação do agrotóxico<br>O <a href="#produtor">produtor</a> pode <a href="#enviar_foto_agrotoxico">enviar foto do agrotóxico</a><br>A aplicação do agrotóxico entra em análise pelo técnico|

<div id="analisar_aplicacao_agrotoxico"/>
|LV03|Descrição|
|----|--------------------|
|**Nome**|**Analisar Aplicação do Agrotóxico**|
|**Sinônimos**||
|**Noção**|Analise se as informações da aplicação do <a href="#agrotoxico">agrotóxico</a> estão corretas|
|**Impacto**|O <a href="#tecnico">técnico</a> analisa as <a href="#aplicacao_agrotoxico">aplicações de agrotóxicos</a> da <a href="#propriedade">propriedade</a> que ele supervisiona<br>O técnico pode <a href="#notificar_erro">notificar erro</a> quando encontrar algum problema<br>A aplicação de agrotóxico pode estar em análise, finalizada ou com problemas|

<div id="supervisionar_propriedade"/>
|LV04|Descrição|
|----|--------------------|
|**Nome**|**Supervisionar Propriedade**|
|**Sinônimos**||
|**Noção**|O <a href="#tecnico">técnico</a> pode supervisionar <a href="#propriedade">propriedades</a>|
|**Impacto**|O técnico pode <a href="#visualizar_propriedade">visualizar propriedade</a>, <a href="#visualizar_plantio">visualizar plantio</a>, <a href="#visualizar_aplicacao_agrotoxico">visualizar aplicações de agrotóxico</a>, <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a> e <a href="#analisar_aplicacao_agrotoxico">analisar aplicação de agrotóxico</a>|

<div id="visualizar_plantio"/>
|LV05|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Plantio**|
|**Sinônimos**||
|**Noção**|Visualização das informações do <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode visualizar plantio|

<div id="visualizar_propriedade"/>
|LV06|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Propriedade**|
|**Sinônimos**||
|**Noção**|Visualização das informações sobre a <a href="#propriedade">propriedade</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode visualizar propriedade|

<div id="visualizar_aplicacao_agrotoxico"/>
|LV07|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Aplicação de Agrotóxico**|
|**Sinônimos**||
|**Noção**|Visualização das aplicações de agrotóxico sobre um <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode visualizar aplicação de agrotóxico|

<div id="gerar_caderneta_de_campo"/>
|LV08|Descrição|
|----|--------------------|
|**Nome**|**Gerar Caderneta de Campo**|
|**Sinônimos**||
|**Noção**|Junção das informações relacionadas ao plantio em forma de uma <a href="#cardeneta_de_campo">caderneta de campo</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode gerar a caderneta de campo|

<div id="enviar_foto_agrotoxico"/>
|LV09|Descrição|
|----|--------------------|
|**Nome**|**Enviar Foto do Agrotóxico**|
|**Sinônimos**||
|**Noção**|Envio da foto do agrotóxico aplicado sobre um <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#produtor">produtor</a> pode enviar foto do agrotóxico aplicado|

<div id="colher_plantio"/>
|LV010|Descrição|
|----|--------------------|
|**Nome**|**Colher Plantio**|
|**Sinônimos**||
|**Noção**|O <a href="#produtor">produtor</a> pode colher uma ou várias vezes um <a href="#plantio">plantio</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode gerar a caderneta de campo<br>Após colher todo o plantio, o <a href="#plantio_finalizado">plantio está finalizado</a>|

<div id="notificar_erro"/>
|LV11|Descrição|
|----|--------------------|
|**Nome**|**Notificar Erro**|
|**Sinônimos**||
|**Noção**|Notificação ao <a href="#produtor">produtor</a> caso ocorra algum problema na <a href="#rastreabilidade">rastreabilidade</a> do <a href="#plantio">plantio</a> por meio do aplicativo ou whatsapp|
|**Impacto**|O <a href="#tecnico">técnico</a> pode notificar erro na rastreabilidade|

## 4.3 Estados

<div id="plantio_plantado"/>
|LE01|Descrição|
|----|--------------------|
|**Nome**|**Plantio está Plantado**|
|**Sinônimos**|Cultura plantada|
|**Noção**|<a href="#plantio">Plantio</a> está Plantado significa que uma <a href="#cultura">cultura</a> plantada em um <a href="#talhao">talhão</a> ainda não foi finalizada|
|**Impacto**|O <a href="#produtor">produtor</a> pode <a href="#aplicar_agrotoxico">aplicar agrotóxico</a> e colher o plantio<br>Após colhido, o <a href="#plantio_finalizado">plantio está finalizado</a>|

<div id="plantio_finalizado"/>
|LE02|Descrição|
|----|--------------------|
|**Nome**|**Plantio está Finalizado**|
|**Sinônimos**||
|**Noção**|Plantio está Finalizado significa que o <a href="#produtor">produtor</a> acabou de colher o <a href="#plantio_plantado">plantio plantado</a> em um determinado <a href="#talhao">talhão</a>|
|**Impacto**|O <a href="#usuario">usuário</a> pode <a href="#gerar_caderneta_de_campo">gerar caderneta de campo</a>|

<div id="aplicacao_agrotoxico_analise"/>
|LE03|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico em Análise**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico ainda está sendo analisada pelo <a href="#tecnico">técnico</a>|
|**Impacto**|Após análise, a aplicação pode estar com problema ou ser finalizada com sucesso|

<div id="aplicacao_agrotoxico_problema"/>
|LE04|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico com Problemas**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico foi analisada, porém o técnico encontrou problemas|
|**Impacto**|O <a href="#tecnico">técnico</a> pode <a href="#notificar_erro">notificar erro</a><br>Após contato com o <a href="#produtor">produtor</a>, o técnico pode finalizar a análise|

<div id="aplicacao_agrotoxico_finalizada"/>
|LE05|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico Finalizada**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico foi analisada com sucesso pelo <a href="#tecnico">técnico</a>|
|**Impacto**|O <a href="#produtor">produtor</a> pode colher o plantio sem problemas|

## 5. Bibliografia
> [1] SERRANO, Milene; SERRANO, Maurício. Requisitos - Aula 10. 2019. 35 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.
