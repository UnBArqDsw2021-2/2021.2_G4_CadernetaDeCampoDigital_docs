<style> #dict th, #dict td { vertical-align: middle; text-align: center; border: 0.5px solid rgba(0,0,0,0.2); } </style>

# Dicionário de Dados

## 1. Versionamento

| Versão | Data       | Descrição               | Autor(es)    |
| ------ | ---------- | ----------------------- | ------------ |
| 1.0    | 17/02/2022 | Abertura do documento   | Thiago       |
| 1.1    | 17/02/2022 | Adição do dicionário geral | Thiago    |
| 1.2    | 17/02/2022 | Adição do dicionário individual | Eduardo e Thiago |
| 1.3    | 18/02/2022 | Adição da introdução | Thiago |
| 1.4    | 20/02/2022 | Renomeando casa para numero | Thiago |
| 1.4    | 20/02/2022 | Revisão por pares | Brenno e Vitor Lamego |

## 2. Introdução

<p align="justify" style="text-indent: 20px">O Dicionário de Dados é composto de um conjunto de relações, idênticas em propriedades às relações utilizadas para armazenar dados, e é utilizado para armazenar informações dos objetos e como um repositório de metadados [1]. Dessa forma, este documento especifica, de forma concisa e clara, as entidades, atributos e relacionamentos implementadas e validadas no Modelo Entidade-Relacionamento (<a href="../mer">MER</a>), Diagrama Entidade-Relacionamento (<a href="../der">DER</a>) e Diagrama Lógico de Dados (<a href="../dld">DLD</a>).
</p>

<p align="justify" style="text-indent: 20px">O Dicionário de Dados de cada relação é composto pelos seguintes tipos de informações:</p>
- Definição dos atributos
- Tipo do dado
- Tamanho em bytes
- Restrições de Integridades, por exemplo, chave primária, chave estrangeira, obrigatório, único e optativo
- Descrição do atributo


## 3. Dicionário de Dados

### 3.1 Descrição Geral das Entidades

<table id="dict">
  <tr>
    <th>Entidade</th>
    <th>Relacionamento</th>
    <th>Nome do Relacionamento</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>USUARIO</td>
    <td></td>
    <td></td>
    <td>Cadastro dos dados pessoais dos usuários.</td>
  </tr>
  <tr>
    <td>PRODUTOR</td>
    <td>PROPRIEDADE</td>
    <td>detem</td>
    <td>Cadastro dos dados pessoais de cada produtor</td>
  </tr>
  <tr>
    <td>TECNICO</td>
    <td>PROPRIEDADE</td>
    <td>supervisiona</td>
    <td>Cadastro dos dados dos técnicos.</td>
  </tr>
  <tr>
    <td>CADERNETA_DE_CAMPO</td>
    <td>PLANTIO</td>
    <td>registra</td>
    <td>Cadastro da caderneta de campo que o produtor faz do plantio</td>
  </tr>
  <tr>
    <td rowspan="4">PLANTIO</td>
    <td>CADERNETA_DE_CAMPO</td>
    <td>registra</td>
    <td rowspan="4">Cadastro de uma plantação da propriedade</td>
    <tr>
      <td>CULTURA</td>
      <td>possui</td>
    </tr>
    <tr>
    <td>AGROTOXICO</td>
      <td>contem</td>
    </tr>
    <tr>
      <td>PROPRIEDADE</td>
      <td>pertence</td>
    </tr>
  </tr>
  <tr>
    <td rowspan="3">PROPRIEDADE </td>
    <td>PLANTIO</td>
    <td>pertence</td>
    <td rowspan="3">Cadastro de cada propriedade</td>
    <tr>
      <td>PRODUTOR</td>
      <td>detem</td>
    </tr>
    <tr>
      <td>TECNICO</td>
      <td>supervisiona</td>
    </tr>
  </tr>
  <tr>
    <td rowspan="2">CULTURA</td>
    <td>PLANTIO</td>
    <td>possui</td>
    <td rowspan="2">Cadastro do alimento que está sendo plantado em cada plantio</td>
    <tr>
      <td>AGROTOXICO</td>
      <td>espera</td>
    </tr>
  </tr>
  <tr>
    <td rowspan="3">AGROTOXICO</td>
    <td>PLANTIO</td>
    <td>contem</td>
    <td rowspan="3">Cadastro dos agrotóxicos utilizados nos plantios</td>
    <tr>
      <td>CULTURA</td>
      <td>aplica</td>
      </tr>
    <tr>
      <td>TIPO_AGROTOXICO</td>
      <td>tem</td>
    </tr>
  </tr>
  <tr>
    <td>TIPO_AGROTOXICO</td>
    <td>AGROTOXICO</td>
    <td>tem</td>
    <td>Cadastro dos tipos de agrotóxicos utilizados</td>
  </tr>
