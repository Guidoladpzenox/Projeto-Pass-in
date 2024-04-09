# **Passin** 📚

Passin é um sistema de gerenciamento de eventos e participantes, desenvolvido com Spring Boot.

## Funcionalidades Principais

- **Eventos:** Crie, atualize, visualize e exclua eventos.
- **Participantes:** Registre participantes em eventos e gerencie seus check-ins.
- **Geração de Crachás:** Gere crachás para os participantes dos eventos.

## Configuração do Projeto

### Requisitos

- Java JDK 8 ou superior
- Maven
- Banco de dados MySQL

### Configuração do Banco de Dados

1. Crie um banco de dados MySQL chamado `passin`.
2. Atualize as configurações de conexão com o banco de dados no arquivo `application.properties`.

```bash
spring.datasource.url=jdbc:mysql://localhost:3306/passin
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

Executando o Projeto

    Clone o repositório: git clone https://github.com/seu_usuario/passin.git
    Navegue até o diretório do projeto: cd passin
    Compile o projeto: mvn clean install
    Execute o projeto: java -jar target/passin.jar

O servidor estará em execução em http://localhost:8080.
Endpoints API

    GET /events/{id}: Retorna detalhes de um evento específico.
    POST /events: Cria um novo evento.
    POST /events/{eventId}/attendees: Registra um participante em um evento.
    GET /events/attendees/{id}: Retorna a lista de participantes de um evento.
    GET /attendees/{attendeeId}/badge: Retorna o crachá de um participante.
    POST /attendees/{attendeeId}/check-in: Registra o check-in de um participante.


Teste

Usado o insomnia  para realizar os testes de requisições e respostas dos Endpoints.

Link insomnia: https://insomnia.rest/download

Contribuindo

Sinta-se à vontade para enviar sugestões, relatar problemas ou contribuir com o desenvolvimento deste projeto.
