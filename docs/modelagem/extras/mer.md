# Modelo Entidade-Relacionamento

## 1. Versionamento

| Versão | Data       | Descrição                                        | Autor(es)           |
| ------ | ---------- | ------------------------------------------------ | ------------------- |
| 1.0    | 13/02/2022 | Abertura do documento                            | Thiago              |
| 1.1    | 13/02/2022 | Introdução do documento                          | Rafael Ramos        |
| 1.1.1  | 14/02/2022 | Revisão por pares                                | João Pedro e Carlos |
| 1.2    | 17/02/2022 | Correção de formato e erros                      | Thiago              |
| 1.3    | 17/02/2022 | Adição do atributo de estado                     | Thiago              |
| 1.3.1  | 20/02/2022 | Melhoria do tópico de metodologia                | Rafael e João Pedro |
| 1.4    | 20/02/2022 | Adição da entidade talhão e seus relacionamentos | Rafael              |

## 2. Introdução

<p align="justify" style="text-indent: 20px">O Modelo de Entidade-Relacionamento (ME-R) foi elaborado para facilitar o projeto de um Banco de Dados, por meio da especificação de um esquema de negócio que representa a estrutura lógica geral de um banco de dados (SILBERSCHATZ) [1]. É constituído por um conjunto de objetos básicos que são as Entidades, seus relacionamentos e atributos, baseia-se na percepção abstrata do mundo real e corresponde a uma visão lógica de alto nível dos dados [2]. </p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">O modelo foi elaborado pelo Rafael e pelo Thiago, através de uma reunião no Discord (canal de comunicação da equipe) no dia 13 de fevereiro de 2022.</p>

## 4. Entidades

- [USUARIO](../../../requisitos/modelagem/lexicos#usuario)
- [PRODUTOR](../../../requisitos/modelagem/lexicos#produtor)
- [TECNICO](../../../requisitos/modelagem/lexicos#tecnico)
- [PROPRIEDADE](../../../requisitos/modelagem/lexicos#propriedade)
- [TALHAO](../../../requisitos/modelagem/lexicos#talhao)
- [PLANTIO](../../../requisitos/modelagem/lexicos#plantio)
- [CADERNETA_DE_CAMPO](../../../requisitos/modelagem/lexicos#cardeneta_de_campo)
- [CULTURA](../../../requisitos/modelagem/lexicos#cultura)
- [AGROTOXICO](../../../requisitos/modelagem/lexicos#agrotoxico)
- [TIPO_AGROTOXICO](../../../requisitos/modelagem/lexicos#tipo_agrotoxico)

## 5. Descrição das Entidades

- USUARIO ( <span style="text-decoration: underline;">idUsuario</span>, cpf, nome, dataNascimento, senha, telefone )
- PRODUTOR ( <span style="text-decoration: underline;">idUsuario</span>, dap )
- TECNICO ( <span style="text-decoration: underline;">idUsuario</span>, crea, formacao, email, emailVerificado )
- PROPRIEDADE ( <span style="text-decoration: underline;">idPropriedade</span>, idProdutor, idTecnico, endereco(cep, cidade, bairro, logradouro, numero, complemento), hectares )
- TALHAO ( <span style="text-decoration: underline;">idTalhao</span>, idPropriedade, numero, estaAtivo)
- PLANTIO ( <span style="text-decoration: underline;">idPlantio</span>, numeroTalhao, idPropriedade, dataPlantio, idCultura, estado )
- CADERNETA_DE_CAMPO ( <span style="text-decoration: underline;">numeroSerie</span>, dataColheita, idPlantio )
- CULTURA ( <span style="text-decoration: underline;">idCultura</span>, nome )
- AGROTOXICO ( <span style="text-decoration: underline;">idAgrotoxico</span>, nome, idTipoAgrotoxico )
- TIPO_AGROTOXICO ( <span style="text-decoration: underline;">idTipoAgrotoxico</span>, nome )

## 6. Relacionamentos

<ul>
<li align="justify"><b>PLANTIO - registra - CADERNETA_DE_CAMPO</b>: Um PLANTIO registra apenas uma ou várias CADERNETA_DE_CAMPO, e uma CADERNETA_DE_CAMPO é registrada por apenas um PLANTIO. <br/>Cardinalidade: (1,n)</li>

<li align="justify"><b>PLANTIO - possui - CULTURA</b>: Um PLANTIO possui apenas uma CULTURA, e uma CULTURA pode ser
  possuída por um ou vários PLANTIO. <br/>Cardinalidade: (n,1)</li>

<li align="justify"><b>PLANTIO - plantado - TALHAO</b>: Um PLANTIO é plantado em um TALHAO e um TALHAO 
  pode ter plantado um ou mais PLANTIO. <br/>Cardinalidade: (n,1)</li>

<li align="justify"><b>TALHAO - pertence - PROPRIEDADE</b>: Um TALHAO pertence a uma PROPRIEDADE e uma PROPRIEDADE
  possui um ou mais TALHAO. <br/>Cardinalidade: (n,1)</li>

<li align="justify"><b>PRODUTOR - detem - PROPRIEDADE</b>: Um PRODUTOR detém uma ou mais PROPRIEDADE, e uma
  PROPRIEDADE pertence a apenas um PRODUTOR. <br/>Cardinalidade: (1,n)</li>

<li align="justify"><b>PLANTIO - contem - AGROTOXICO</b>: Um PLANTIO pode conter nenhum ou vários AGROTOXICO, e um
  AGROTOXICO pode estar em um ou vários PLANTIO. <br/>Cardinalidade: (n,m)</li>

<li align="justify"><b>AGROTOXICO - tem - TIPO_AGROTOXICO</b>: Um AGROTOXICO tem um TIPO_AGROTOXICO, e um
  TIPO_AGROTOXICO pode ser de um ou vários AGROTOXICO. <br/>Cardinalidade: (n,1)</li>

<li align="justify"><b>CULTURA - espera - AGROTOXICO</b>: Uma CULTURA espera por um ou vários AGROTOXICO, e um
  AGROTOXICO pode ser aplicado em uma ou várias CULTURA. <br/>Cardinalidade: (n,m)</li>

<li align="justify"><b>TECNICO - supervisiona - PROPRIEDADE</b>: Um TECNICO supervisiona uma ou várias PROPRIEDADE, e uma
  PROPRIEDADE é supervisionada por apenas um TECNICO. <br/>Cardinalidade: (1,n)</li>
</ul>

## 7. Referências

> [1] ABRAHAM, SILBERSCHATZ,. Sistema de Banco de Dados. Grupo GEN, 2020. 9788595157552. Disponível em: <a href="https://integrada.minhabiblioteca.com.br/#/books/9788595157552/" target="_blanck"> https://integrada.minhabiblioteca.com.br/#/books/9788595157552/</a>. Acesso em: 13 fev. 2022.

> [2] RODRIGUES, Joel. **MER e DER: Modelagem de Bancos de Dados**. DEVMEDIA. Disponível em: <a href="https://www.devmedia.com.br/mer-e-der-modelagem-de-bancos-de-dados/14332" target="_blanck">https://www.devmedia.com.br/mer-e-der-modelagem-de-bancos-de-dados/14332</a>. Acesso em: 18/02/2022.
