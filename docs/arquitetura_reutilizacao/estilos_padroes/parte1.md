# Estilos e Padrões Arquiteturais Parte 1

## 1. Versionamento

| Versão | Data       | Descrição                                    | Autor(es)   |
| ------ | ---------- | -------------------------------------------- | ----------- |
| 1.0    | 22/03/2022 | Abertura do documento                        | Carlos      |
| 1.1    | 22/03/222  | Adição do introdução, metodologia e tópico 4 | Carlos      |
| 1.2    | 23/03/222  | Adição do stand-alone, n-camadas e mvc | Eduardo      |
| 1.2.1    | 28/03/222  | Revisão por pares | João e Thiago      |

## 2. Introdução

<p align="justify" style="text-indent: 20px">Com o objetivo de promover uma maior aderência ao conteúdo, este documento expõe um resumo dos estilos e padrões arquiteturais parte 1 disponibilizados durante a realização da disciplina [2].</p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">De forma a distribuir melhor as tarefas a serem feitas e garantir um melhor aproveitamento de tempo, os tópicos a seguir foram divididos entre os participantes Carlos e Eduardo para que individualmente realizassem sua documentação.</p>

## 4. Arquiteturas

<p align="justify" style="text-indent: 20px"> A palavra arquitetura tem em seu significado o sentido de edificar, e no escopo de software pode ser compreendida como a estrutura de um sistema, sendo constituída das propriedades e relacionamentos entre seus componentes [1].</p>

### 4.1 Monolíticas

<p align="justify" style="text-indent: 20px">A arquitetura monolítica é baseada em processamento centralizado, com terminais "burros" e redes de comunicação mais lentas. Suas funcionalidades são realizadas em um único processo, uma única instância de servidor, e para escalabilidade é feita a replicação. Para evolução e/ou substituição se torna algo complicado, devido ao sistema ter sido construído em conjunto [2]. Esse é um tipo de arquitetura muito usada no desenvolvimento de aplicações web [3].</p>

Possui as seguintes vantagens [2, 3]:

- Devido ao código estar presente em apenas um lugar sua gerência é facilitada, em termos de segurança, controle de usuários e aplicações.
- Facilita a aplicação e execução de testes de integração e end-to-end.
- A <i>stack</i>(conjunto de tecnologias) é mais condensada.

E as seguintes desvantagens [2, 3]:

- Falta de autonomia e limitação na interface para o usuário.
- Dependência de replicação para escalabilidade.
- Alto custo de manutenção e evolução.
- Alto acoplamento.
- Difícil adoção de novas tecnologias.

### 4.2 Distribuídas

<p align="justify" style="text-indent: 20px">A arquitetura distribuída é baseada em servidores de serviços compartilhados com alta capacidade de processamento, com estações de trabalho executando aplicações locais, sendo necessárias redes mais rápidas [2]. </p>

<p align="justify" style="text-indent: 20px">"Nessa arquitetura é necessário pensar em como os componentes estão organizados e como devem interagir entre si, bem como, com outros componentes. A concepção/implantação efetiva de um sistema distribuído requer a instanciação e associação de componentes de software em máquinas reais, o que pode ser feito de diferentes maneiras." [4]</p>

Possui as seguintes vantagens [2]:

- Autonomia para o usuário.
- Interface montada localmente e com recursos gráficos.
- Processamento espelhado.
- Arquiteturas de software e comunicação podem ser proprietárias, mas com recursos de integração entre plataformas.

E as seguintes desvantagens [2]:

- Sobrecarga da rede.
- Dificuldade de gerência, em termos de segurança, controle de usuários e aplicações.
## 5. Estilos

### 5.1 Stand-alone

<p align="justify" style="text-indent: 20px">Pode-se traduzir o termo "stand-alone" como "de pé por si só", e esta tradução resume bem o estilo arquitetural. O stand-alone tem como premissa que o sistema deve funcionar de maneira independente e autossuficiente, sem consumir ou utilizar os serviços de terceiros. Em decorrência dessa limitação expressa na definição, o estilo é utilizado em produtos mais simples [2].</p>

