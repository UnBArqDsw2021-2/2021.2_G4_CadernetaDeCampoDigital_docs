# GoF's Estruturais

## 1. Versionamento

| Versão | Data       | Descrição                                  | Autor(es)                 |
| ------ | ---------- | ------------------------------------------ | ------------------------- |
| 1.0    | 03/03/2022 | Criação do documento                       | Eduardo Afonso |
| 1.1    | 03/03/2022 | Adicionando metodologia, adapter, composite, bridge e facade| Eduardo Afonso |

## 2. Introdução

## 3. Metodologia

<p align="justify" style="text-indent: 20px">Como metodologia escolhida pela equipe para a produção desse documento, optou-se pelos integrantes Eduardo Afonso e Vitor Lima debaterem e organizarem os estudos e documentação utilizando um chat privado no Telegram.</p>

## 4. GoF's Estruturais

### 4.1 <i>Adapter</i>

<p align="justify" style="text-indent: 20px">O adapter tem como principal objetivo fazer com que seja possível substituir um objeto, que é a solução atual para o problema, por outro objeto que resolve o mesmo problema porém com outra interface [1].</p>

<p align="justify" style="text-indent: 20px">Esse padrão de projeto utiliza de uma classe herdeira da solução atual (Adapter) que sobrescreve os métodos do pai (Target), mantendo a mesma assinatura porém chama os métodos da classe que contém a nova solução (Adaptee). Com isso, o cliente (Client) continua consumindo os dados da mesma forma, porém com os resultados provenientes da nova solução [1]. Conforme exemplificado na figura 1.</p>

<p align="justify" style="text-indent: 20px">Uma das utilizações mais comuns do adapter é para fazer a substituição de uma solução antiga ou obsoleta por uma mais moderna e eficaz. Utilizando desse padrão de projeto é possível alterar a solução sem fazer grandes mudanças na forma como os clientes consomem o objeto alterado [1].</p>

<center>
<img src="../../../assets/padroes_projetos/adapter_exemplo.png" class="zoom"> 
<h6>Figura 1: Exemplo genérico do padrão de projeto adapter.</h6>
<h6>Fonte: 09b - Vídeo-Aula - DSW - GoFs - Estruturais - Adapter [1]</h6>
</center>

### 4.2 <i>Composite</i>

<p align="justify" style="text-indent: 20px">O padrão de projeto composite tem como objetivo fazer com que o cliente consiga interagir com folhas (não possui filhos) e nós (possui filhos, folhas ou outros nós) de uma árvore de componentes sem distinção. Isto é, a operação necessária para o cliente interagir com uma folha é a mesma necessária para interagir com um nó [2].</p>

<p align="justify" style="text-indent: 20px">Para utilizar esse padrão de projeto, é necessário ter uma classe ou interface (Component) que irá definir um comportamento das Leafs (folhas) e dos Composites (nós). Cada Leaf irá sobrescrever os métodos da Component à sua própria maneira. E os Composites, além de sobrescrever os métodos, também terão métodos para adicionar ou remover Leafs criando uma relação todo-parte [3]. Conforme exemplificado na figura 2.</p>

<center>
<img src="../../../assets/padroes_projetos/composite_exemplo.png" class="zoom"> 
<h6>Figura 2: Exemplo genérico do padrão de projeto composite.</h6>
<h6>Fonte: 09c - Vídeo-Aula - DSW - GoFs - Estruturais - Composite [3]</h6>
</center>

### 4.3 <i>Bridge</i>

<p align="justify" style="text-indent: 20px">Esse padrão de projeto parte do princípio que existe uma hierarquia na lógica de abstração e que existem elementos nessa hierarquia que se tornam muito específicos ou que acabam divergindo do intuito principal da abstração. Então para resolver esse problema, as duas lógicas são separadas em duas hierarquias diferentes, uma que trata sobre o foco principal e outra sobre o assunto que divergiu do foco principal [4].</p>

<p align="justify" style="text-indent: 20px">A hierarquia principal irá agregar a hierarquia que foi separada, criando uma ponte entre as duas. Mantendo assim o projeto mais desacoplado, permitindo que a mesma lógica que foi separada possa ser trabalhada e reaproveitada de forma independente [4]. </p>

<center>
<img src="../../../assets/padroes_projetos/bridge_exemplo.png" class="zoom"> 
<h6>Figura 3: Exemplo genérico do padrão de projeto bridge.</h6>
<h6>Fonte: 09d - Vídeo-Aula - DSW - GoFs - Estruturais - Demais Padrões - Visão Rápida [4]</h6>
</center>

### 4.4 <i>Facade</i>

<p align="justify" style="text-indent: 20px">O padrão de projeto facade funciona basicamente criando uma interface que faz o intermédio entre o cliente e os serviços que serão utilizados. A interface do facade geralmente oferece os serviços de uma forma mais amigável para que o cliente consiga realizar as suas requisições de forma simplificada e unificada, evitando assim que o cliente tenha que se adaptar para utilizar as diferentes interfaces dos diferentes serviços.</p>

<center>
<img src="../../../assets/padroes_projetos/facade_exemplo.png" class="zoom"> 
<h6>Figura 1: Exemplo genérico do padrão de projeto facade.</h6>
<h6>Fonte: 09d - Vídeo-Aula - DSW - GoFs - Estruturais - Demais Padrões - Visão Rápida [4]</h6>
</center>

### 4.5 <i>Decorator</i>

### 4.6 <i>Proxy</i>

### 4.7 <i>Flyweigth</i>

## 5. Referências

> [1] SERRANO, Milene. 09b - Vídeo-Aula - DSW - GoFs - Estruturais - Adapter. Material apresentado para a disciplina de Arquitetura e Desenho de Software no curso de Engenharia de Software da Universidade de Brasília, FGA.

> [2] Composite Pattern. Spring Framework Guru. Disponível em: https://springframework.guru/gang-of-four-design-patterns/composite-pattern/. Acesso em: 03 de março de 2022.

> [3] SERRANO, Milene. 09c - Vídeo-Aula - DSW - GoFs - Estruturais - Composite. Material apresentado para a disciplina de Arquitetura e Desenho de Software no curso de Engenharia de Software da Universidade de Brasília, FGA.

> [4] SERRANO, Milene. 09d - Vídeo-Aula - DSW - GoFs - Estruturais - Demais Padrões - Visão Rápida. Material apresentado para a disciplina de Arquitetura e Desenho de Software no curso de Engenharia de Software da Universidade de Brasília, FGA.