</table>
<h6 align = "center">Tabela 1: Descrição Geral das Entidades.</h6>
<h6 align = "center">Fonte: Autores</h6>

### 3.2 Descrição Individual das Entidades

<table id="dict">
  <tr>
    <th colspan="6">USUARIO</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idUsuario</td>
    <td>UUID</td>
    <td>7</td>
    <td>chave primária e obrigatório</td>
    <td>Identificador único do usuário</td>
  </tr>
  <tr>
    <td>cpf</td>
    <td>VARCHAR</td>
    <td>11</td>
    <td>obrigatório e único</td>
    <td>Número do CPF do usuário</td>
  </tr>
  <tr>
    <td>nome</td>
    <td>VARCHAR</td>
    <td>80</td>
    <td>obrigatório</td>
    <td>Nome do usuário</td>
  </tr>
  <tr>
    <td>dataNascimento</td>
    <td>DATE</td>
    <td>4</td>
    <td>obrigatório</td>
    <td>Data de nascimento do usuário</td>
  </tr>
  <tr>
    <td>senha</td>
    <td>VARCHAR</td>
    <td>255</td>
    <td>obrigatório</td>
    <td>Hash da senha do usuário</td>
  </tr>
  <tr>
    <td>telefone</td>
    <td>VARCHAR</td>
    <td>12</td>
    <td>obrigatório</td>
    <td>Número do telefone do usuário</td>
  </tr>
</table>
<h6 align = "center">Tabela 2: Descrição Individual do USUARIO.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">PRODUTOR</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idUsuario</td>
    <td>UUID</td>
    <td>7</td>
    <td>chave primária, chave estrangeira e obrigatório</td>
    <td>Identificação do usuário</td>
  </tr>
  <tr>
    <td>dap</td>
    <td>VARCHAR</td>
    <td>11</td>
    <td>único e obrigatório</td>
    <td>Declaração de Aptidão ao Pronaf (DAP) do produtor</td>
  </tr>
</table>
<h6 align = "center">Tabela 3: Descrição Individual do PRODUTOR.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">TECNICO</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idUsuario</td>
    <td>UUID</td>
    <td>7</td>
    <td>chave primária, chave estrangeira e obrigatório</td>
    <td>Identificação do usuário</td>
  </tr>
  <tr>
    <td>crea</td>
    <td>VARCHAR</td>
    <td>10</td>
    <td>obrigatório e único</td>
    <td>Número do CREA do técnico</td>
  </tr>
  <tr>
    <td>formacao</td>
    <td>VARCHAR</td>
    <td>80</td>
    <td>obrigatório</td>
    <td>Formação do técnico</td>
  </tr>
  <tr>
    <td>email</td>
    <td>VARCHAR</td>
    <td>120</td>
    <td>obrigatório</td>
    <td>E-mail do técnico</td>
  </tr>
  <tr>
    <td>emailVerificado</td>
    <td>BOOLEAN</td>
    <td>1</td>
    <td>obrigatório</td>
    <td>Verificar se o e-mail do técnico foi confirmado</td>
  </tr>
