# Documento de Especificação Suplementar

## 1. Versionamento
Versão|Data|Descrição|Autor(es)
------|----|---------|--------
1.0   | 08/02/2022 | Criação do documento | João Pedro Moura |

## 2. Introdução
<p style="text-align: justify; text-indent: 20px">Durante muito tempo o processo de qualidade de software foi deixado de lado, porém com o aumento da importância da visão do usuário dentro de um produto, antigas e novas metodologias passaram a serem comumente utilizadas e se tornaram cada vez mais importante dentro de todas as fases de um software (SINGH, 2018) [1]. Uma dessas metodologias, e que a equipe optou para a modelagem dos requisitos funcionais e principalmente os não funcionais, é a modelagem FURPS+ extendida pela IBM Rational software.</p>
<p style="text-align: justify; text-indent: 20px">O acrônomo FURPS+ pode ser decomposto nas seguintes categorias: <i><b>F</b>unctionality</i> (Funcionalidade), <i><b>U</b>sability</i> (Usabilidade), <i><b>R</b>eliability</i> (Confiabilidade), <i><b>P</b>erformance</i> (Desempenho) e <i><b>S</b>upportability</i> (Suportabilidade). Por sua vez, o <b>+</b> representa os demais requisitos não funcionais que não foram abrangidos nas características anteriores.</p>
<p style="text-align: justify; text-indent: 20px">Por fim, é interessante ressaltar que apesar das divisões propostas por esse modelo não estão inclusos os atributos de portabilidade, como são evidênciados em modelos como o de McCall e na ISO 9126-1 (SINGH, 2018) [1].</p> 

## 3. Metodologia FURPS+
### 3.1 Funcionalidade
<p style="text-align: justify; text-indent: 20px">Para a categora de Funcionalidade, a metodologia define que todos o requisitos funcionais devem estar abrangidos, sendo eles portanto:</p> 

|ID|Descrição|
|:--:|:--:|
|E04| O aplicativo deve fornecer a <a href="../../../requisitos/modelagem/lexicos#cardeneta_de_campo">Caderneta de Campo</a> para <a href="../../../requisitos/modelagem/lexicos#rastreabilidade">rastreabilidade</a> das <a href="../../../requisitos/modelagem/lexicos#colher_plantio">colheitas</a> |
|E06| O <a href="../../../requisitos/modelagem/lexicos#produtor">produtor</a> deve ser capaz de <a href="../../../requisitos/modelagem/lexicos#cadastrar_plantio">cadastrar seu plantio</a> |
|E07| O produtor pode escolher em qual <a href="../../../requisitos/modelagem/lexicos#talhao">talhão</a> cadastrar o seu plantio |
|E08| O produtor deve ser capaz de cadastrar a <a href="../../../requisitos/modelagem/lexicos#aplicar_agrotoxico">aplicação de agrotóxicos</a> |
|E10| O produtor deve ser capaz de saber o <a href="../../../requisitos/modelagem/lexicos#periodo_carencia">período de carência</a> |
|E13| O <a href="../../../requisitos/modelagem/lexicos#tecnico">técnico</a> deve ser capaz de cadastrar <a href="../../../requisitos/modelagem/lexicos#agrotoxico">agrotóxicos</a> |
|E17| O aplicativo deve permitir a <a href="../../../requisitos/modelagem/lexicos#rastreabilidade">rastreabilidade</a> das <a href="../../../requisitos/modelagem/lexicos#aplicacao_agrotoxico">aplicações de agrotóxicos</a> |
|I01| Cadastro e login de <a href="../../../requisitos/modelagem/lexicos#usuario">usuário</a> com opção de recuperar senha |
|I02|O produtor deve <a href="../../../requisitos/modelagem/lexicos#visualizar_propriedade">visualizar suas propriedades</a> |
|I05| O produtor pode visualizar o perfil do <a href="../../../requisitos/modelagem/lexicos#tecnico">técnico</a> que está <a href="../../../requisitos/modelagem/lexicos#supervisionar_propriedade">monitorando sua propriedade</a> |
|I06| O produtor pode visualizar o <a href="../../../requisitos/modelagem/lexicos#plantio_plantado">status</a> de cada <a href="../../../requisitos/modelagem/lexicos#plantio">plantação</a> |
|I08| O técnico deve ter <a href="../../../requisitos/modelagem/lexicos#analisar_aplicacao_agrotoxico">acesso a foto dos agrotóxicos</a> enviadas pelos produtores |
|I09| O técnico deve visualizar as <a href="../../../requisitos/modelagem/lexicos#supervisionar_propriedade">propriedades supervisionadas</a> por ele |
|I12| O produtor pode ter acesso a recomendações e boas práticas para o produto agrícola plantado |
|I13| O produtor deve adicionar a data de colheita <a href="../../../requisitos/modelagem/lexicos#plantio_finalizado">encerrando a plantação</a> |
|I16| O usuário pode editar suas informações pessoais |
|ST05| A partir do sistema deve ser possível ao produtor enviar informações sobre as <a href="../../../requisitos/modelagem/lexicos#cultura">culturas</a> presentes nos <a href="../../../requisitos/modelagem/lexicos#talhao">talhões</a> |
|ST06| O sistema deve informar ao técnico as informações dos produtores designados |
|BS01| O técnico deve ser capaz de cadastrar um produtor |
|BS02| O técnico deve ser capaz de cadastrar uma propriedade |
|BS03| O técnico deve ser capaz de cadastrar uma plantação |
|BS05| O técnico deve ser capaz de gerenciar conta do produtor |
|BS08| O técnico deve ser capaz de gerenciar o uso de agrotoxico |
|BS09| O técnico deve ser capaz de gerar uma caderneta de campo |
|BS11| O técnico deve ser capaz de visualizar histórico de propriedades |
|BS12| O técnico deve ser capaz de visualizar histórico de plantações |
|BS14| O usuário deve ser capaz de usar o redirecionamento para o <a href="../../../requisitos/modelagem/lexicos#whatsapp">whatsapp</a> |
|BS20| O produtor deve ser capaz de visualizar <a href="../../../requisitos/modelagem/lexicos#visualizar_plantio">histórico de suas plantações</a> |
|BS21| O produtor deve ser capaz de <a href="../../../requisitos/modelagem/lexicos#visualizar_aplicacao_agrotoxico">visualizar histórico de uso de agrotóxicos</a> |

