# Casos de Uso

## 1. Versionamento

|Versão|Data|Descrição|Autor(es)|
|:------:|:----:|:---------:|:---------:|
|0.1|16/02/2022|Abertura do documento de casos de uso|Denniel William|
|1.0|17/02/2022|Introdução, especificação, referências|Denniel William|

## 2. Introdução

<p style="text-align: justify; text-indent: 20px">Os diagramas de caso de uso tem por objetivo auxiliar na modelagem, demonstrando o comportamento do sistema e ajudam a capturar seus requisitos. Eles identificam as interações entre o sistema e os atores. Seu foco é mostrar como o sistema se comporta a nível de usuário mas não descreve a operação interna.</p>.

<p style="text-align: justify; text-indent: 20px">Com os diagramas de caso de uso é possível modelar um sistema complexo em um único diagrama. Ele é desenvolvido na fase inicial do projeto e são consultados durante todo o processo de desenvolvimento</p>.

## 3. Diagrama de caso de uso

![Diagrama de caso de uso](/docs/assets/requisitos/modelagem/diagrama_de_caso_de_uso.jpg)
<p style="text-align: center; text-indent: 20px"><strong>Figura 1: Casos de Uso do Caderneta de Campo Digital.<br/>Fonte: Autoria própria</strong></p>.

## 4. Especificação dos Casos de Uso

### UC01 Login
|UC01|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> e/ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> conecta no sistema com uma conta individual|
|Ator| <a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a>, <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> |
|Pré-Condições| Acesso a internet e ter conta no aplicativo|
|Ação|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a> ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> entrar na conta|
|Fluxo principal| **FP01:** Fluxo de fazer login no aplicativo <br/> 1. Ator entra no aplicativo <br/> 2. Ator clica em conectar <br/> 3. Ator digita suas informações de login |
|Pós-condições| O ator poderá ter acesso as funcionalidades do seu tipo de <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> logado|
|Data de criação|17/02/2022|

### UC02 Cadastrar
|UC02|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> e/ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> cria conta no aplicativo |
|Ator|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a>, <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Acesso a internet |
|Ação|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a> ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criar conta|
|Fluxo principal| **FP01:** Fluxo de se cadastrar no aplicativo <br/> 1. Ator entra no aplicativo <br/> 2. Ator clica em Cadastrar <br/> 3. Ator digita suas informações de cadastro e confirma |
|Pós-condições| O ator terá conta criada no aplicativo|
|Data de criação|17/02/2022|

### UC03 Editar conta
|UC03|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> e/ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> edita informações da conta no aplicativo |
|Ator|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a>, <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Acesso a internet e ter conta no aplicativo|
|Ação|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a> ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> editar informações da conta|
|Fluxo principal| **FP01:** Fluxo de editar informações no aplicativo <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator acessa seu perfil <br/> 4. Ator altera suas informações e salva |
|Pós-condições| O ator poderá ter acesso as funcionalidades do seu tipo de <a href="/requisitos/modelagem/lexicos#usuario">usuário</a> logado|
|Data de criação|17/02/2022|

### UC04 Visualizar propriedade
|UC04|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#tecnico">técnico</a> visualiza propriedade do <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> e <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> visualiza sua propriedade |
|Ator|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a>, <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Acesso a internet, ter conta no aplicativo, ter <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> cadastrada |
|Ação|<a href="/requisitos/modelagem/lexicos#tecnico">Técnico</a> ou <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> visualizar informações da propriedade|
|Fluxo principal| **FP01:** Fluxo de visualizar propriedade no aplicativo <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em visualizar <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> |
|Pós-condições| O ator poderá ter acesso as informações da <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
|Data de criação|17/02/2022|

### UC05 Gerar caderneta de campo
|UC05|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição| O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> gera <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a>  |
|Ator|<a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet, ter ao menos uma <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> , um  <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> e um <a href="/requisitos/modelagem/lexicos#plantio">plantio</a> cadastrado |
|Ação| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> gerar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
|Fluxo principal| **FP01:** Fluxo de gerar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em gerar <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
|Pós-condições| O ator baixado um pdf com todas as informações da <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
|Data de criação| 17/02/2022 |

### UC06 Adicionar propriedade
|UC06|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição| O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> adiciona <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>  |
|Ator| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet |
|Ação| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> adicionar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
|Fluxo principal| **FP01:** Fluxo de adicionar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica em adicionar nova <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 5. Ator registra informações da <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
|Pós-condições| O ator baixado um pdf com todas as informações da <a href="/requisitos/modelagem/lexicos#cardeneta_de_campo">caderneta de campo</a> |
|Data de criação| 17/02/2022 |