</table>
<h6 align = "center">Tabela 4: Descrição Individual do TECNICO.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">PROPRIEDADE</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idPropriedade</td>
    <td>INT</td>
    <td>4</td>
    <td>chave primária e obrigatório</td>
    <td>Identificação da propriedade</td>
  </tr>
  <tr>
    <td>cep</td>
    <td>VARCHAR</td>
    <td>8</td>
    <td>obrigatório</td>
    <td>Número do CEP da propriedade</td>
  </tr>
  <tr>
    <td>estado</td>
    <td>VARCHAR</td>
    <td>2</td>
    <td>obrigatório</td>
    <td>Sigla da unidade federativa em que a propriedade se encontra</td>
  </tr>
  <tr>
    <td>cidade</td>
    <td>VARCHAR</td>
    <td>40</td>
    <td>obrigatório</td>
    <td>Nome da cidade em que a propriedade se encontra</td>
  </tr>
  <tr>
    <td>bairro</td>
    <td>VARCHAR</td>
    <td>40</td>
    <td>obrigatório</td>
    <td>Nome do bairro em que a propriedade se encontra</td>
  </tr>
  <tr>
    <td>logradouro</td>
    <td>VARCHAR</td>
    <td>80</td>
    <td>obrigatório</td>
    <td>Endereço da propriedade</td>
  </tr>
  <tr>
    <td>numero</td>
    <td>INT</td>
    <td>4</td>
    <td>obrigatório</td>
    <td>Número da propriedade</td>
  </tr>
  <tr>
    <td>complemento</td>
    <td>VARCHAR</td>
    <td>80</td>
    <td>optativo</td>
    <td>Descrição complementar ao endereço</td>
  </tr>
  <tr>
    <td>hectares</td>
    <td>DECIMAL</td>
    <td>6 casas inteiras mais 2 casas decimais</td>
    <td>optativo</td>
    <td>Número de hectares da propriedade</td>
  </tr>
  <tr>
    <td>idProdutor</td>
    <td>UUID</td>
    <td>7</td>
    <td>chave estrangeira e obrigatório</td>
    <td>Identificador do produtor que detem a propriedade</td>
  </tr>
  <tr>
    <td>idTecnico</td>
    <td>UUID</td>
    <td>7</td>
    <td>chave estrangeira e obrigatório</td>
    <td>Identificador do técnico que supervisiona a propriedade</td>
  </tr>
</table>
<h6 align = "center">Tabela 5: Descrição Individual do PROPRIEDADE.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">PLANTIO</th>
  <tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idPlantio</td>
    <td>INT</td>
    <td>4</td>
    <td>chave primária e obrigatório</td>
    <td>Identificação do plantio</td>
  <tr>
  </tr>
    <td>dataPlantio</td>
    <td>DATE</td>
    <td>4</td>
    <td>obrigatório</td>
    <td>Data em que o produtor plantou a cultura</td>
  </tr>
  <tr>
    <td>numeroTalhao</td>
    <td>INT</td>
    <td>4</td>
    <td>obrigatório</td>
    <td>Número do talhão que o produtor plantou</td>
  </tr>
  <tr>
    <td>idCultura</td>
    <td>INT</td>
    <td>4</td>
    <td>chave estrangeira e obrigatório</td>
    <td>Identificação da cultura que foi plantada</td>
  </tr>
  <tr>
    <td>idPropriedade</td>
    <td>INT</td>
    <td>4</td>
    <td>chave estrangeira e obrigatório</td>
    <td>Identificação da propriedade</td>
  </tr>
  <tr>
    <td>estado</td>
    <td>CHAR</td>
    <td>1</td>
    <td>obrigatório</td>
    <td>Estado atual do plantio. Podendo ser Plantado, PeriodoDeCarencia, Colheita, Finalizado e etc</td>
  </tr>
