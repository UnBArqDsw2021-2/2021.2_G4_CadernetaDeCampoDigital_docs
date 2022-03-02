# GOFS Comportamentais

## 1. Versionamento

| Versão | Data       | Descrição                                  | Autor(es)                 |
| ------ | ---------- | ------------------------------------------ | ------------------------- |
| 1.0    | 01/03/2022 | Abertura do documento                      | Brenno e Thiago           |
| 1.1    | 02/03/2022 | Adicionando tópicos 4.1 a 4.5              | Brenno                    |

## 2. Introdução

<p align="justify" style="text-indent: 20px"> </p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">A metodologia utilizada pela dupla responsável foi separar cinco tópicos para cada integrantes documentarem separadamente e ao final se juntar para revisar o trabalho, além de criar a introdução.</p>

## 4. GoF's Comportamentais

### 4.1 <i>Observer</i>

<p align="justify" style="text-indent: 20px">O padrão de projeto <i>Observer</i> tem como objetivo "definir um mecanismo eficiente para reagir às alterações realizadas em determinados objetos"[1], funcionando como um mecanismo de assinatura[2] para enviar as mudanças.</p>

<p align="justify" style="text-indent: 20px">Para a modelagem desse padrão é preciso a implementação dos seguintes objetos:</p>
- **Observador** **(*****Observer*****)**: Interface padronizadora dos objetos observadores concretos  relacionados às alterações, os <i>Subjects</i>.
- **Observador Concreto** **(*****ConcretObserver*****)**: Classes que implementam observadores específicos.
- **Assunto** **(*****Subject*****)**: Interface que padroniza objetos a serem observados.
- **Assunto Concreto** **(*****ConcretSubject*****)**: Classes concretas a serem observadas, implementando o Assunto.

<center>
<img src="../../../assets/padroes_projetos/observer_exemplo.png" class="zoom"> 
<h6>Figura 1: Exemplo Observer</h6>
<h6>Fonte: Padrões de Projetos[3]</h6>
</center>

### 4.2 <i>State</i>

<p align="justify" style="text-indent: 20px">O padrão <i>State</i> propõe a alteração do comportamento de um objeto dependendo do estado que ele possui[4], parecendo que sua classe foi alterada[3].</p>

<p align="justify" style="text-indent: 20px">A modelagem do Estado possui os participantes abaixo:</p>
- **Context**: Classe que define o que será de interesse aos clientes, isto é, fará referência ao <i>State</i>.
- **Estado** **(*****State*****)**: Interface que define os estados do <i>Context</i>.
- **Estado Concreto** **(*****ConcreteState*****)**: Implementação do Estado de acordo com sua peculiaridade.

<center>
<img src="../../../assets/padroes_projetos/state_exemplo.png" class="zoom"> 
<h6>Figura 2: Exemplo State</h6>
<h6>Fonte: Padrões de Projetos[3]</h6>
</center>

### 4.3 <i>Strategy</i>

<p align="justify" style="text-indent: 20px">A partir do padrão Strategy é possível variar os algoritmos utilizados na resolução de determinado problema[1].</p>

<p align="justify" style="text-indent: 20px">A estrutura necessária para a implementação do padrão precisa dos seguintes elementos::</p>
- **Estratégia** **(*****Strategy*****)**: Interface para a definição dos algoritmos a serem suportados.
- **Estratégia Concreta** **(*****ConcreteStrategy*****)**: Implementação do algoritmo a ser utilizado.
- **Contexto** **(*****Context*****)**: Classe para chamar a Estratégia.

<center>
<img src="../../../assets/padroes_projetos/strategy_exemplo.png" class="zoom"> 
<h6>Figura 3: Exemplo Strategy</h6>
<h6>Fonte: Padrões de Projetos[3]</h6>
</center>

### 4.4 <i>Template Method</i>

<p align="justify" style="text-indent: 20px">O <i>Template Method</i> busca definir o esqueleto de um algoritmo em sua superclasse, enquanto as suas subclasses sobrescrevem as etapas ao mesmo tempo que sua estrutura é mantida[5].</p>

