# 🥦 MHK System — Backend

Sistema de pedidos para conectar fornecedores (produtores) e clientes no setor de hortifrúti, permitindo venda direta de produtos frescos, como frutas, legumes e hortaliças.

---

## 📌 Objetivo

O **MHK System** tem como propósito facilitar a comunicação entre produtores e consumidores, oferecendo uma plataforma simples e eficiente para:

- Fornecedores cadastrarem produtos
- Clientes visualizarem e realizarem pedidos
- Acompanhamento do status do pedido (do envio à entrega)

---

## ⚙️ Tecnologias Utilizadas

- **Java 17+**
- **Spring Boot 3.x**
  - Spring Web
  - Spring Data JPA
  - Spring Security
- **PostgreSQL**
- **Maven**
- **Lombok**

---

## 🏗️ Como rodar o projeto localmente

### ✅ Pré-requisitos

- Java 17+
- PostgreSQL instalado
- Maven
- Git

## 🧱 Configuração do banco de dados + ▶️ Rodando a aplicação

1. **Crie o banco de dados no PostgreSQL:**

```sql
CREATE DATABASE maisHortaKilo;
```

2. **Configure a conexão com o banco no arquivo `application.properties`:**

#### 📁 `src/main/resources/application.properties`

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/maisHortaKilo
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
```

> Substitua `seu_usuario` e `sua_senha` conforme sua instalação local do PostgreSQL.

3. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/mhk-backend.git
cd mhk-backend
```

4. **Execute a aplicação:**

Se estiver usando o Maven Wrapper:

```bash
./mvnw spring-boot:run
```

Ou, com Maven instalado globalmente:

```bash
mvn spring-boot:run
```

5. **Acesse a aplicação no navegador ou via Postman:**

```
http://localhost:8080
```

---