### UC07 Alterar propriedade
|UC07|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> altera <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>|
|Ator|<a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet, e <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> criada |
|Ação|<a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> alterar conta |
|Fluxo principal| **FP01:** Fluxo de alterar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica no ícone de alterar <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 5. Ator altera informações da <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
|Pós-condições|Ator alterou informações da propriedade|
|Data de criação|17/02/2022|

### UC08 Remover propriedade
|UC08|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição|O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> remover <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a>|
|Ator|<a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet, e <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> criada |
|Ação|<a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> alterar conta |
|Fluxo principal| **FP01:** Fluxo de remover <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica no ícone de remover <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> |
|Pós-condições|Ator removeu propriedade|
|Data de criação|17/02/2022|

### UC09 Adicionar talhão
|UC09|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição| O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> adiciona <a href="/requisitos/modelagem/lexicos#talhao">talhão</a>  |
|Ator| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet |
|Ação| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> adicionar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Fluxo principal| **FP01:** Fluxo de adicionar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica em uma <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 5. Ator clica em adicionar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Pós-condições| <a href="/requisitos/modelagem/lexicos#talhao">Talhão</a> adicionado na propriedade |
|Data de criação| 17/02/2022 |

### UC10 Visualizar talhão
|UC10|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição| O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> visualiza <a href="/requisitos/modelagem/lexicos#talhao">talhão</a>  |
|Ator| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet, ter <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> cadastrado |
|Ação| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> visualizar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Fluxo principal| **FP01:** Fluxo de visualizar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica em uma <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 5. Ator clica em visualizar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Pós-condições| <a href="/requisitos/modelagem/lexicos#talhao">Talhão</a> visualizar na propriedade |
|Data de criação| 17/02/2022 |

### UC11 Alterar talhão
|UC11|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição| O <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> altera <a href="/requisitos/modelagem/lexicos#talhao">talhão</a>  |
|Ator| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a>|
|Pré-Condições| Ter conta como <a href="/requisitos/modelagem/lexicos#produtor">produtor</a> criada no aplicativo, acesso a internet, ter <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> cadastrado |
|Ação| <a href="/requisitos/modelagem/lexicos#produtor">Produtor</a> alterar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Fluxo principal| **FP01:** Fluxo de alterar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> <br/> 1. Ator entra no aplicativo <br/> 2. Ator conecta na sua conta <br/> 3. Ator clica em Minhas <a href="/requisitos/modelagem/lexicos#propriedade">propriedades</a> <br/> 4. Ator clica em uma <a href="/requisitos/modelagem/lexicos#propriedade">propriedade</a> <br/> 5. Ator clica no ícone de alterar <a href="/requisitos/modelagem/lexicos#talhao">talhão</a> |
|Pós-condições| <a href="/requisitos/modelagem/lexicos#talhao">Talhão</a> alterado na propriedade |
|Data de criação| 17/02/2022 |

### UC12 Remover talhão
|UC12|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC13 Adicionar plantação
|UC13|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC14 Visualizar plantações colhidas
|UC15|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC16 Visualizar plantação
|UC16|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC17 Registrar aplicação de agrotóxico
|UC17|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC18 Alterar plantação
|UC18|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC19 Marcar plantação como colhida
|UC19|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC20 Remover plantação
|UC20|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC21 Visualizar caderneta de campo
|UC21|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC22 Solicitar alteração na caderneta de campo
|UC22|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC23 Desassociar de uma propriedade
|UC23|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### U24 Se associar a uma propriedade
|UC24|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC25 Informar período de carência
|UC25|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC26 Cadastrar agrotóxico
|UC26|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

### UC27 Remover agrotóxico
|UC27|Informações|
|:------:|:----:|:---------:|:---------:|
|Descrição||
|Ator||
|Pré-Condições||
|Ação||
|Fluxo principal||
|Pós-condições||
|Data de criação||

## 5. Referências

> [1] **Diagrama de caso de uso UML: O que é, como fazer e exemplos**. Lucidchart. Disponível em: <a href="https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml" target="_blanck">https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml</a>. Acesso em: 16/02/2022.

> [2] **Casos de uso**. Disponível em: <a href="https://requisitos-de-software.github.io/2021.1-Ingresso.com/modelagem/use_case/#3-diagrama-de-casos-de-uso" target="_blanck">https://requisitos-de-software.github.io/2021.1-Ingresso.com/modelagem/use_case/#3-diagrama-de-casos-de-uso</a>. Acesso em: 17/02/2022.