</table>
<h6 align = "center">Tabela 6: Descrição Individual do PLANTIO.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">CADERNETA_DE_CAMPO</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>numeroSerie</td>
    <td>VARCHAR</td>
    <td>11</td>
    <td>chave primária e obrigatório</td>
    <td>Número de identificação da caderneta do produtor</td>
  </tr>
  <tr>
    <td>dataColheita</td>
    <td>DATE</td>
    <td>4</td>
    <td>único e obrigatório</td>
    <td>Data em que o produtor colheu o plantio</td>
  </tr>
  <tr>
    <td>idPlantio</td>
    <td>INT</td>
    <td>4</td>
    <td>chave estrangeira, único e obrigatório</td>
    <td>Identificação do plantio</td>
  </tr>
</table>
<h6 align = "center">Tabela 7: Descrição Individual do CADERNETA_DE_CAMPO.</h6>
<h6 align = "center">Fonte: Autores</h6>



<table id="dict">
  <tr>
    <th colspan="6">CULTURA</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idCultura</td>
    <td>INT</td>
    <td>4</td>
    <td>chave primária e obrigatório</td>
    <td>Número de identificação da cultura</td>
  </tr>
  <tr>
    <td>nome</td>
    <td>VARCHAR</td>
    <td>30</td>
    <td>obrigatório</td>
    <td>Nome da cultura</td>
  </tr>
</table>
<h6 align = "center">Tabela 8: Descrição Individual do CULTURA.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">AGROTOXICO</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idAgrotoxico</td>
    <td>INT</td>
    <td>4</td>
    <td>chave primária e obrigatório</td>
    <td>Número de identificação do agrotóxico</td>
  </tr>
  <tr>
    <td>nome</td>
    <td>VARCHAR</td>
    <td>40</td>
    <td>obrigatório</td>
    <td>Nome do agrotóxico</td>
  </tr>
  <tr>
    <td>idTipoAgrotoxico</td>
    <td>INT</td>
    <td>4</td>
    <td>chave estrangeira e obrigatório</td>
    <td>Número de identificação do tipo do agrotóxico</td>
  </tr>
</table>
<h6 align = "center">Tabela 9: Descrição Individual do AGROTOXICO.</h6>
<h6 align = "center">Fonte: Autores</h6>

<table id="dict">
  <tr>
    <th colspan="6">TIPO_AGROTOXICO</th>
  </tr>
  <tr>
    <th>Atributo</th>
    <th>Tipo de Dados</th>
    <th>Tamanho (bytes)</th>
    <th>Restrições</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>idTipoAgrotoxico</td>
    <td>INT</td>
    <td>4</td>
    <td>chave primária e obrigatório</td>
    <td>Número de identificação do tipo do agrotóxico</td>
  </tr>
  <tr>
    <td>nome</td>
    <td>VARCHAR</td>
    <td>80</td>
    <td>único e obrigatório</td>
    <td>Nome do tipo do agrotóxico</td>
  </tr>
</table>
<h6 align = "center">Tabela 10: Descrição Individual do TIPO_AGROTOXICO.</h6>
<h6 align = "center">Fonte: Autores</h6>

## 4. Referências

> [1] BITTENCOURT, Rogério Gonçalves. Modelo Relacional: Dicionário de Dados. In: ASPECTOS Básicos de Bancos de Dados. Florianópolis: UNESP, 2004. p. 30-32. Disponível em: <a href="https://www.marilia.unesp.br/Home/Instituicao/Docentes/EdbertoFerneda/BD%20-%20Aspectos%20Basicos.pdf" target="_blanck">https://www.marilia.unesp.br/Home/Instituicao/Docentes/EdbertoFerneda/BD%20-%20Aspectos%20Basicos.pdf</a>. Acesso em: 18 fev. 2022.
