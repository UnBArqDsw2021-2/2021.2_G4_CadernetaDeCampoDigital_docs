# Padrões de Projetos Emergentes

## 1. Versionamento

| Versão | Data       | Descrição                                             | Autor(es)                     |
| ------ | ---------- | ----------------------------------------------------- | ----------------------------- |
| 1.0    | 24/02/2022 | Criação do documento e introdução                     | Vitor Lamego |
| 1.1    | 24/02/2022 | Adição dos Padrões Emergentes                     | Vitor Lamego |
| 1.2    | 24/02/2022 | Adição dos Padrões Rest e MVT                     | Denniel William |
| 1.3    | 27/02/2022 | Remoção dos tópicos tratados no GOFs              | Denniel William |
| 1.4    | 27/02/2022 | Adição das imagens e explicação sobre REST        | Denniel William |



## 2. Introdução

<p align="justify" style="text-indent: 20px">Padrões de projeto são formatos de soluções que são utilizadas de forma recorrente dentro do projeto. Esses padrões são comumente utilizados em projetos com o paradigma Orientado a Objeto, tranformando esses padrões em artifícios de comunicação e solução dentro das equipes.[1]</p>

<p align="justify" style="text-indent: 20px">Os padrões nomeados como emergentes são derivados da necessidade de algum fator específico para utilizar determinada solução. Portanto, os padrões emergentes são definidos quando possuímos um determinado comportamento inerente ao padrão, contudo não possuimos a estrutura que o descreve, o que é muito comum em situações como: falta de conhecimento por parte do desenvolvedor sobre os padrões de projetos, sucessivas mudanças em outras classes que então são refletidos em uma determinada parte do código, falta de refatoração, característica do problema.[1]</p>


## 3. Exemplos de Padrões Emergentes

### 3.1 Injeção de Dependência

<p align="justify" style="text-indent: 20px">Injeção de dependência é um padrão utilizado para dimimuir o acoplamento de determinada parte do código, que costuma acontecer quando uma classe depende da instância de uma outra classe para a sua criação. Dessa forma a interface é a responsável por injetar em cada classe as suas dependências declaradas. Nesta ocasião a injeção de dependência se relaciona com o padrão de "Inversão de controle", mas não pode ser considerado como um sinônimo, ou seja, a responsabilidade de informar a implementação utilizada deixa de ser da classe e passa a ser de quem está consumindo a classe.[2]</p>

<p align="justify" style="text-indent: 20px">O baixo acoplamento é importante para facilitar a manutenibilidade do código, além de permitir a utilização de mocks para realizar testes unitários nas respecivas classes. E assim, como explicado sobre a injeção de dependência, esse aumento entre a independência dos módulos colabora para o baixo acoplamento do projeto.</p>

### 3.2 Rest

<p align="justify" style="text-indent: 20px">O padrão REST, Representational State Transfer (Transferência de Estado Representacional), define a padronização de rotas, requisições e comunicações sem estado, também conhecido como protocolo HTTP. Sendo assim, uma API que utiliza essa padronização e que possui inteligência para aplicá-la é denominada de RESTful. [3]</p>

<p align="justify" style="text-indent: 20px">Existem 4 princípios principais do REST: [5]</p>

- **Client-Server (Cliente-Servidor):** Sempre há um cliente e um servidor e esses dois sistemas precisam de limites para o funcionamento.[5]
- **Stateless (Sem estado):** Os servidores precisam ser capazes de processar as mensagens que recebem. Para fazer isso, cada solicitação que um servidor receber deve ter as informações necessárias para que o servidor funcione.[5]
- **Uniform Interface (Interface Uniforme):** O uso de terminologia e recursos semelhantes ajuda a padronizar as APIs. De acordo com o princípio, os seguintes verbos HTTP são usados: GET, PUT, POST,DELETE. Os recursos sempre se referem a URIs (identificador uniforme de recursos). As respostas HTTP sempre vêm com um status e um corpo.[5]
- **Cacheable (Armazenável com cache):** Os clientes precisam ser capazes de armazenar em cache as representações. Devido à ausência de estado (toda representação sendo autodescritiva), isso é possível em uma API RESTful.[5]

<img src="../../../assets/padroes_projeto/rest.png" width="800"/>
<h6 align = "center">Figura 1: API REST Model</h6>
<h6 align = "center">Fonte: https://www.astera.com/pt/tipo/blog/definição-de-api/</h6>


### 3.3 Padrão MVT (Model - View - Template)

<p align="justify" style="text-indent: 20px">Um dos padrões também que serão seguidos, será o MVT, em decorrência da utilização do framework Django, definido pela equipe para o back-end.</p>
<p align="justify" style="text-indent: 20px">O padrão MVT se baseia na distribuição de Model, View e Template: A model atua como a interface de dados, ela é a estrutura lógica por trás do aplicativo e é representado pelo banco de dados do projeto; A view é usada para executar as regras de negócios, interação com o modelo para transporte de dados e renderização do template; O template é a camada de apresentação, e é responsável pela parte da interface do usuário.[4]</p>

<img src="../../../assets/padroes_projeto/mvt.png" width="800"/>
<h6 align = "center">Figura 2: Padrão MVT</h6>
<h6 align = "center">Fonte: https://www.treinaweb.com.br/blog/entendendo-o-mtv-do-django</h6>

## 4. Referências

> [1] JOB, Ricardo de Sousa. Uma abordagem para detecção de padrões emergentes. 2014. 92f. (Dissertação de Mestrado em Ciência da Computação) Programa de Pós-graduação em Ciência da Computação, Centro de Engenharia Elétrica e Informática, Universidade Federal de Campina Grande - Paraiba - Brasil, 2014.

> [2] **Injeção de Dependência**. O que é injeção de dependência ? Disponível em: <a href="https://medium.com/@eduardolanfredi/inje%C3%A7%C3%A3o-de-depend%C3%AAncia-ff0372a1672" >Injeção de Dependência</a>. Acesso em: 24 de fev. de 2022.

> [3] **Design de API Rest**. Design de API Rest. Disponível em: <a href="https://wssilva-willian.medium.com/design-de-api-rest-9807a5b16c9f" >Design de API Rest</a>. Acesso em: 25 de fev. de 2022.

> [4] **Django MVT**. Django MVT. Disponível em: <a href="https://www.javatpoint.com/django-mvt" >Django MVT</a>. Acesso em: 25 de fev. de 2022.

> [5] **What Is the Difference Between REST and RESTful APIs?**. What Is the Difference Between REST and RESTful APIs?. Disponível em: <a href="https://blog.devmountain.com/what-is-the-difference-between-rest-and-restful-apis" >Django MVT</a>. Acesso em: 27 de fev. de 2022.