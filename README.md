<h1 align="center">
  🏥 Sistema de Clínica com Spring Security
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=spring-security&logoColor=white" alt="Spring Security" />
  <img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Thymeleaf-005C84?style=for-the-badge&logo=thymeleaf&logoColor=white" alt="Thymeleaf" />
</p>

<p align="center">
  <strong>Uma aplicação robusta dedicada ao gerenciamento de serviços e rotinas clínicas, construída sobre o ecossistema Spring Boot com forte ênfase em segurança e controle de acessos.</strong>
</p>

<hr>

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Contato](#-contato)

## 💻 Sobre o Projeto

O **Clínica Spring Security** foi desenvolvido para simular e solucionar os desafios modernos de um ambiente clínico, focando rigorosamente na integridade dos dados, autorização e autenticação exigidas no mundo corporativo (Java Enterprise). 

Este projeto mostra o uso avançado do **Spring Security** para lidar com hierarquias de usuários, restrição de acesso em views (Thymeleaf Sec) e bloqueio forte de rotas web, apresentando-se como um excelente portfólio de domínio em segurança para arquiteturas monolíticas Java.

## ✨ Funcionalidades Principais

- **Autenticação e Autorização Segura:** Login criptografado usando BCrypt e sessões protegidas usando Spring Security completo.
- **Gestão de Roles (Hierarquias):** Controle de acesso baseado em papéis (ex: Médico, Recepcionista, Admin). O sistema impede nativamente ações onde o usuário logado não detém privilégios adequados, tanto no back-end (rotas) quanto front-end (elementos da interface).
- **Painel Responsivo e Limpo:** Layouts elegantes unindo Thymeleaf com Bootstrap 4 para a renderização do HTML partilhado (*layout dialect*).
- **Experiência com AJAX Dinâmico:** Diversas interações (pesquisas, paginação ou desbloqueios de tela) valem-se de chamadas AJAX via jQuery, impedindo os *reloads* constantes de tela.
- **Notificações por Email:** Disparos de envio de correio (JavaMail API) para rotinas comuns, por exemplo: aprovação de processos ou redefinição de senhas.
- **Persistência Completa:** Gestão robusta sobre banco de dados MySQL, operado por JPA, estruturando entidades e chaves relacionais coerentes ao negócio clínico.

## 🛠 Tecnologias Utilizadas

O backend e integração com front-end utilizam:

* **Linguagem:** [Java 14](https://www.oracle.com/java/)
* **Core & APIs Web:** [Spring Boot 2.3](https://spring.io/projects/spring-boot) (Spring MVC, Spring Data JPA, Spring Mail)
* **Controle de Acessos:** [Spring Security](https://spring.io/projects/spring-security) (incluindo dialect extension pro Thymeleaf)
* **Banco de Dados:** [MySQL](https://www.mysql.com/)
* **View/Frontend:** [Thymeleaf](https://www.thymeleaf.org/), HTML5, Bootstrap 4, jQuery e WebJars.
* **Gerenciador de Dependências:** Maven

## 📂 Arquitetura Central

O sistema apoia-se em camadas rigorosamente distintas pela abordagem **MVC (Model-View-Controller)**:
- **Models / Entities:** Mapeamento de tabelas DB, validações internas.
- **Repositories & Services:** Toda manipulação de persistência relacional e regras de negócio complexas de clínicas isoladas das requisições web.
- **Controllers:** Guiam a navegação da plataforma lidando puramente com requisições HTTP RESTful ou endpoints HTML.
- **Security Configs:** Centralização lógica via `WebSecurityConfigurerAdapter`, onde regras de *ant-matching* mapeiam as restrições hierárquicas.

## 🚀 Como Executar o Projeto

### Pré-requisitos
Você precisa ter no mínimo o [Java JDK 14](https://www.oracle.com/java/technologies/javase-downloads.html) configurado, [MySQL](https://www.mysql.com/downloads/) em operação (na porta padrão 3306), o [Git](https://git-scm.com/) e sua IDE preferida.

### Instalação e Testes

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/kauaxp77/Clinica-Spring.git
   ```

2. **Configuração do Banco de Dados:**
   - Como primeiro passo, crie um _schema_ de banco de dados compatível no seu MySQL.
   - Execute o script `script-mysql.sql` (disponível na raiz). Esse script criará as tabelas vitais e populará usuários "teste" baseados nas hierarquias de rotina.
   
3. **Conexões do Projeto:**
   - Acesse `src/main/resources/application.properties` com as propriedades da aplicação.
   - Altere `spring.datasource.username` e `spring.datasource.password` para o respectivo usuário master do seu MySQL local.

4. **Start da Aplicação:**
   - Dê um _update maven_ no projeto usando sua IDE e aguarde os downloads estáticos (WebJars) e do Maven.
   - Execute por meio da classe inicial do Spring Boot e acesse remotamente ou local em `http://localhost:8080`.

## 👨‍💻 Autor

Criado e mantido por:

* **Nome:** Wendeson Kauã 
* **Email:** Wendesonkaua11@gmail.com
* **GitHub:** [@kauaxp77](https://github.com/kauaxp77)
* **LinkedIn:** [Acesse para me contatar](https://www.linkedin.com/in/wendesonsnts/) 