### 3.2 Usabilidade
- <b>A aplicação deve ser intuitiva para o uso tanto para <a href="../../../requisitos/modelagem/lexicos#produtor">produtores</a> como para <a href="../../../requisitos/modelagem/lexicos#tecnico">técnicos</a></b>
<p style="text-align: justify; text-indent: 20px">Pelo público alvo da aplicação serem <a href="../../../requisitos/modelagem/lexicos#produtor">produtores</a> que não possuem uma escolaridade muito alta, o aplicativo deve ser de fácil utilização, intuitivo e com textos simples. Além disso, os <a href="../../../requisitos/modelagem/lexicos#tecnico">técnicos</a> também poderão utilizar essa interface de forma eficiente facilitanto a comunicação entre ambos. Por fim, a aplicação também deve prover funcionalidades que necessitem de poucas etapas para serem concluídas.</p>
Rastros: <a href="../../../requisitos/elicitacao/entrevista">E02</a>, <a href="../../../requisitos/elicitacao/entrevista">E20</a> e <a href="../../../requisitos/storytelling/">ST01</a>

- <b>O aplicativo deve ser acessível e de fácil acesso</b>
<p style="text-align: justify; text-indent: 20px">Como já ressaltado anteriormente, a aplicação deve ser feita voltada para <a href="../../../requisitos/modelagem/lexicos#produtor">produtores</a> que não possuem níveis de escolaridade muito altos. Por esse motivo, o aplicativo deve possuir textos simples, muitas vezes acompanhados de fotos, de forma que seja acessível à todo tipo de público.</p>
Rastros: <a href="../../../requisitos/elicitacao/introspeccao">I20</a> e <a href="../../../requisitos/elicitacao/entrevista">E03</a>

### 3.3 Confiabilidade
- <b>O aplicativo deve ser confiável na garantia da <a href="../../../requisitos/modelagem/lexicos#rastreabilidade">rastreabilidade</a></b>
<p style="text-align: justify; text-indent: 20px">Por ser o foco principal do aplicativo, a <a href="../../../requisitos/modelagem/lexicos#rastreabilidade">rastreabilidade</a> deve ser segura e confiável, visto que o rastro das <a href="../../../requisitos/modelagem/lexicos#plantacao">plantações</a> é uma das características fundamentais da <a href="../../../requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a>. Para garantir a confiabilidade, o sistema também deve restringir o uso e registro de <a href="../../../requisitos/modelagem/lexicos#tecnico">técnicos</a> já cadastrados pelo Instituto de Assistência Técnica e Extensão Rural(EMATER).</p>
Rastros: <a href="../../../requisitos/elicitacao/introspeccao">I18</a> e <a href="../../../requisitos/storytelling/">ST03</a>

### 3.4 Desempenho
- <b>O aplicativo deve desempenhar suas funções de forma eficiente</b>
<p style="text-align: justify; text-indent: 20px">Para garantir o bem estar dos usuários e uma experiência agradável, é indispensável que o aplicativo seja leve, otimizado e eficiente, de forma à incluir e alcançar o maior número de usuários alvos da aplicação.</p>
Rastro: <a href="../../../requisitos/elicitacao/entrevista">E19</a>

### 3.5 Suportabilidade
- <b>O sistema deve estar disponível por meio de um aplicativo mobile e que possua acesso à camera</b>
<p style="text-align: justify; text-indent: 20px">Como já discutido em diversos documentos, são raras as ocasiões que um <a href="../../../requisitos/modelagem/lexicos#produtor">produtor</a> e um <a href="../../../requisitos/modelagem/lexicos#tecnico">técnico</a> não possuem um telefone celular para comunicação. Além disso, através da entrevista foi confirmado que muitos <a href="../../../requisitos/modelagem/lexicos#produtor">produtores</a> tem facilidade e preferência na utilização desse meio. Outro fato que reforça essa afirmação, é a capacidade do <a href="../../../requisitos/modelagem/lexicos#produtor">produtor</a> fazer o <a href="../../../requisitos/modelagem/lexicos#enviar_foto_agrotoxico">envio de fotos de agrotóxicos</a> para sanar suas dúvidas em relação ao mesmo. Por esses motivos, o desenvolvimento da aplicação deve ser feita visando telefones celulares que tenham acesso à camera.</p>
Rastro: <a href="../../../requisitos/storytelling/">ST07 </a>e <a href="../../../requisitos/storytelling/">ST08</a>

## 4. Referências
> [1] SINGH, Jagannath - User's Perspective of Software Quality. 2018.
