# Hello World - Java, Quarkus, JUnit 5, RestAssured

## Sobre o Projeto

O **Hello World** é um projeto básico criado para demonstrar o uso do **Quarkus** como framework para desenvolvimento de aplicações Java modernas. Este projeto inclui testes automatizados utilizando **JUnit 5** e **RestAssured** para validação de endpoints RESTful.

---

## Tecnologias Utilizadas

- **Java**: Linguagem principal de desenvolvimento.
- **Quarkus**: Framework Java para aplicações nativas em nuvem e de alto desempenho.
- **JUnit 5**: Framework de testes para Java.
- **RestAssured**: Biblioteca para testes de APIs RESTful.

---

## Funcionalidades

- **Endpoint de Teste**: Um endpoint simples para retornar "Hello, World!".
- **Testes Automatizados**: Verifica o funcionamento correto do endpoint usando JUnit 5 e RestAssured.

---

## Pré-requisitos

- **Java 11 ou superior**
- **Maven** (versão 3.8+)
- **Quarkus CLI** (opcional, mas recomendado)

---

## Como Executar o Projeto

### 1. Clone o Repositório
```bash
git clone https://github.com/samuelbaldasso/Hello-World-Quarkus-JUnit5-RestAssured.git
```

### 2. Navegue para o Diretório do Projeto
```bash
cd Hello-World-Quarkus-JUnit5-RestAssured
```

### 3. Execute o Projeto
#### Com Maven:
```bash
mvn quarkus:dev
```

#### Com Quarkus CLI:
```bash
quarkus dev
```

A aplicação estará disponível em `http://localhost:8080`.

---

## Testando o Projeto

### Executar Testes Automatizados

```bash
mvn test
```

Os testes verificarão se o endpoint retorna a resposta esperada.

---

## Estrutura do Projeto

```plaintext
Hello-World-Quarkus/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/helloworld/
│   │   │       ├── GreetingResource.java   # Endpoint principal
│   │   │       └── application.properties  # Configurações da aplicação
│   │   └── resources/
│   │       └── META-INF/
│   │           └── resources/
│   │               └── index.html          # Página inicial (opcional)
│   └── test/
│       └── java/
│           └── com/example/helloworld/
│               ├── GreetingResourceTest.java # Testes unitários
│               └── NativeGreetingIT.java     # Testes nativos (GraalVM)
├── pom.xml                                 # Configuração do Maven
└── README.md                               # Documentação
```

---

## Próximos Passos

- Adicionar suporte para endpoints adicionais e lógica de negócios.
- Configurar integração com banco de dados (ex.: Panache, Hibernate).
- Explorar a criação de imagens nativas com GraalVM.

---

## Contribuindo

Contribuições são sempre bem-vindas! Para colaborar:

1. Faça um fork do repositório.
2. Crie uma branch para a sua feature (`git checkout -b minha-feature`).
3. Commit suas alterações (`git commit -m 'Adiciona minha feature'`).
4. Envie para o repositório remoto (`git push origin minha-feature`).
5. Abra um Pull Request.

---

## Licença

Este projeto está licenciado sob a [MIT License](./LICENSE).
