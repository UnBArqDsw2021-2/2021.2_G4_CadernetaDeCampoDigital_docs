## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|:------:|:----:|:---------:|:---------:|
|1.0|27/07|Abertura do documento de léxicos|João, Rafael e Thiago|
|1.1|03/02|Documentação e especificação dos léxicos|Thiago|

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
|**Noção**|Caderneta utilizada para anotações sobre aplicações de agrotóxico, entre outras informações sobre a propriedade. Permite a rastreabilidade de um plantio|
|**Impacto**|O usuário pode gerar uma caderneta de campo|

<div id="produtor"/>
|LO02|Descrição|
|----|--------------------|
|**Nome**|**Produtor**|
|**Sinônimos**|Fazendeiro|
|**Noção**|O produtor que planta um plantio em sua propriedade|
|**Impacto**|O produtor pode cadastrar plantio, aplicar agrotóxico, enviar foto, colher plantio, visualizar plantio, visualizar aplicações de agrotóxico e gerar caderneta de campo|

<div id="tecnico"/>
|LO03|Descrição|
|----|--------------------|
|**Nome**|**Técnico**|
|**Sinônimos**|Agrônomo|
|**Noção**|O técnico que auxilia o produtor na plantação|
|**Impacto**|O técnico pode supervisionar uma propriedade, analisar aplicação de agrotóxico, visualizar propriedade, visualizar plantios, visualizar aplicações de agrotóxico e notificar erro|

<div id="usuario"/>
|LO04|Descrição|
|----|--------------------|
|**Nome**|**Usuário**|
|**Sinônimos**|Cliente|
|**Noção**|A união do técnico e do produtor|
|**Impacto**|O usuário pode visualizar propriedade, visualizar aplicações de agrotóxico, visualizar plantio e gerar caderneta de campo|

<div id="propriedade"/>
|LO05|Descrição|
|----|--------------------|
|**Nome**|**Propriedade**|
|**Sinônimos**|Chácara e Fazenda|
|**Noção**|Local onde o produtor planta suas culturas|
|**Impacto**|O usuário pode visualizar propriedade<br>O produtor pode cadastrar um plantio<br>O técnico pode supervisionar a propriedade|

<div id="cultura"/>
|LO06|Descrição|
|----|--------------------|
|**Nome**|**Cultura**|
|**Sinônimos**|Alimento e/ou Vegetal|
|**Noção**|O tipo de alimento que o produtor planta|
|**Impacto**|O produtor pode plantar uma cultura|

<div id="plantio"/>
|LO07|Descrição|
|----|--------------------|
|**Nome**|**Plantio**|
|**Sinônimos**|Plantação|
|**Noção**|O ato do produtor plantar uma cultura resulta em um plantio|
|**Impacto**|O usuário pode visualizar plantio<br>O produtor pode cadastrar plantio, aplicar agrotóxico sobre um plantio, colher plantio e gerar caderneta de campo|

<div id="talhao"/>
|LO08|Descrição|
|----|--------------------|
|**Nome**|**Talhão**|
|**Sinônimos**|Porção do Terreno|
|**Noção**|A propriedade é dividida em diversos setores chamados de talhão, é a porção do terreno onde o produtor planta uma cultura|
|**Impacto**|O produtor pode cadastrar plantio em um talhão|

<div id="agrotoxico"/>
|LO09|Descrição|
|----|--------------------|
|**Nome**|**Agrotóxico**|
|**Sinônimos**|Produto Químico|
|**Noção**|Produto químico aplicado sobre um plantio|
|**Impacto**|O produtor pode aplicar agrotóxico|

<div id="tipo_agrotoxico"/>
|LO10|Descrição|
|----|--------------------|
|**Nome**|**Tipo de Agrotóxico**|
|**Sinônimos**|Classe Agrotóxico|
|**Noção**|Tipo do agrotóxico, por exemplo, herbicida ou fungicida|
|**Impacto**|O técnico pode diferenciar o agrotóxico pelo tipo|

<div id="periodo_carencia"/>
|LO11|Descrição|
|----|--------------------|
|**Nome**|**Período de Carência**|
|**Sinônimos**|Dias de Carência|
|**Noção**|Período recomendado de dias que se deve colher após a aplicação de agrotóxico|
|**Impacto**|O técnico pode notificar erro na rastreabilidade|

<div id="aplicacao_agrotoxico"/>
|LO12|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico**|
|**Sinônimos**||
|**Noção**|O registro da aplicação do agrotóxico aplicado no plantio|
|**Impacto**|O usuário pode visualizar aplicações de agrotóxico<br>O produtor pode aplicar agrotóxico e enviar foto agrotóxico<br>|

<div id="rastreabilidade"/>
|LO13|Descrição|
|----|--------------------|
|**Nome**|**Rastreabilidade**|
|**Sinônimos**|Rastro|
|**Noção**|Aquilo que possui um rastro de forma a facilitar a identificação/localização de algo|
|**Impacto**|O usuário pode gerar caderneta de campo|

<div id="whatsapp"/>
|LO14|Descrição|
|----|--------------------|
|**Nome**|**WhatsApp**|
|**Sinônimos**|Aplicativo de comunicação|
|**Noção**|Aplicação de comunicação utilizada por muitos produtores para entrar em contato com seus técnicos e tirarem dúvidas/validarem suas plantações|
|**Impacto**|O técnico pode notificar erro na rastreabilidade|

## 4.2 Verbos

<div id="cadastrar_plantio"/>
|LV01|Descrição|
|----|--------------------|
|**Nome**|**Cadastrar Plantio**|
|**Sinônimos**|Registrar Plantio; Plantar Cultura|
|**Noção**|O produtor pode registrar um plantio|
|**Impacto**|O usuário pode visualizar plantio e gerar caderneta de campo<br>O produtor pode aplicar agrotóxico e colher plantio|

