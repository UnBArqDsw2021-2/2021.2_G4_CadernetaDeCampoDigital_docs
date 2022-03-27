# Reutilização Django

## 1. Versionamento

| Versão | Data       | Descrição                                  | Autor(es)                 |
| ------ | ---------- | ------------------------------------------ | ------------------------- |
| 1.0    | 27/03/2022 | Abertura do documento                      | Thiago                    |
| 1.1    | 27/03/2022 | Adição da introdução                       | Thiago                    |
| 1.2    | 27/03/2022 | Adição dos plugins                         | Thiago                    |

## 2. Introdução

<p align="justify" style="text-indent: 20px">O back-end da Caderneta de Campo digital também reutilizou diversos softwares para conseguir prover um serviço web, visando aumentar a qualidade do produto e a produtividade da equipe. Dessa forma, o Django foi o framework escolhido para implementação do back-end.</p>

<p align="justify" style="text-indent: 20px">O Django é um framework web python de alto nível que permite desenvolver de forma rápida, segura e manutenível um serviço web [1]. Ele fornece diversas ferramentas que facilitam o desenvolvimento. Uma delas, Django ORM, permite fazer um mapeamento objeto-relacional e foi muito utilizada para a comunicação com o banco de dados relacional.</p>

<p align="justify" style="text-indent: 20px">A comunicação entre o front-end e back-end é por meio de uma API REST. O Django Rest Framework, que é uma extensão do Django [2], concede uma grande liberdade, fornecendo ferramentas, como <i>serializers</i>, rotas e validações pré-prontas, para reutilização e implementação de uma API REST.</p>

## 3. Plugins

<p align="justify" style="text-indent: 20px">Também foi utilizado plugins para complementar as funcionalidades do Django e do Django Rest Framework. Eles foram muito úteis, uma vez que fornecem diversos serviços feitos e testados pela comunidade para que não haja a necessidade de reinventar a roda. Os plugins são listados abaixo.</p>

- django-cors-headers: adiciona cabeçalho do tipo Cross-Origin Resource Sharing</i> (CORS) nas respostas.
- djangorestframework-simplejwt: fornece autenticação por meio de JSON Web Token.
- django-fake-model: permite criar instâncias falsas de uma entidade do banco de dados para serem utilizadas em testes.
- django-filter: fornece novos meios de filtrar os conjuntos de dados do Django ORM.
- django-phonenumber-field: fornece um campo de número de telefone para as entidades do Django ORM
- django-polymorphic: simplifica o uso de herança em entidades do Django ORM.

## 4. Referências

> [1] **Django introduction**. Disponível em: <a href="https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction">https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction</a>. Acesso em: 27 mar. 2022.

> [2] **O que é o Django Rest Framework**. Disponível em: <a href="https://www.treinaweb.com.br/blog/o-que-e-o-django-rest-framework">https://www.treinaweb.com.br/blog/o-que-e-o-django-rest-framework</a>. Acesso em: 27 mar. 2022.
