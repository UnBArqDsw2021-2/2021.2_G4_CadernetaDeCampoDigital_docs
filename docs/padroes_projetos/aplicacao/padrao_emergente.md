# Aplicação Padrões Emergentes

## 1. Versionamento

| Versão | Data       | Descrição                   | Autor(es)                 |
| ------ | ---------- | --------------------------- | ------------------------- |
| 1.0    | 17/03/2022 | Abertura do documento       | Denniel e Thiago |
| 1.1    | 18/03/2022 | Padrões emergentes e exemplos com projeto      | Denniel e Thiago |


## 2. Introdução

<p align="justify" style="text-indent: 20px"></p>

## 3. Metodologia

<p align="justify" style="text-indent: 20px"></p>

## 4. Padrões Emergentes

### 4.1 <i>Rest</i>

<p align="justify" style="text-indent: 20px">O padrão REST, Representational State Transfer (Transferência de Estado Representacional), define a padronização de rotas, requisições e comunicações sem estado, também conhecido como protocolo HTTP. Sendo assim, uma API que utiliza essa padronização e que possui inteligência para aplicá-la é denominada de RESTful. [1]</p>

<p align="justify" style="text-indent: 20px">Existem 4 princípios principais do REST: [2]</p>

- **Client-Server (Cliente-Servidor):** Sempre há um cliente e um servidor e esses dois sistemas precisam de limites para o funcionamento.
- **Stateless (Sem estado):** Os servidores precisam ser capazes de processar as mensagens que recebem. Para fazer isso, cada solicitação que um servidor receber deve ter as informações necessárias para que o servidor funcione.
- **Uniform Interface (Interface Uniforme):** O uso de terminologia e recursos semelhantes ajuda a padronizar as APIs. De acordo com o princípio, os seguintes verbos HTTP são usados: GET, PUT, POST,DELETE. Os recursos sempre se referem a URIs (identificador uniforme de recursos). As respostas HTTP sempre vêm com um status e um corpo.
- **Cacheable (Armazenável com cache):** Os clientes precisam ser capazes de armazenar em cache as representações. Devido à ausência de estado (toda representação sendo autodescritiva), isso é possível em uma API RESTful.

<p align="justify" style="text-indent: 20px">Sendo assim, o diagrama abaixo demonstra a comunicação e estrutura que está sendo utilizada e como o Django-Rest se aplica nesse processo. </p>

<p align="justify" style="text-indent: 20px">Assim como mostrado no esquema abaixo, temos o flutter como client principal do nosso sistema, sendo que, através do Django-Rest foi desenvolvida a api RESTful do nosso projeto. A transmissão entre client e REST API é feita inicialmente através de um JSON, mas o XML também pode ser necessário a medida que forem aparecendo dados mais complexos a ser transmitidos.</p>

<center>
  <img src="../../../assets/padroes_projetos/api_rest_django.svg" class="zoom">
  <h6 align = "center">Figura 1: API REST Model</h6>
  <h6 align = "center">Fonte: Autores</h6>
</center>

<p align="justify" style="text-indent: 20px">A imagem abaixo demonstra os verbos de uma API REST implementado no sistema do projeto, em que no caso demonstrado é um JSON com os dados do técnico do projeto.</p>

<center>
  <img src="../../../assets/padroes_projetos/exemplo_django_rest.png" width="800" class="zoom"/>
  <h6 align = "center">Figura 2: Exemplo API REST - Backend </h6>
  <h6 align = "center">Fonte: Autores</h6>
</center>

<p align="justify" style="text-indent: 20px">A imagem abaixo procura mostrar, com o projeto, como é feita a comunicação entre client e API REST no projeto, em que através do Dio e pelos verbos HTTP foi utilizado um POST para conseguir passar as informações registradas no client para a nossa api, sendo a imagem acima o retorno ao ser concluído o verbo. </p>

<center>
  <img src="../../../assets/padroes_projetos/rest_post_tecnico.png" width="800" class="zoom"/>
  <h6 align = "center">Figura 3: Exemplo comunicação Client - API REST</h6>
  <h6 align = "center">Fonte: Autores</h6>
</center>


## 5. Referências

> [1] **Design de API Rest**. Design de API Rest. Disponível em: <a href="https://wssilva-willian.medium.com/design-de-api-rest-9807a5b16c9f" >Design de API Rest</a>. Acesso em: 25 de fev. de 2022.

> [2] **What Is the Difference Between REST and RESTful APIs?**. What Is the Difference Between REST and RESTful APIs?. Disponível em: <a href="https://blog.devmountain.com/what-is-the-difference-between-rest-and-restful-apis" >Django MVT</a>. Acesso em: 27 de fev. de 2022.