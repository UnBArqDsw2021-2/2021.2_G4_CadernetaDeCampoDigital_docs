# Reutilização Pytest

## 1. Versionamento

| Versão | Data       | Descrição                                  | Autor(es)                 |
| ------ | ---------- | ------------------------------------------ | ------------------------- |
| 1.0    | 27/03/2022 | Abertura do documento                      | Thiago                    |
| 1.1    | 27/03/2022 | Adição da introdução                       | Thiago                    |
| 1.2    | 27/03/2022 | Adição dos hot spots                       | Thiago                    |
| 1.3    | 27/03/2022 | Adição dos plugins                         | Thiago                    |

## 2. Introdução

<p align="justify" style="text-indent: 20px">O back-end da Caderneta de Campo digital utilizou da técnica de Desenvolvimento Orientado a Testes (TDD) no seu desenvolvimento para aumentar a qualidade do produto, aumentando a integridade e facilitando a refatoração. Para isso, o Pytest foi o framework escolhido para fornecer ferramentas de testes.</p>

<p align="justify" style="text-indent: 20px">O framework Pytest permite, de forma fácil, escrever testes pequenos e legíveis e escalar facilmente para suportar aplicações complexas [1]. Além disso, há uma interface simples para realizar testes de integração com o Django Rest Framework, fornecendo classes, decorators e métodos de execução e filtragem de testes reutilizáveis.</p>

## 3. _Hot Spots_

- Functions: fornece funções prontas para diversas comparações.
- Marks: fornece decoradores para estender os testes, como parametrize que permite rodar o teste com diversos parâmetros, e o xfail que permite ao teste falhar dado uma certa condição.
- Fixtures: fornece meios para preparar o ambiente antes de testar, provendo objetos pré-prontos para os testes.

## 4. Plugins

- freezegun: permite testar em diferentes tempos, fornecendo o mock do datetime.
- ipdb: permite o debug do código.
- model-bakery: fornece ferramentas para criar instâncias de classe.
- parameterized: fornece decoradores para testar um mesmo teste com diversos parâmetros diferentes.
- pytest-cov: fornece integração do pytest com o coverage para registrar a cobertura do código.
- pytest-django: fornece integração do pytest com o django.
- pytest-subtests: fornece a possibilidade de realizar subtestes, ou seja, testes dentro de outros testes.


## 5. Referências

> [1] **pytest: helps you write better programs**. Disponível em: <a href="https://docs.pytest.org/en/7.1.x/
">https://docs.pytest.org/en/7.1.x/</a>. Acesso em: 27 mar. 2022.
