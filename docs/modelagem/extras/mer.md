# Modelo Entidade-Relacionamento

## 1. Versionamento

| Versão | Data       | Descrição               | Autor(es)    |
| ------ | ---------- | ----------------------- | ------------ |
| 1.0    | 13/02/2022 | Abertura do documento   | Thiago       |
| 1.1    | 13/02/2022 | Introdução do documento | Rafael Ramos |

## 2. Introdução

<p align="justify" style="text-indent: 20px">O Modelo de Entidade-Relacionamento (ME-R) foi elaborado para facilitar o projeto de um Banco de Dados, por meio da especificação de um esquema de negócio que representa a estrutura lógica geral de um banco de dados (SILBERSCHATZ) [1]. É constituído por um conjunto de objetos básicos que são as Entidades, seus relacionamentos e atributos, baseia-se na percepção abstrata do mundo real e corresponde a uma visão lógica de alto nível dos dados. </p>

## 3. Entidades

- [USUARIO](../../../requisitos/modelagem/lexicos#usuario)
- [PRODUTOR](../../../requisitos/modelagem/lexicos#produtor)
- [TECNICO](../../../requisitos/modelagem/lexicos#tecnico)
- [PROPRIEDADE](../../../requisitos/modelagem/lexicos#propriedade)
- [PLANTIO](../../../requisitos/modelagem/lexicos#plantio)
- [CADERNETA_DE_CAMPO](../../../requisitos/modelagem/lexicos#cardeneta_de_campo)
- [CULTURA](../../../requisitos/modelagem/lexicos#cultura)
- [AGROTOXICO](../../../requisitos/modelagem/lexicos#agrotoxico)
- [TIPO_AGROTOXICO](../../../requisitos/modelagem/lexicos#tipo_agrotoxico)

## 4. Descrição das Entidades

- USUARIO ( <span style="text-decoration: underline;">idUsuario</span>, cpf, nome, telefone, dataNascimento, senha, telefone )
- PRODUTOR ( <span style="text-decoration: underline;">idUsuario</span>, dap )
- TECNICO ( <span style="text-decoration: underline;">idUsuario</span>, crea, formacao, email, emailVerificado )
- PROPRIEDADE ( <span style="text-decoration: underline;">idPropriedade</span>, idProdutor, idTecnico, endereco(cep, cidade, bairro, logradouro, numero, complemento), hectares )
- PLANTIO ( <span style="text-decoration: underline;">idPlantio</span>, numeroTalhao, idPropriedade, dataPlantio, idCultura )
- CADERNETA_DE_CAMPO ( <span style="text-decoration: underline;">numeroSerie</span>, dataColheita, idPlantio )
- CULTURA ( <span style="text-decoration: underline;">idCultura</span>, nome )
- AGROTOXICO ( <span style="text-decoration: underline;">idAgrotoxico</span>, nome, idTipoAgrotoxico )
- TIPO_AGROTOXICO ( <span style="text-decoration: underline;">idTipoAgrotoxico</span>, nome )

## 5. Relacionamentos

- <b>PLANTIO - registra - CADERNETA_DE_CAMPO</b> 1. Um PLANTIO registra apenas uma ou várias CADERNETA_DE_CAMPO, e
  uma CADERNETA_DE_CAMPO é registrada por apenas um PLANTIO 2. Cardinalidade: (1,n)

- <b>PLANTIO - possui - CULTURA</b> 1. Um PLANTIO possui apenas uma CULTURA, e uma CULTURA pode ser
  possuída por um ou vários PLANTIO 2. Cardinalidade: (n,1)

- <b>PLANTIO - pertence - PROPRIEDADE</b> 1. Um PLANTIO pertence a uma PROPRIEDADE e uma PROPRIEDADE
  possui um ou mais PLANTIO 2. Cardinalidade: (n,1)

- <b>PRODUTOR - detem - PROPRIEDADE</b> 1. Um PRODUTOR detém uma ou mais PROPRIEDADE, e uma
  PROPRIEDADE pertence a apenas um PRODUTOR. 2. Cardinalidade: (1,n)

- <b>PLANTIO - contem - AGROTOXICO</b> 1. Um PLANTIO pode conter nenhum ou vários AGROTOXICO, e um
  AGROTOXICO pode estar em um ou vários PLANTIO. 2. Cardinalidade: (n,m)

- <b>AGROTOXICO - tem - TIPO_AGROTOXICO</b> 1. Um AGROTOXICO tem um TIPO_AGROTOXICO, e um
  TIPO_AGROTOXICO pode ser de um ou vários AGROTOXICO. 2. Cardinalidade: (n,1)

- <b>CULTURA - espera - AGROTOXICO</b> 1. Uma CULTURA espera por um ou vários AGROTOXICO, e um
  AGROTOXICO pode ser aplicado em uma ou várias CULTURA. 2. Cardinalidade: (n,m)

- <b>TECNICO - supervisiona - PROPRIEDADE</b> 1. Um TECNICO supervisiona uma ou várias PROPRIEDADE, e uma
  PROPRIEDADE é supervisionada por apenas um TECNICO. 2. Cardinalidade: (1,n)

## 6. Referências

> [1] ABRAHAM, SILBERSCHATZ,. Sistema de Banco de Dados. Grupo GEN, 2020. 9788595157552. Disponível em: <a href="https://integrada.minhabiblioteca.com.br/#/books/9788595157552/" target="_blanck"> https://integrada.minhabiblioteca.com.br/#/books/9788595157552/</a>. Acesso em: 13 fev. 2022.
