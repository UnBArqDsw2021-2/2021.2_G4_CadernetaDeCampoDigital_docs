# Estilos e Padrões Arquiteturais - Parte 4

## 1. Versionamento

| Versão | Data       | Descrição                                    | Autor(es)         |
| ------ | ---------- | -------------------------------------------- | -----------       |
| 1.0    | 22/03/2022 | Abertura do documento                        | Vitor Lamego      |
| 1.1    | 22/03/222  | Adição do resultado dos estudos              | Vitor Lamego      |

## 2. Introdução

<p align="justify" style="text-indent: 20px">Conforme conteúdo estudado na disciplina, o assunto de "Estilos e Padrões Arquiteturais" foi divido em algumas partes para melhor divisão e compreensão. Sendo assim, esse documento é responsável pela documentação dos assuntos vistos na última parte, sendo apresentado o estilo arquitetural orientado a eventos e orientado a serviços.</p>

## 3. Estilo Arquitetural Orientado a Eventos

<p align="justify" style="text-indent: 20px">Durante a disciplina, foi definido que a arquitetura de software é responsável por definir a estrutura que será implementada em um determinado software. Sabendo disso, iremos abordar alguns pontos importantes relacionados ao Estilo Arquitetural Orientado a Eventos. Para isso, é importante entender que um evento é tudo aquilo que representa uma mudança significativa no estado do software em questão, podendo ter uma origem interna, algum clique por parte d usuário, ou externa, alguma informação recebida do servidor [1]. A principal diferença entre um evento e uma entrada qualquer é que o evento está fora de controle do processo que o manipula. [2]</p>

<p align="justify" style="text-indent: 20px">Portanto, a arquitetura orientada a eventos acaba sendo voltada para o design de aplicações, e hoje em dia esse estilo de arquitetura pode ser implementado facilmente por qualquer framework que esteja sendo utilizado para o projeto. Para a efetiva implementação do estilo em questão é fundamental a presença de alguns componentes que lidam com a captura de evento, comunicação, processamento e persistência, sendo detalhado mais a frente a importância de cada um dentro dessa arquitetura. [1]</p>

<p align="justify" style="text-indent: 20px">De forma básica, o seu funcionamento consiste em um evento ser publicado em um determinado barramento ou alguma fila e os serviços que possuem interesse nesse determinado evento consomem e reagem [3]. Entretanto, será abordado dois modelos de eventos existentes e que são bastante utilizados, sendo eles: </p>

<ol>
    <li><b>Pub/Sub</b>: Assim que um evento é recebido, ele é enviado para todos os assinantes, naquele momento, daquele determinado evento.</li>
    <li><b>Streaming de Eventos</b>: Os eventos ficam armazenados em um registro, sendo assim os consumidores não precisam se inscrever naquele determinado evento, podendo acessar os registros armazenados e reagir a qualquer evento que já tenha ocorrido a qualquer momento. </li>
</ol>

### Pontos Positivos

<p align="justify" style="text-indent: 20px">A partir das explicações dadas e dos estudos feitos, pode-se perceber que existem algumas vantagens na utilização desse determinado estilo arquitetural no projeto. Alguns dos benefícios e das causas para utilização serão listados a seguir: </p>

<ol>
    <li><b>Baixo acoplamento</b>: Os produtores de evento não sabem que os consumidores estão detectando os eventos e muito menos o que está sendo feito como resposta</li>
    <li><b>Capacidade de adaptação</b>: A mudança de estados pode ser muito bem controlada a partir do consumo de eventos na aplicação, podendo ser feita tomadas de decisões em tempo real. </li>
    <li><b>Escalabilidade</b>: A sua evolução acaba sendo uma tarefa muito simples, além de fornencer uma capacidade de resposta muito melhor para o projeto, aumentando a escalabilidade.</li>
</ol>

## 4. Estilo Arquitetural Orientado a Serviços

<p align="justify" style="text-indent: 20px">Antes de falarmos sobre a arquitetura orientada a serviços, é bom entendermos o que seria um serviço. Portanto, serviço é uma unidade ou conjunto de funcionalidades de um software independente, sendo desenvolvida para executar uma tarefa específica.</p>

<p align="justify" style="text-indent: 20px">O estilo arquitetural orientado a serviços consiste em um tipo de design em que os componentes são reutilizáveis a partir do uso de algumas interfaces de serviços com uma linguagem de comunicação comum em uma rede [4]. Foi a partir dessa nova arquitetura de software que as empresas conseguiram ter um acesso mais democrático e viável a servidores remotos que estão fora da própria organização, além de permitir que as empresas e organizações tornem acessíveis as suas informações para outros programas a partir da publicação de uma interface de WebService [2]. Resumidamente, a arquitetura orientada a serviços integra componentes de software que foram implantados e mantidos separadamente, permitindo que trabalhem juntos para formar aplicações que funcionam em sistemas diferentes [4].</p>

<p align="justify" style="text-indent: 20px">Falando um pouco mais sobre o funcionamento do estilo arquitetural orientado a serviços, a comunicação entre serviços é feita por um sistema de "baixo acomplamento" o que permite que a conexão entre os seus componentes seja mais simples por não possuírem dependência entre si, o que também permite a reutilização desses mesmos serviços em outros projetos. Antigamente, a cada projeto que se fazia necessário a utilização de serviços era feito um processo complexo de conexão da aplicação que incluía vários processos e fases que davam certo trabalho, também conhecido como modelo monoçítico.</p>

### Pontos Positivos

<p align="justify" style="text-indent: 20px">Alguns pontos positivos da utilização desse estilo de arquitetura em comparação ao estilo monolítico são:</p>

<ol>
    <li><b>Flexibilidade</b>: Como comentado anteriormente, a reutilização dos serviços permite a criação de novas aplicações de maneira muito mais rápida</li>
    <li><b>Fácil manutenção</b>: Os serviços são independentes, portanto é possível realizar atualizações e modificações sem comprometer outros serviços</li>
    <li><b>Disponibilidade</b>: os recursos estão disponíveis para todos.</li>
</ol>

## 5. Referências

> [1] RedHat. **O que é uma arquitetura orientada por eventos**. <a href="https://www.redhat.com/pt-br/topics/integration/what-is-event-driven-architecture#:~:text=A%20arquitetura%20orientada%20a%20eventos,modelo%20tradicional%20orientado%20a%20solicita%C3%A7%C3%B5es.">RedHat - Arquitetura Orientada a Eventos</a>.  Acesso em: 22 mar. 2022.

> [2] SERRANO, Milene. Arquitetura e Desenho de Software. **AULA - ESTILOS E PADRÕES ARQUITETURAIS IV**. Acesso em: 22 mar. 2022.

> [3] Medium. **EDA - Arquitetura Orietada a Eventos**. <a href="https://medium.com/alex-ribeiro/eda-arquitetura-orientada-a-eventos-ff197b2b429c">Medium - Arquitetura Orientada a Eventos</a>.  Acesso em: 22 mar. 2022.

> [4] RedHat. **O que é arquitetura orientada a serviços (SOA)?**. <a href="https://www.redhat.com/pt-br/topics/cloud-native-apps/what-is-service-oriented-architecture#:~:text=Arquitetura%20orientada%20a%20servi%C3%A7os%20(SOA)%20%C3%A9%20um%20tipo%20de%20design,comunica%C3%A7%C3%A3o%20comum%20em%20uma%20rede.">RedHat - Arquitetura Orientada a Serviços</a>.  Acesso em: 22 mar. 2022.