# Aplicação Grasp

## 1. Versionamento

| Versão | Data       | Descrição                                  | Autor(es)                 |
| ------ | ---------- | ------------------------------------------ | ------------------------- |
| 1.0    | 17/03/2022 | Abertura do documento                      | Carlos e Paulo            |


## 2. Introdução

<p align="justify" style="text-indent: 20px">Após estudo dos padrões GRASP(s), iremos demonstrar sua aplicação na <a href="../../modelagem/estatica/diagrama_de_pacotes.md" target="_blank">modelagem</a> do projeto. </p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px">Como forma de manter maior coesão e consequentemente a realização de um melhor trabalho, os participantes se reuniram em chamada de voz e realizaram a aplicação dos padrões GRASP(s) em alguns artefatos específicos da modelagem.</p>

## 4. GRASP(s)

### 4.1 Coesão

### 4.2 Controlador

<p align="justify" style="text-indent: 20px"> Através dos nossos estudos indentificamos que o Controlador é responsável por receber e lidar com um evento do sistema, ou seja, tem como responsabilidade coordenar todos os procedimentos solicitados pelo usuário e identificar os responsáveis por tais tarefas. A partir disso, analisando o nosso diagrama de pacotes podemos identificar a utilização desse princípio.</p>

<p align="justify" style="text-indent: 20px">No nosso projeto os controllers são responsaveis por acessar as "services" e estabelecer a lógica referente a cada página, informando esses dados para as "pages". A seguir está apresentado a imagem referente à modelagem de pacotes, onde podemos ver a controller. </p>

<center>
<img src="../../../assets/padroes_projetos/aplicacao_controlador_grasps.png" class="zoom"> 
<h6>Figura 2: Aplicação Controller</h6>
<h6>Fonte: Autores.</h6>
</center>

### 4.3 Criador

<p align="justify" style="text-indent: 20px">A partir do diagrama de classes é notado o uso do padrão GRASP criador, onde a classe "Produtor" é a responsável pela criação de instâncias do objeto "Propriedade". Aplicando o questionamento usado no <a>estudo</a>, temos que:</p>

- Produtor "possui" Propriedade.
- Produtor registra Propriedade.
- Produtor possui dados iniciais de Propriedade, que são passados assim que Propriedade é criada.

<p align="justify" style="text-indent: 20px">Na figura abaixo é visível que o método </p>

```
adiciona_propriedade()
```

<p align="justify" style="text-indent: 20px"> seria o responsável pela criação. </p>

<center>
<img src="../../../assets/padroes_projetos/aplicacao_criador_grasps.png" class="zoom"> 
<h6>Figura 3: Aplicação Criador</h6>
<h6>Fonte: Autores</h6>
</center>
