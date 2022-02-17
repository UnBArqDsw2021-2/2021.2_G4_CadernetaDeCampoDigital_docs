# Dicionário de Dados

## 1. Versionamento

| Versão | Data       | Descrição               | Autor(es)    |
| ------ | ---------- | ----------------------- | ------------ |
| 1.0    | 17/02/2022 | Abertura do documento   | Thiago       |
| 1.1    | 17/02/2022 | Adição do dicionário geral | Thiago |

## 2. Introdução


## 3. Dicionário de Dados

### 3.1 Descrição Geral das Entidades

<style> #dict th, #dict td { vertical-align: middle; text-align: center; border: 0.5px solid rgba(0,0,0,0.2); } </style>

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
    <td rowspan="3">Cadastro de cada propriedade</td>>
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

## 6. Referências
