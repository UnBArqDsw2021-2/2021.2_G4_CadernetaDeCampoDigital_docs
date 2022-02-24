# Padrões de Projetos Emergentes

## 1. Versionamento

| Versão | Data       | Descrição                                             | Autor(es)                     |
| ------ | ---------- | ----------------------------------------------------- | ----------------------------- |
| 1.0    | 24/02/2022 | Criação do documento e introdução                     | Vitor Lamego |
| 1.1    | 24/02/2022 | Adição dos Padrões Emergentes                     | Denniel e Vitor Lamego |



## 2. Introdução

<p align="justify" style="text-indent: 20px">Padrões de projeto são formatos de soluções que são utilizadas de forma recorrente dentro do projeto. Esses padrões são comumente utilizados em projetos com o paradigma Orientado a Objeto, sendo bastante, tranformando esses padrões em artifícios de comunicação e solução dentro das equipes.[1]</p>

<p align="justify" style="text-indent: 20px">Os padrões nomeados como emergentes são derivados da necessidade de algum fator específico para utilizar determinada solução. Portanto, os padrões emergentes são definidos quando possuímos um determinado comportamento inerente ao padrão, contudo não possui a estrutura que o descreve, o que é muito comum em situações como: falta de conhecimento por parte do desenvolvedor sobre os padrões de projetos, sucessivas mudanças em outras classes que então é refletida em uma determinada parte do código, falta de refatoração, característica do problema e, então, não necessita implementar o padrão.[1]</p>


## 3. Exemplos de Padrões Emergentes

### 3.1 Singleton

<p align="justify" style="text-indent: 20px">Existindo uma determinada classe A, se esta for um Singleton, em qualquer momento de execução essa classe pode ter apenas zero ou uma instância dessa classe. Portando todos os caminhos possíveis do programa, se necessário, devem utilizar essa única instância e não criar uma nova. É muito comum esse comportamento ser repetido por classes dentro de um projeot, mas não respeitando a sua estrutrua para ser considerada um padrão de projeto, nessas ocasiões o Singleton acaba sendo um padrão que emerge naquela parte específica do código.</p>

### 3.2 Injeção de Dependência

<p align="justify" style="text-indent: 20px">Injeção de dependência é um padrão utilizado para dimimuir o acoplamento de determinada parte do código, que costuma acontecer quando uma classe depende da instância de uma outra classe para a sua criação. Dessa forma a interface é a responsável por injetar em cada classe as suas dependências declaradas. Nesta ocasião a injeção de dependência se relaciona com o padrão de "Inversão de controle", mas não pode ser considerado como um sinônimo, ou seja, a responsabilidade de informar a implementação utilizada deixa de ser da classe e passa a ser de quem está consumindo a classe.[2]</p>

<p align="justify" style="text-indent: 20px">O baixo acoplamento é importante para facilitar a manutenibilidade do código, além de permitir a utilização de mocks para realizar testes unitários nas respecivas classes.</p>

### 3.3 Factory Method

<p align="justify" style="text-indent: 20px">O padrão de Factory Method é utilizado quando temos um método m que é responsável por retornar um objeto do tipo T, que podem, a qualquer momento, serem instanciadas apenas a partir do método m. Um exemplo claro de quando temos o Factory Method como um padrão emergente é quando não existem subclasses que permitam a escolha de como será implementado as instâncias desse objeto T.[1]</p>


## 4. Referências

> [1] JOB, Ricardo de Sousa. Uma abordagem para detecção de padrões emergentes. 2014. 92f. (Dissertação de Mestrado em Ciência da Computação) Programa de Pós-graduação em Ciência da Computação, Centro de Engenharia Elétrica e Informática, Universidade Federal de Campina Grande - Paraiba - Brasil, 2014.

> [2] **Injeção de Dependência**. O que é injeção de dependência ? Disponível em: <a href="https://medium.com/@eduardolanfredi/inje%C3%A7%C3%A3o-de-depend%C3%AAncia-ff0372a1672" >Injeção de Dependência</a>. Acesso em: 24 de fev. de 2022.