<p align="justify" style="text-indent: 20px">Sua estruturação consiste em:</p>
- **Classe Abstrata** **(*****AbstractClass*****)**: Classe abstrata para a definição das operações primitivas e qual sequência deve ser seguida.
- **Classe Concreta** **(*****ConcreteClass*****)**: Implementação das operações primitivas a serem utilizadas.

<center>
<img src="../../../assets/padroes_projetos/template_method_exemplo.png" class="zoom"> 
<h6>Figura 4: Exemplo Template Method</h6>
<h6>Fonte: Padrões de Projetos[3]</h6>
</center>

### 4.5 <i>Chain of Responsibility</i>

<p align="justify" style="text-indent: 20px">O padrão de projeto <i>Chain of Responsibility</i> tem como objetivo evitar a dependência entre objetos receptores com seus solicitantes[1]. Para que seu objetivo seja alcançado é preciso que uma corrente de <i>handlers</i> processe os pedidos[6].</p>

<p align="justify" style="text-indent: 20px">Os participantes abaixo definem sua estrutura:</p>
- **Handler**: Interface para a definição do método para lidar com os pedidos, podem também conter o método para chamar o próximo <i>handler</i>.
- **ConcreteHandler**: Implementação dos métodos definidos pela interface <i>Handler</i>.
- **Cliente** **(*****Client*****)**: Objeto iniciador da solicitação, enviando o pedido ao handler desejado.

<center>
<img src="../../../assets/padroes_projetos/cor_exemplo.png" class="zoom"> 
<h6>Figura 5: Exemplo Chain of Responsibility</h6>
<h6>Fonte: Padrões de Projetos[3]</h6>
</center>

### 4.6 <i>Command</i>

<p align="justify" style="text-indent: 20px"></p>

<center>
<img src="../../../assets/padroes_projetos/" class="zoom"> 
<h6>Figura 6: </h6>
<h6>Fonte: </h6>
</center>

### 4.7 <i>Iterator</i>

<p align="justify" style="text-indent: 20px"></p>

<center>
<img src="../../../assets/padroes_projetos/" class="zoom"> 
<h6>Figura 7: </h6>
<h6>Fonte: </h6>
</center>

### 4.8 <i>Mediator</i>

<p align="justify" style="text-indent: 20px"></p>

<center>
<img src="../../../assets/padroes_projetos/" class="zoom"> 
<h6>Figura 8: </h6>
<h6>Fonte: </h6>
</center>

### 4.9 <i>Visitor</i>

<p align="justify" style="text-indent: 20px"></p>

<center>
<img src="../../../assets/padroes_projetos/" class="zoom"> 
<h6>Figura 9: </h6>
<h6>Fonte: </h6>
</center>

### 4.10 <i>Memento</i>

<p align="justify" style="text-indent: 20px"></p>

<center>
<img src="../../../assets/padroes_projetos/" class="zoom"> 
<h6>Figura 10: </h6>
<h6>Fonte: </h6>
</center>

## 5. Referências

> [1] SERRANO, Milene. Arquitetura e Desenho de Software. **GoFs Comportamentais**. Acesso em: 28 fev. 2022.

> [2] Refactoring Guru. **Observer**. Disponível em: <a href="https://refactoring.guru/pt-br/design-patterns/observer">https://refactoring.guru/pt-br/design-patterns/observer</a>. Acesso em: 01 mar. 2022

> [3] GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. **Padrões de Projetos**. Grupo A, 2011. 9788577800469. Disponível em: <a href="https://integrada.minhabiblioteca.com.br/#/books/9788577800469/">https://integrada.minhabiblioteca.com.br/#/books/9788577800469/</a>. Acesso em: 01 mar. 2022.

> [4] Refactoring Guru. **State**. Disponível em: <a href="https://refactoring.guru/pt-br/design-patterns/state">https://refactoring.guru/pt-br/design-patterns/state</a>. Acesso em: 01 mar. 2022

> [5] Refactoring Guru. **Template Method**. Disponível em: <a href="https://refactoring.guru/pt-br/design-patterns/template-method">https://refactoring.guru/pt-br/design-patterns/template-method</a>. Acesso em: 02 mar. 2022

> [6] Refactoring Guru. **Chain of Responsibility**. Disponível em: <a href="https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility">https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility</a>. Acesso em: 02 mar. 2022