<div id="aplicar_agrotoxico"/>
|LV01|Descrição|
|----|--------------------|
|**Nome**|**Aplicar Agrotóxico**|
|**Sinônimos**||
|**Noção**|O usuário pode cadastrar uma aplicação de agrotóxico|
|**Impacto**|O usuário pode visualizar aplicações de agrotóxico<br>O técnico pode analisar aplicação do agrotóxico<br>O produtor pode enviar foto do agrotóxico<br>A aplicação do agrotóxico entra em análise pelo técnico|

<div id="analisar_aplicacao_agrotoxico"/>
|LV02|Descrição|
|----|--------------------|
|**Nome**|**Analisar Aplicação do Agrotóxico**|
|**Sinônimos**||
|**Noção**|Analise se as informações da aplicação do agrotóxico estão corretas|
|**Impacto**|O técnico analisa as aplicações de agrotóxicos da propriedade que ele supervisiona<br>O técnico pode notificar erro quando encontrar algum problema<br>A aplicação de agrotóxico pode estar em análise, finalizada ou com problemas|

<div id="supervisionar_propriedade"/>
|LV03|Descrição|
|----|--------------------|
|**Nome**|**Supervisionar Propriedade**|
|**Sinônimos**||
|**Noção**|O técnico pode supervisionar propriedades|
|**Impacto**|O técnico pode visualizar propriedade, visualizar plantio, visualizar aplicações de agrotóxico, gerar caderneta de campo e analisar aplicação de agrotóxico|

<div id="visualizar_plantio"/>
|LV04|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Plantio**|
|**Sinônimos**||
|**Noção**|Visualização das informações do plantio|
|**Impacto**|O usuário pode visualizar plantio|

<div id="visualizar_propriedade"/>
|LV05|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Propriedade**|
|**Sinônimos**||
|**Noção**|Visualização das informações sobre a propriedade|
|**Impacto**|O usuário pode visualizar propriedade|

<div id="visualizar_aplicacao_agrotoxico"/>
|LV06|Descrição|
|----|--------------------|
|**Nome**|**Visualizar Aplicação de Agrotóxico**|
|**Sinônimos**||
|**Noção**|Visualização das aplicações de agrotóxico sobre um plantio|
|**Impacto**|O usuário pode visualizar aplicação de agrotóxico|

<div id="gerar_caderneta_de_campo"/>
|LV07|Descrição|
|----|--------------------|
|**Nome**|**Gerar Caderneta de Campo**|
|**Sinônimos**||
|**Noção**|Junção das informações relacionadas ao plantio em forma de uma caderneta de campo|
|**Impacto**|O usuário pode gerar a caderneta de campo|

<div id="enviar_foto_agrotoxico"/>
|LV08|Descrição|
|----|--------------------|
|**Nome**|**Enviar Foto do Agrotóxico**|
|**Sinônimos**||
|**Noção**|Envio da foto do agrotóxico aplicado sobre um plantio|
|**Impacto**|O produtor pode enviar foto do agrotóxico aplicado|

<div id="colher_plantio"/>
|LV09|Descrição|
|----|--------------------|
|**Nome**|**Colher Plantio**|
|**Sinônimos**||
|**Noção**|O produtor pode colher uma ou várias vezes um plantio|
|**Impacto**|O usuário pode gerar a caderneta de campo<br>Após colher todo o plantio, o plantio está finalizado|

<div id="notificar_erro"/>
|LV10|Descrição|
|----|--------------------|
|**Nome**|**Notificar Erro**|
|**Sinônimos**||
|**Noção**|Notificação ao produtor caso ocorra algum problema na rastreabilidade do plantio por meio do aplicativo ou whatsapp|
|**Impacto**|O técnico pode notificar erro na rastreabilidade|

## 4.3 Estados

<div id="plantio_plantado"/>
|LE01|Descrição|
|----|--------------------|
|**Nome**|**Plantio está Plantado**|
|**Sinônimos**|Cultura plantada|
|**Noção**|Plantio está Plantado significa que uma cultura plantada em um talhão ainda não foi finalizada|
|**Impacto**|O produtor pode aplicar agrotóxico e colher o plantio<br>Após colhido, o plantio está finalizado|

<div id="plantio_finalizado"/>
|LE02|Descrição|
|----|--------------------|
|**Nome**|**Plantio está Finalizado**|
|**Sinônimos**||
|**Noção**|Plantio está Finalizado significa que o produtor acabou de colher a cultura plantada em um determinado talhão|
|**Impacto**|O usuário pode gerar caderneta de campo|

<div id="aplicacao_agrotoxico_analise"/>
|LE03|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico em Análise**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico ainda está sendo analisada pelo técnico|
|**Impacto**|Após análise, a aplicação pode estar com problema ou ser finalizada com sucesso|

<div id="aplicacao_agrotoxico_problema"/>
|LE04|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico com Problemas**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico foi analisada, porém o técnico encontrou problemas|
|**Impacto**|O técnico pode notificar erro<br>Após contato com o produtor, o técnico pode finalizar a análise|

<div id="aplicacao_agrotoxico_finalizada"/>
|LE05|Descrição|
|----|--------------------|
|**Nome**|**Aplicação de Agrotóxico Finalizada**|
|**Sinônimos**||
|**Noção**|A Aplicação de Agrotóxico foi analisada com sucesso pelo técnico|
|**Impacto**|O produtor pode colher o plantio sem problemas|

## 5. Bibliografia
> [1] SERRANO, Milene; SERRANO, Maurício. Requisitos - Aula 10. 2019. 35 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.
