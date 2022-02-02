# Política de Contribuição

## Versionamento
| Versão | Data | Modificação | Autor |
|--|--|--|--|
|1.0| 29/01/2022| Criação do documento | João Pedro Moura |

## Políticas de Branch para o repositório Doc
<p style="text-align: justify; text-indent: 20px">As branches serão nomeadas seguindo um padrão para a melhor organização do projeto. Por se tratar de um projeto baseado em documentos, terá apenas um tipo de nomenclatura de branch. Todas as branchs devem ser criadas a partir da <b>master</b> e devem estar nomeadas da seguinte maneira:</p>

``` 
X-Nome_Documento 
Exemplo: 4-Política_de_Contribuição
```

<p style="text-align: justify; text-indent: 20px"> Sendo X o número da issue atribuída seguido pelo nome do documento, como destacado anteriormente. Em ocasiões em que não se está trabalhando com nenhum documento em específico, então deve-se colocar o nome da issue correspondente.</p>

## Políticas de Branch para os repositórios Dev
<p style="text-align: justify; text-indent: 20px"> Ao contrário do repositório Doc, as branchs dos repositórios Dev (Frontend e Backend) seguem o padrão GitFlow e devem ser derivadas da <b>develop</b>. A seguir existe uma explicação mais detalhada para cada branch:</p>

### Branch Master
<p style="text-align: justify; text-indent: 20px"> A branch master deverá conter todo código que se encontra em produção, ou seja, essa branch será a responsável por receber os commits derivados de cada release através de um merge.</p>
- Só existe uma branch <b>Master</b>.
- Commits não são permitidos diretamente nessa branch.
- Os commits devem ocorrer por pull requests das branchs <b>Develop</b> a cada release e <b>Bugfix</b>

### Branch Develop
<p style="text-align: justify; text-indent: 20px"> Similar a branch master, ela armazena o código principal do projeto, entretando para o ambiente de homologação. Ou seja, todo o código que se encontra nessa branch é o mais atualizado, podendo conter bugs e funcionalidades ainda em desenvolvimento.</p>
- Só existe uma branch <b>Develop</b>.
- Commits não são permitidos diretamente nessa branch.
- Os commits devem ocorrer por pull requests das branchs individuais <b>Feauture</b> e <b>Hotfix</b>

### Branchs Feauture
<p style="text-align: justify; text-indent: 20px"> Branchs individuais em que cada desenvolvedor deverá estar trabalhando. Focada na adição de novas funcionalidades que estaram presentes na branch develop.</p>
- Existem diversas branchs <b>Feauture</b>.
- Commits diretos devem ser feitos nessas branchs.
- Derivadas da <b>Develop</b>.
- Devem sempre ser devolvidas para a <b>Develop</b>.
- Formato: `feature/numeroIssue-nome_feature`

### Branchs Hotfix
<p style="text-align: justify; text-indent: 20px"> Branchs individuais para que os desenvolveldores resolvam bugs e erros urgentes presentes na branch <b>Develop</b></p>
- Existem diversas branchs <b>Hotfix</b>.
- Commits diretos devem ser feitos nessas branchs.
- Derivadas da <b>Develop</b>.
- Não necessitam de reviews
- Formato: `hotfix/numeroIssue-nome_feature`

### Branchs Bugfix
<p style="text-align: justify; text-indent: 20px"> Branchs individuais para que os desenvolveldores resolvam bugs e erros urgentes presentes na branch <b>Master</b></p>
- Raramente devem existir branchs <b>Bugfix</b>.
- Commits diretos devem ser feitos nessas branchs.
- Derivadas da <b>Master</b>.
- Formato: `bugfix/numeroIssue-nome_bug`

## Políticas de Commits
<p style="text-align: justify; text-indent: 20px">Os commits devem ser feitos de maneira clara e objetiva respeitando os padrões comentados a seguir: </p>

<ul>
    <li> Devem estar escritos em português. </li>
    <li> Os verbos devem estar no gerúndio. </li>
    <li> Devem apresentar o número base da issue. </li>
</ul>

&emsp;&emsp;Portanto a formatação do commit será: ` #4 Corrigindo documento de planejamento `
<p style="text-align: justify; text-indent: 20px">Vale a pena lembrar que é possível utilizar o seguinte Hook já configurado para esse repositório, que acrescentará automaticamente o número da Branch em seu commit:</p>
```bash
#!/bin/sh
BRANCH=$(git branch | grep "*" | sed 's/* \([0-9]*\)-.*/#\1/')
TEXT=$(cat "$1" | sed '/^#.*/d')

if [ -z "$BRANCH" ]
then
    echo "Branch não esta no formato NUMERO-TITULO_ISSUE."
fi

if [ -n "$TEXT" ]
then
    echo "$BRANCH" "$TEXT" > $1
else
    echo "Commit sem mensagem."
    exit 1
fi
```

<p style="text-align: justify; text-indent: 20px"> E por fim, nas ocasiões em que o commit for realizado por duas ou mais pessoas, deve ser acrescentado à mensagem do commit o seguinte texto: </p>

```
#4 Corrigindo documento de planejamento


Co-authored-by: Fábio Silva <fabiosilva@gmail.com>
```
