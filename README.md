# Desafio Java - Spring

O Desafio é bem simples, vou solicitar técnicas não muito avançadas mas que darão a entender como funcionaremos na criação das próximas Api's Rest.

## Avisos antes de começar

- Crie um repositório no seu GitHub.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o meu email "patrick.tavares@idor.org".
- Fique à vontade para perguntar qualquer dúvida.

### Sobre o ambiente da aplicação:

- Java 17

- Spring Boot 3.1.4

- Maven

- Packing Jar

## Objetivo: Sistema simples de estoque

Teremos produtos em apenas um estoque, estes por sua vezes devem conter nome, código de barras, valor BR$ e quantidade. Os serviços que disponibilizaremos a partir dessa api é: Quando solicitado uma demanda de produtos, eles devem retornar o valor em dólar ( US$ ), e esse valor deve estar integrado à uma API que retorne em tempo real o câmbio dessa moeda.

Além disso, deve ser verificado se existem tais quantidades em estoque, para que o valor n se torne negativo no estoque, senão, deve entrar em uma Exception já tratada que retorne a quantidade de itens faltantes.

### Payload

O Payload fica à seu critério como deve trazê-lo, mas segue um exemplo:

POST /demanda

```json
{
    "id_product" : 3,
    "qntdd" : 4,
    "US$" : 3500.00
}
```
###Pontos importantes:

- Atenção aos packages do projeto.

- Escolha de arquitetura clara.

- Atenção aos endpoints de uma API Restful.

- Integração com banco de dados de sua escolha.

- Recursos prioritários: Spring Data JPA, Lombok e Spring Web.

- Faz-se importante também uma documentação clara e objetiva que inclua o deploy, seja em Docker ou não de sua aplicação, mas recomendo o uso de docker =D

Boa sorte!
