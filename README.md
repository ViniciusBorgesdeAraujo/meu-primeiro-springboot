# Meu Primeiro Projeto Spring Boot 🚀

Este é um projeto de API RESTful desenvolvido com **Spring Boot**. Ele fornece funcionalidades básicas de autenticação, gerenciamento de produtos e mensagens. O projeto foi criado com o objetivo de praticar e consolidar conhecimentos em Java, Spring Security, JWT, JPA e REST APIs.

## 📁 Estrutura do Projeto

```

src
└── main
├── java/com/example/meu\_primeiro\_springboot
│   ├── controller
│   │   ├── AuthController.java
│   │   ├── MensagemController.java
│   │   └── ProdutoController.java
│   ├── exceptions
│   │   ├── GlobalExceptionHandler.java
│   │   └── RecursoNaoEncontradoException.java
│   ├── model
│   │   ├── Produto.java
│   │   └── Usuario.java
│   ├── repository
│   │   ├── ProdutoRepository.java
│   │   ├── UsuarioRepository.java
│   │   └── MensagemRepository.java
│   ├── security
│   │   ├── JwtAuthFilter.java
│   │   ├── JwtUtil.java
│   │   └── SecurityConfig.java
│   ├── service
│   │   ├── ProdutoService.java
│   │   ├── UsuarioService.java
│   │   ├── UsuarioDetailsService.java
│   │   └── MensagemService.java
│   ├── HelloController.java
│   └── MeuPrimeiroSpringbootApplication.java
└── resources

````

## ✅ Funcionalidades

- 🔐 Autenticação com JWT
- 👤 Cadastro e login de usuários
- 📦 CRUD de produtos
- 💬 Envio e listagem de mensagens
- ❌ Tratamento global de exceções

## 🛠️ Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3**
- **Spring Security**
- **JWT (JSON Web Token)**
- **Spring Data JPA**
- **H2 / MySQL** (dependendo da sua configuração)
- **Maven**

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/ViniciusBorgesdeAraujo/meu-primeiro-springboot


2. Navegue até a pasta do projeto:

   ```bash
   cd meu-primeiro-springboot
   ```
3. Execute o projeto:

   ```bash
   ./mvnw spring-boot:run
   ```
4. Acesse a API:

   * Local: `http://localhost:8080`

## 🔑 Endpoints principais

| Método | Endpoint      | Descrição                         |
| ------ | ------------- | --------------------------------- |
| POST   | `/auth/login` | Autentica usuário e retorna token |
| GET    | `/produtos`   | Lista todos os produtos           |
| POST   | `/produtos`   | Cria um novo produto              |
| GET    | `/mensagens`  | Lista mensagens                   |
| POST   | `/mensagens`  | Envia uma nova mensagem           |

## 🧪 Testes

O projeto contém testes básicos na pasta:

```
src/test/java/com/example/meu_primeiro_springboot
```

Execute os testes com:

```bash
./mvnw test
```

## 📌 Observações

* Certifique-se de configurar seu banco de dados no `application.properties`.
* Você pode trocar o banco H2 por outro como MySQL, PostgreSQL etc.

---