Possui a seguinte vantagem [2]:

- Estilo extremamente simples.


E a seguinte desvantagem [2]:

- Limita a capacidade de expansão do projeto.


### 5.2 N-Camadas

<p align="justify" style="text-indent: 20px">Um estilo de projeto bastante popular é o estilo n-camadas. Ele consiste basicamente em dividir o sistema em um conjunto de camadas, sendo que cada camada possui seu próprio objetivo. O estilo n-camadas é amplamente versátil, podendo acrescentar ou remover camadas conforme as necessidades e particularidades de cada projeto. Por conta disso existem diversos padrões e modelos derivados do estilo n-camadas [2].</p>

<p align="justify" style="text-indent: 20px">Cada camada deve estar em um nível de abstração diferente, sendo altamente recomendado que cada camada dependa somente da camada de nível imediatamente inferior ao dela (arquitetura restrita), ou no mínimo de quaisquer camadas que sejam de níveis inferiores ao dela (arquitetura relaxada), nunca de camadas de nível superior [2].</p>

Possui as seguintes vantagens [2]:

- Camadas podem ser reutilizadas.
- Por as camadas estarem dispostas em níveis de abstração diferentes, as dependências entre as camadas é minimizada.
- É um estilo mais versátil e de fácil adaptação.
- Pode ser utilizados em projetos de complexidade simples ou elevada.

E a seguinte desvantagem [2]:

- Mudanças nas camadas mais baixas podem resultar em um efeito cascata, afetando todas as camadas acima.

## 6. Padrão MVC

<p align="justify" style="text-indent: 20px">O padrão MVC utiliza o estilo de projeto n-camadas com 3 camadas lógicas, sendo elas Model (Modelo), View (Visão) e Controller (Controladora). A camada Model é responsável por manter a funcionalidade principal do projeto e os dados associados a cada entidades de domínio, a View é responsável pela apresentação dos dados ao usuário e a Controller, além de fazer o intermédio entre a Model e a View, também cuida das interações do usuário [2].</p>

<p align="justify" style="text-indent: 20px">Este padrão de projeto é muito recomendado para projetos Web, ou projetos em que há mudanças recorrentes nas interfaces ou na apresentação e valor dos dados [2].</p>

Possui as seguintes vantagens [2]:

- Permite mudanças independentes em cada camada.
- Níveis de abstração bem definidos e de fácil entedimento.

E as seguintes desvantagens [2]:

- Para códigos muito simples pode acrescentar uma complexidade desnecessária.
- Alto acoplamento das camadas controller e view dependendo da implementação.

## 7. Referências

> [1] SIQUEIRA, Fernando de. Sistemas Distribuidos. **Arquiteturas Distribuidas**. <a href="https://sites.google.com/site/proffdesiqsistemasdistribuidos/aulas/2--arquiteturas-distribuidas">https://sites.google.com/site/proffdesiqsistemasdistribuidos/aulas/2--arquiteturas-distribuidas</a>.  Acesso em: 22 mar. 2022.

> [2] SERRANO, Milene. Arquitetura e Desenho de Software. **AULA - ESTILOS E PADRÕES ARQUITETURAIS I**. Acesso em: 22 mar. 2022.

> [3] Medium. **Padrões de Arquitetura Web — Monolítica ou Micro Serviços?** Disponível em: <a href="https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe">https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe </a>. Acesso em: 22 mar. 2022.

> [4] FAINA, Luís F. 2013. **Arquiteturas de Sist. Distribuídos**. <a href="http://www.facom.ufu.br/~faina/BCC_Crs/GSI028-2014-1S/DL/DS-Ch02.pdf">http://www.facom.ufu.br/~faina/BCC_Crs/GSI028-2014-1S/DL/DS-Ch02.pdf</a>. Acesso em: 22 mar. 2022.