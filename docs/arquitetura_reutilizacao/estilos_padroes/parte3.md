# Estilos e Padrões Arquiteturais Parte 3

## 1. Versionamento

| Versão | Data       | Descrição                                   | Autor(es) |
| ------ | ---------- | ------------------------------------------- | --------- |
| 1.0    | 22/03/2022 | Abertura do documento                       | Brenno    |
| 1.1    | 22/03/2022 | Adição da Introdução, Metodologia e Estilos | Brenno    |

## 2. Introdução

<p align="justify" style="text-indent: 20px">Estilos e Padrões Arquiteturais definem uma organização estrutural a partir do conjunto pré-definido de subsistemas e responsabilidades com regras e diretrizes para esses subsistemas[1].</p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">Para a realização do documento, o membro do grupo responsável documentou as informações referentes aos estilos definidos na parte 3 do moodle da disciplina.</p>

## 4. Estilos

### 4.1. Pipes and Filters(Filtros e Dutos)

<p align="justify" style="text-indent: 20px">O Estilo Pipes and Filters apresenta aos fluxos uma organização para a passagem de dados, organizando a estrutura com os seguintes participantes:</p>

- **Filtro** **(*****Filter*****)**: Recebe, processa e recoloca dados no fluxo.
- **Duto** **(*****Pipe*****)**: Transfere dados e realiza buffer(dado temporário)
- **Fonte de dados** **(*****Data source*****)**: Fonte para os dados a serem utilizados
- **Coletor de dados** **(*****Data sink*****)**: Destino dos dados processados ao final

<p align="justify" style="text-indent: 20px">Dessa forma temos uma estrutura chamada tubulação de processamento, onde dutos fazem a ligação entre filtros, representada na figura 1. O estilo é útil para aplicações com pouca interação com usuários.</p>

<center>
<img src="../../../assets/estilos_padroes/pipes-and-filters.png" class="zoom"> 
<h6>Figura 1: Estrutura do Pipes and Filters</h6>
<h6>Fonte: Aula Estilos e Padrões Arquiteturais III - Profa. Milene [1]</h6>
</center>

**Vantagens**

- Decomposição de problemas 
- Reutilização de código a partir de componentes e interfaces bem definidas
- Pode ser sequencial ou concorrente[2]

**Desvantagens**

- Manutenção limitada caso um componente seja alterado frequentemente
- É possível que ocorram deadlocks por conta do uso de buffers

### 4.2. Repositório

<p align="justify" style="text-indent: 20px">As duas principais maneiras para a troca de dados entre subsistemas são: o compartilhamento de um banco de dados central que permite o acesso de outros subsistemas e bancos de dados próprios para o subsistema, sendo esses os responsáveis pela troca de dados entre si.</p>

<p align="justify" style="text-indent: 20px">O Estilo Repositório consiste nas primeira maneira apresentada, chamada de repositório compartilhado, sendo mais adequada para o compartilhamento de grandes quantidades de dados, dessa forma os subsistemas não interagem diretamente para acessar os dados.</p>

**Vantagens**

- Independência entre componentes
- Facilidade para gerenciamento dos dados por estarem centralizados

**Desvantagens**

- Problemas no repositório afeta todos
- Distribuição do repositório pode ser difícil
- Pode se tornar ineficiente de ser evoluída

## 5. Referências
> [1] SERRANO, Milene. Arquitetura e Desenho de Software. **Aula Estilos e Padrões Arquiteturais III**. Acesso em: 22 mar. 2022

> [2] SOMMERVILLE, Ian. Projeto de Arquitetura. **Engenharia de Software**. 10. ed. [S. l.]: Pearson Universidades, 2019. cap. 6, ISBN 8543024978.