# Estilos e Padrões Arquiteturais Parte 1

## 1. Versionamento

| Versão | Data       | Descrição                                    | Autor(es)   |
| ------ | ---------- | -------------------------------------------- | ----------- |
| 1.0    | 22/03/2022 | Abertura do documento                        | Carlos      |
| 1.1    | 22/03/222  | Adição do introdução, metodologia e tópico 4 | Carlos      |

## 2. Introdução

<p align="justify" style="text-indent: 20px">Com o objetivo de promover uma maior aderência ao conteúdo, este documento expõe um resumo dos estilos e padrões arquiteturais parte 1 disponibilizados durante a realização da disciplina.</p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">De forma a distribuir melhor as tarefas a serem feitas e garantir um melhor aproveitamento de tempo, os tópicos a seguir foram divididos entre os participantes Carlos e Eduardo para que individualmente realizassem sua documentação.</p>

## 4. Arquiteturas

<p align="justify" style="text-indent: 20px"> A palavra arquitetura tem em seu significado o sentido de edificar, e no escopo de software pode ser compreendida como a estrutura de um sistema, sendo constituída das propriedades e relacionamentos entre seus componentes [1].</p>

### 4.1 Monolíticas

<p align="justify" style="text-indent: 20px">A arquitetura monolítica é baseada em processamento centralizado, com terminais "burros" e redes de comunicação mais lentas. Suas funcionalidades são realizadas em um único processo, uma única instância de servidor, e para escalabilidade é feita a replicação. Para evolução e/ou substituição se torna algo complicado, devido ao sistema ter sido construído em conjunto [2]. Arquitetura muito usada no desenvolvimento de aplicações web [3].</p>

Possui as seguintes vantagens [2, 3]:

- Devido ao código estar presente em apenas um lugar sua gerência é facilitada, em termos de segurança, controle de usuários e aplicações.
- Facilita a aplicação e execução de testes de integração e end-to-end.
- A <i>stack</i>(conjunto de tecnologias) é mais condensada.

E as seguintes desvantagens [2, 3]:

- Falta de autonomia e limitação na interface para o usuário.
- Dependência de replicação para escalabilidade.
- Alto custo de manutenção e evolução.
- Alto acoplamento.
- Difícil adoção de nova tecnologia.

### 4.2 Distribuídas

<p align="justify" style="text-indent: 20px">A arquitetura distribuída é baseada em servidores de serviços compartilhados com alta capacidade de processamento, com estações de trabalho executando aplicações locais, sendo necessário redes mais rápidas [2]. </p>

<p align="justify" style="text-indent: 20px">"É necessário pensar em como os componentes estão organizados e como devem interagir entre si bem como com outros componentes. A concepção/implantação efetiva de um sistema distribuído requer a instanciação e associação de componentes de software em
máquinas reais, o que pode ser feito de diferentes maneiras." [4]</p>

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

### 5.2 N-Camadas

## 6. Padrão MVC

## 7. Referências

> [1] SIQUEIRA, Fernando de. Sistemas Distribuidos. **Arquiteturas Distribuidas**. <a href="https://sites.google.com/site/proffdesiqsistemasdistribuidos/aulas/2--arquiteturas-distribuidas">https://sites.google.com/site/proffdesiqsistemasdistribuidos/aulas/2--arquiteturas-distribuidas</a>.  Acesso em: 22 mar. 2022.

> [2] SERRANO, Milene. Arquitetura e Desenho de Software. **AULA - ESTILOS E PADRÕES ARQUITETURAIS I**. Acesso em: 22 mar. 2022.

> [3] Medium. **Padrões de Arquitetura Web — Monolítica ou Micro Serviços?** Disponível em: <a href="https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe">https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe </a>. Acesso em: 22 mar. 2022.

> [4] FAINA, Luís F. 2013. **Arquiteturas de Sist. Distribuídos**. <a href="http://www.facom.ufu.br/~faina/BCC_Crs/GSI028-2014-1S/DL/DS-Ch02.pdf">http://www.facom.ufu.br/~faina/BCC_Crs/GSI028-2014-1S/DL/DS-Ch02.pdf</a>. Acesso em: 22 mar. 2022.
