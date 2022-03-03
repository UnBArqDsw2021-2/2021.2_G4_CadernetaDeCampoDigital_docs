# Aplicação de GRASP(s)

## 1. Versionamento
| Versão | Data       | Descrição                         | Autor(es)             |
| ------ | ---------- | --------------------------------- | --------------------- |
| 1.0    | 02/03/2022 | Criação do documento              | Paulo e Carlos        |
| 1.1    | 03/03/2022 | Adição da introdução e metodologia| Carlos                |

## 2. Introdução

<p align="justify" style="text-indent: 20px">"Padrões de projeto são soluções recorrentes para problemas de projeto orientados a objetos em um contexto particular.
Quando usados de forma eficaz, eles podem ajudar a melhorar a eficiência no esforço de projeto detalhado, fornecendo soluções reutilizáveis de alta qualidade que podem ser aplicadas em muitas aplicações práticas." [1]</p>
<p align="justify" style="text-indent: 20px">Sendo assim, padrões GRASP (General Responsability Assignment Software Patterns) são um conjunto de príncipios baseados em conceitos para atribuição de responsabilidade a classes e objetos [2]. A responsabilidade pode ser entendida como a obrigação (papel) que um objeto possui dentro do seu escopo, cabendo ainda considerar as interações com outros objetos [3].</p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">Como forma de ter um melhor preparo para a aplicação dos padrões GRASP no projeto assim como um melhor entendimento do conteúdo, este documento foi elaborado pelos integrantes Carlos Eduardo e Paulo Vitor. Após estudos individuais e reunião para planejamento, os tópicos aqui presentes foram divididos e elaborados pelos integrantes há pouco citados. </p>

## 4. Padrões GRASP

### 4.1 Polimorfismo

<p align="justify" style="text-indent: 20px">O polimorfismo é um recurso muito importante na orientação a objetos, se trata da capacidade de classes de mesmo tipo de possuírem métodos que se comportam de formas diferentes. </p>

<p>"Isso permite que objetos da mesma hierarquia de tipo se comportem de forma diferente em tempo de execução simplesmente associando a chamada de método de interface à instância de tempo de execução apropriada. Esse recurso é conhecido como polimorfismo." [1]</p>

<p align="justify" style="text-indent: 20px">Como exemplo temos o uso de uma classe abstrata "Peca" para a representação de algumas peças do jogo de xadrez, sendo que cada classe descendente sobrescreveu o método "mover":</p>

<center>
<img src="../../../assets/padroes_projetos/exemploPolimorfismo.png" class="zoom"> 
<h6>Figura 1: Exemplo Polimorfismo.</h6>
<h6>Fonte: Programação
Orientada a Objetos. Diego Oliveira. [4]</h6>
</center>

### 4.2 Criador

<p align="justify" style="text-indent: 20px">"Padrões de design criacional são padrões para abstrair e controlar a maneira como os objetos são criados em aplicativos de software. Eles desempenham um papel fundamental no projeto de sistemas, tornando-os independentes de como os objetos no sistema são criados, compostos e representados." [1]</p>
<p align="justify" style="text-indent: 20px">A responsabilidade de Criador é usada para definir qual classe é responsável pela criação de determinado objeto. Para isso, definindo A e B como classes distintas e B como possível responsável por criar instâncias de A, pode-se realizar os seguintes questionamentos [4]:</p>

- B “contém” A ou é uma composição de A.
- B registra A.
- B usa A de maneira muito próxima.
- B tem dados iniciais de A, os quais serão passados para A quando este
for criado. B é um “especialista” em relação à criação de A.

<p align="justify" style="text-indent: 20px"></p>

### 4.3 Especialista

### 4.4 Coesão 

### 4.5 Acoplamento 
     
### 4.6 Controlador

### 4.7 Invenção pura ou Fabricação Própria

### 4.8 Variações Protegidas

### 4.9 Indireção


## 5. Referências

> [1] Otero, Carlos. Software Engineering Design : Theory and Practice, Auerbach Publishers, Incorporated, 2012. ProQuest Ebook Central, http://ebookcentral.proquest.com/lib/univbrasilia-ebooks/detail.action?docID=1580108.
Created from univbrasilia-ebooks on 2022-03-03 22:07:59.

> [2] https://medium.com/@leandrovboas/padr%C3%B5es-grasp-padr%C3%B5es-de-atribuir-responsabilidades-1ae4351eb204

> [3] https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704

> [4] Milene

> [5] https://edisciplinas.usp.br/pluginfile.php/2186358/mod_resource/content/1/Aula09_GRASP.pdf]

> https://levelup.gitconnected.com/what-are-general-responsibility-assignment-software-patterns-6ad9635a44da