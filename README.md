# Explorando Padrões de Projetos na Prática com Java / Exploring Design Patterns in Java

Este README contém duas seções: Português (PT-BR) e English (EN). Cada seção descreve o propósito do projeto, requisitos, instruções de execução e detalhes do Spring usados.

---

Português (PT-BR)

Visão geral
Este repositório contém implementações e exemplos práticos de padrões de projeto aplicados em aplicações Java usando o Spring Framework. O objetivo é demonstrar como cada padrão pode ser estruturado e testado em um contexto real, com foco em clareza pedagógica.

Padrões implementados
- Singleton: controle de instância única para objetos de configuração/serviço quando apropriado.
- Strategy / Repository: separação de estratégias de negócio e abstração de acesso a dados via repositórios.
- Facade: fachada para agrupar operações complexas e expor uma API simplificada aos clientes.

Requisitos
- Java 17 (conforme propriedade <java.version> no pom.xml)
- Maven 3.6+
- IDE recomendada: IntelliJ IDEA, VS Code ou Eclipse

Sobre o Spring (detalhes do projeto)
- Spring Boot: 2.5.4
- Spring Cloud: 2020.0.3
- Dependências principais:
  - spring-boot-starter-web
  - spring-boot-starter-data-jpa
  - spring-cloud-starter-openfeign
  - springdoc-openapi-ui (v1.5.10)
  - H2 Database (runtime)

Dicas de configuração
- Configure application.properties ou application.yml em src/main/resources para porta, datasource e perfis.
- H2 Console (quando habilitado): /h2-console
- Swagger / OpenAPI UI (springdoc): /swagger-ui.html ou /swagger-ui/index.html
- Rodar em outra porta: -Dserver.port=8081 ou application.properties

Como executar
1. Clone o repositório:
   git clone <URL-do-repositório>
2. Entre na pasta do projeto:
   cd lab-padroes-projeto-spring-main
3. Build e execução (Maven):
   mvn clean package
   mvn spring-boot:run
   # ou: java -jar target/*.jar

Estrutura do projeto
- src/main/java: implementação dos padrões e classes de exemplo
- src/main/resources: arquivos de configuração
- src/test/java: testes automatizados
- pom.xml: dependências e versão do Spring Boot

Testes
Executar testes unitários:
  mvn test

Contribuição
- Abra uma issue para discutir mudanças maiores
- Faça fork e envie pull request com descrição clara
- Inclua testes e documentação para mudanças significativas

Licença
Adicionar informação de licença (ex: MIT) se aplicável.

Autor
Jackson Barbosa

---

English (EN)

Overview
This repository contains practical implementations and examples of design patterns applied in Java applications using the Spring Framework. It aims to show how each pattern can be structured and tested in a real-like context, focusing on clarity for learning.

Implemented patterns
- Singleton: control of a single instance for configuration/services when appropriate.
- Strategy / Repository: separation of business strategies and data-access abstraction via repositories.
- Facade: a facade to group complex operations and expose a simplified API to clients.

Requirements
- Java 17 (as set in the pom.xml <java.version>)
- Maven 3.6+
- Recommended IDE: IntelliJ IDEA, VS Code or Eclipse

About Spring (project details)
- Spring Boot: 2.5.4
- Spring Cloud: 2020.0.3
- Main dependencies:
  - spring-boot-starter-web
  - spring-boot-starter-data-jpa
  - spring-cloud-starter-openfeign
  - springdoc-openapi-ui (v1.5.10)
  - H2 Database (runtime)

Configuration tips
- Edit application.properties or application.yml in src/main/resources to change port, datasource and profiles.
- H2 Console (if enabled): /h2-console
- Swagger / OpenAPI UI (springdoc): /swagger-ui.html or /swagger-ui/index.html
- Run on different port: pass -Dserver.port=8081 or set in application properties.

How to run
1. Clone the repo:
   git clone <repository-URL>
2. Enter the project folder:
   cd lab-padroes-projeto-spring-main
3. Build and run (Maven):
   mvn clean package
   mvn spring-boot:run
   # or: java -jar target/*.jar

Project structure
- src/main/java: pattern implementations and example classes
- src/main/resources: configuration files
- src/test/java: automated tests
- pom.xml: dependencies and Spring Boot version

Tests
Run unit tests:
  mvn test

Contributing
- Open an issue to discuss larger changes
- Fork and send a pull request with a clear description
- Include tests and documentation for significant changes

License
Add license information (e.g., MIT) if applicable.

Author
Jackson Barbosa

Notes / Next steps
If you want, examples of application.properties, sample endpoints, screenshots of Swagger UI or a quickstart script can be added — say which you prefer and the README will be updated accordingly.
