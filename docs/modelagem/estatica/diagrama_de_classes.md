# Diagrama de Classes

## 1. Versionamento

| Versão | Data       | Descrição                         | Autor(es)                          |
| ------ | ---------- | --------------------------------- | ---------------------------------- |
| 1.0    | 10/02/2022 | Criação do documento e introdução | Rafael Ramos                       |
| 1.1    | 10/02/2022 | Adição do Diagrama de Classe      | Rafael Ramos e Thiago              |
| 1.1.1  | 13/02/2022 | Revisão por pares                 | João Pedro Moura e Denniel William |
| 1.1.2  | 20/02/2022 | Adição do tópico de metodologia   | Rafael Ramos e João Pedro          |
| 1.2    | 05/03/2022 | Adição da classe talhão           | Thiago     |
| 1.2.1 | 07/03/2022 | Revisão por pares                 | João Pedro Moura e Denniel William |

## 2. Introdução

<p align="justify" style="text-indent: 20px">Diagramas de classes fazem parte de um dos seis tipos de diagramas estruturais em UML (Unified Modeling Language), tem por objetivo modelar a estrutura estática de um sistema que representa suas classes, atributos, operações e as relações entre os objetos. Os diagramas de classes podem ajudar no entendimento dos requisitos do domínio do problema e na identificação de seus componentes, também podem ser traduzidos em classes e objetos reais no software em um projeto orientado a objetos. Portanto os diagramas de classes podem ser usados para visualizar, especificar e documentar recursos estruturais em seus modelos. (IBM) [1]</p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">Utilizando o software <a href="https://www.lucidchart.com/pages/">Lucidchart</a>, os integrantes Rafael Ramos e Thiago realizaram a confecção do diagrama enquanto alinhavam as ideias em uma chamada simultânea utilizando o <a href="https://discord.com/app">Discord</a>. Foi utilizado o <a href="../../agil/product_backlog">Product Backlog</a> já confeccionado pela equipe para a modelagem das classes e relacionamentos do diagrama visando cumprir com os requisitos do domínio do problema.</p>

## 4. Diagrama de classes

### Versão 2.0

<img src="../../../assets/modelagem/estatica/diagramaClasseV2.svg" class="zoom"/>
<h6 align = "center">Figura 1: Diagrama de Classes Versão 2.0.</h6>
<h6 align = "center">Fonte: Autores</h6>
#### Observações
- Todos os atributos públicos possuem métodos Getters e Setters, não foram incluídos no diagrama para facilitar a visualização.
- A nomenclatura dos atributos foi em Snake case para facilitar a futura implementação com a linguagem utilizada no back-end (Python).

### Versão 1.0

<img src="../../../assets/modelagem/diagrama_classes.svg" class="zoom"/>
<h6 align = "center">Figura 2: Diagrama de Classes versão 1.0</h6>
<h6 align = "center">Fonte: Autores</h6>
#### Observações
- Todos os atributos públicos possuem métodos Getters e Setters, não foram incluídos no diagama para facilitar a visualização.
- A nomenclatura dos atributos foi em Snake case para facilitar a futura implementação com a linguagem utilizada no back-end (Python).

## 5. Referências

> [1] **Class diagrams**. Disponível em: <a href="https://www.ibm.com/docs/en/rsm/7.5.0?topic=structure-class-diagrams" target="_blanck">https://www.ibm.com/docs/en/rsm/7.5.0?topic=structure-class-diagrams</a>. Acesso em: 10 de fev. de 2022.
