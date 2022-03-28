# Reutilização Flutter

## 1. Versionamento

| Versão | Data       | Descrição                            | Autor(es)          |
| ------ | ---------- | -------------------------------------| -------------------|
| 1.0    | 27/03/2022 | Abertura do documento                | Paulo              |
| 1.1    | 27/03/2022 | Adição dos tópicos 2.1 e 2.2         | Paulo              | 
| 1.2    | 27/03/2022 | Adição dos tópico 3                  | Paulo              | 
| 1.3    | 27/03/2022 | Revisão por pares                    | Brenno e Carlos    |


## 2. Introdução
<p align="justify" style="text-indent: 20px"> Reutilização de software tem como ideia evitar retrabalho no desenvolvimento de um projeto, aproveitando de soluções previamente desenvolvidas e implementando em novos contextos. O objetivo principal do reuso é o aumento da produtividade e redução no esforço de desenvolver novos produtos. [1]</p>

<p align="justify" style="text-indent: 20px"> No framework flutter [2] podemos identificar a reutilização de software principalmente a partir de Widgets que, por meio de um relacionamento de composição, permitem ao desenvolvedor utilizar diversos elementos de UI pré definidos. Além do que o usuário pode criar widgets próprios, que podem ser adaptados de acordo com as necessidades da aplicação.</p>

### 2.1 <i>Hot Spots</i>

- Stateful Widgets
- Containers

### 2.2 <i>Frozen Spots</i>

- Stateless Widget
- Estruturação/Arquivos Fixos

## 3. Plugins

<p align="justify" style="text-indent: 20px"> Vale ressaltar também que utilizamos de alguns plugins, são bastante úteis, e acabam adicionando mais funções e recursos, facilitando o desenvolvimento e ajudaram a complementar nosso projeto. Estão listados alguns logo abaixo:</p>

- dio: O dio é um poderoso cliente HTTP para Dart, que suporta interceptores, configuração global, FormData, cancelamento de solicitação, download de arquivo, tempo limite, entre outras funcionalidades.
- dart_code_metrics: É uma ferramenta de análise estática que ajuda a analisar e melhorar a qualidade do código.
- flutter_test: Biblioteca de testes para flutter.
- cupertino_icons: É um repositório que contém o conjunto padrão de ícones usados ​​pelo Flutter Cupertino widgets.
- flutter_localizations: É um pacote que simplifica a tradução no aplicativo.
- cpf_cnpj_validator: Um plugin para validar CPF/CNPJ.
- intl: Fornece recursos de internacionalização e localização.
- flutter_svg: Desenha aquivos SVG em um widget.
- flutter_lints: Este pacote contém um conjunto recomendado de lints para a aplicação.

## 4. Referências

> [1] DevMedia **Reutilização de Software - Revista Engenharia de Software Magazine 39**. Disponivel em <a href= "https://www.devmedia.com.br/reutilizacao-de-software-revista-engenharia-de-software-magazine-39/21956">https://www.devmedia.com.br/reutilizacao-de-software-revista-engenharia-de-software-magazine-39/21956</a>  Acesso em 27 de mar. de 2022

> [2] Flutter **Documentação Flutter**. Disponivel em <a href= "https://flutter.dev/">https://flutter.dev/</a>  Acesso em 27 de mar. de 2022
