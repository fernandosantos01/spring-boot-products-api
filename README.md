
# 📜API RESTful de Produtos com SpringBoot 3

O projeto implementa um CRUD (Create, Read, Update, Delete) completo, seguindo as melhores práticas de desenvolvimento de APIs, incluindo o uso de DTOs, validações e os princípios do Modelo de Maturidade de Richardson, incluindo HATEOAS para a navegabilidade entre os recursos.


## ✨Funcionalidades

- Cadastro de Produtos: Criação de novos produtos com nome e valor.
- Listagem de Produtos: Visualização de todos os produtos cadastrados.
- Busca de Produto por ID: Detalhamento de um produto específico.

- Atualização de Produtos: Alteração dos dados de um produto existente.

- Exclusão de Produtos: Remoção de um produto do sistema.

- Validação de Dados: Garante que os dados enviados para a API sejam válidos.

- Suporte a HATEOAS: Links para navegação entre os recursos da API.


## 🛠️Stack utilizada

**Java 17:** Versão LTS mais recente da linguagem Java.

**Spring Boot 3.1.0:** Framework principal para a criação da aplicação.

**Spring Web:** Para a criação de endpoints RESTful.

**Spring Data JPA:** Para a persistência de dados de forma simplificada.

**Hibernate:** Implementação da especificação JPA para o mapeamento objeto-relacional.

**Spring HATEOAS:** Para a implementação de hipermídia nos retornos da API.

**Bean Validation:** Para a validação dos dados de entrada.

**Maven:** Gerenciador de dependências do projeto.

**PostgreSQL:** Banco de dados relacional para armazenamento dos dados.


## 🚀 Como Executar o Projeto

Siga os passos abaixo para executar o projeto em seu ambiente local.

Pré-requisitos
Antes de começar, você vai precisar ter instalado em sua máquina:

**JDK 17**

**Maven**

**PostgreSQL**

Um cliente de API, como o **Postman** ou **Insomnia**.


1. **Clonando o Repositório**

```bash
  git clone https://github.com/seu-usuario/seu-repositorio.git
  cd seu-repositorio
```
2. **Configurando o Banco de Dados**
Abra o seu cliente PostgreSQL (como o pgAdmin).

Crie uma nova base de dados. No tutorial, ela foi nomeada `products-api`.

3. **Configurando a Aplicação**
Abra o arquivo `src/main/resources/application.properties`.

Altere as propriedades `spring.datasource.username` e `spring.datasource.password` com suas credenciais do PostgreSQL.
```Properties
spring.datasource.url=jdbc:postgresql://localhost:5432/products-api
spring.datasource.username=seu-usuario-aqui
spring.datasource.password=sua-senha-aqui

spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
```
