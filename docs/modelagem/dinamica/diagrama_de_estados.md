# Diagrama de Estados

## 1. Versionamento

| Versão | Data       | Descrição                         | Autor(es)                   |
| ------ | ---------- | --------------------------------- | --------------------------- |
| 1.0    | 17/02/2022 | Criação do documento e introdução | Carlos Eduardo e Vitor Lamego |
| 1.1    | 17/02/2022 | Adição dos diagramas 3.2, 3.3 e 3.4 | Vitor Lamego |
<!-- | 1.2    | XX/02/2022 | Adição dos diagramas 3.1 e 3.5 | Carlos Eduardo | -->
<!-- | 1.3   | XX/02/2022 | Revisão por pares | Nome 1 e Nome 2 -->


## 2. Introdução

<p align="justify" style="text-indent: 20px">O diagrama de estados é bastante utilizado dentro da área de software, sendo também componente da modelagem dinâmica. O seu objetivo é demonstrar os diferentes estados que um objeto pode ter dentro da aplicação e o diagrama é responsável por explicitar justamente qual é o estado inicial de determinado objeto, os estados pelos quais ele pode passar, a transição, responsável pela mudança de estado, e o estado final.[1]</p>

<p align="justify" style="text-indent: 20px">Os diagramas sempre iniciam com um círculo escuro, sendo este o estado incial, passam por meio das setas, que representam as transições, para um novo estado até que chegue ao estado final que é representado por um círculo contornado. Apesar disso, o intuito principal não é a demonstração da progressão dos processos, mas os tipos específicos de comportamento que podemos encontrar em cada ocasião.[2]</p>


## 3. Diagramas de Estados

<p align="justify" style="text-indent: 20px">Na ocasião do projeto, a metodologia de desenvolvimento dos diagramas de estado consistiu, basicamente, em definir quais são os processos chaves da aplicação e a partir disso discutir e desenvolver os estados que podemos encontrar do app dentro desses processos. Foram encontrados cinco principais projetos, sendo eles: <b>Entrar no app</b>, <b>Cadastrar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a></b>, <b>Cadastrar <a href="/requisitos/modelagem/lexicos#plantio">plantio</a></b>, <b>Acompanhar <a href="/requisitos/modelagem/lexicos#plantio">plantio</a></b> e <b>Acompanhar <a href="/requisitos/modelagem/lexicos#produtor">produtor</a></b>. A seguir será explicado cada diagrama realizado assim como a apresentação da sua imagem.</p>


### 3.1 Entrar no app

<!-- <img src="../../../assets/modelagem/dinamica/diagrama_estados/arquivo.svg" class="zoom"> 
<h6 align = "center">Figura 1: Diagrama de Estados - Entrar no app</h6>
<h6 align = "center">Fonte: Autores</h6> -->

### 3.2 Cadastrar propriedade

<p align="justify" style="text-indent: 20px">Para o diagrama de cadastro de <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>, foi identificado que primeiramente o app mostra todas as <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> já cadastradas. A partir desse estado, existe uma divisão de fluxo em que o <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> pode escolher entre criar um novo registro, ou editar as informações já existentes. Em ambos os casos o aplicativo mostra as informações disponíveis para cada ocasião específica e depois as novas informações são enviadas ao servidor, chegando ao estado final do processo. Veja o diagrama referente a esse processo a seguir:</p>

<img src="../../../assets/modelagem/dinamica/diagrama_estados/cadastrar_propriedade.svg" class="zoom">
<h6 align = "center">Figura 2: Diagrama de Estados - Cadastrar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a></h6>
<h6 align = "center">Fonte: Autores</h6>

### 3.3 Cadastrar plantio

<p align="justify" style="text-indent: 20px">No processo de cadastrar um <a href="/requisitos/modelagem/lexicos#plantio">plantio</a>, foi identificado que inialmente o aplicativo estará mostrando todos os <a href="/requisitos/modelagem/lexicos#talhoes">talhões</a> de uma determinada <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>. Após esse estado existe uma divisão de fluxo onde o <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> pode entrar no fluxo de edição das informações de um determinado <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> ou então no fluxo de cadastro de um novo plantio, bem parecido com o fluxo de cadastro visto no processo anterior. Os dois fluxos se encontram futuramente no estado em que o aplicativo envia as novas informações para o servidor e então chegam ao estado final. Veja o diagrama referente a esse processo a seguir: </p>

<img src="../../../assets/modelagem/dinamica/diagrama_estados/cadastrar_plantio.svg" class="zoom">
</center>
<h6 align = "center">Figura 3: Diagrama de Estados - Cadastrar <a href="/requisitos/modelagem/lexicos#plantio">plantio</a></h6>
<h6 align = "center">Fonte: Autores</h6>

### 3.4 Acompanhar plantio

<p align="justify" style="text-indent: 20px">O acompanhamento de <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> é um processo um pouco mais complexo, uma vez que engloba as principais funcionalidade do aplicativo. O processo, de maneira resumida, inicia-se com um estado inicial onde é mostrado todos os <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> cadastrados. A partir desse estado existe uma divisão de fluxo em que o usuário pode visualizar o histórico de um <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> já colhido ou visualizar as informações de um <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> que ainda não foi colhido. Para a primeira ocasião ele verifica as informações com detalhes e logo em seguida já encontra o estado final do aplicativo. Para a segunda ocasião, se o <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> for um <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> ele passa pelos estados referentes à avaliação de pendências enviadas pelo <a href="/requisitos/modelagem/lexicos#produtor">produtor</a>, se o <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> não for um <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> então ele passa pelos estados de cadastro de <a href="/requisitos/modelagem/lexicos#agrotoxicos">agrotóxicos</a>. Futuramente os dois fluxos se encontram na visualização dos detalhes e informações de um determinado <a href="/requisitos/modelagem/lexicos#plantio">plantio</a>. Essa descrição está bastante resumida devido à complexidade deste diagrama, portanto verifique a imagem a seguir: </p>

<img src="../../../assets/modelagem/dinamica/diagrama_estados/acompanhar_plantio.svg" class="zoom">
</center>
<h6 align = "center">Figura 3: Diagrama de Estados - Acompanhar <a href="/requisitos/modelagem/lexicos#plantio">plantio</a></h6>
<h6 align = "center">Fonte: Autores</h6>

### 3.5 Acompanhar produtor

<!-- <center>
<img src="../../../assets/modelagem/dinamica/atividade_tecnico.svg" class="zoom">
</center>
<h6 align = "center">Figura 3: Diagrama de Estados - Acompanhar produtor</h6>
<h6 align = "center">Fonte: Autores</h6> -->


## 4. Referências

> [1] SERRANO, Milene. 06c - VídeoAula - DSW - Modelagem - Diagrama de Atividades. Material apresentado para a disciplina de Arquitetura e Desenho de Software no curso de Engenharia de Software da Universidade de Brasília, FGA.

> [2] O que é um diagrama de máquina de estados?. Lucidchart. Disponível em: <a href="https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml">Lucidchart - Diagrama de Estados</a>. Acesso em: 17 de fevereiro de 2022.



