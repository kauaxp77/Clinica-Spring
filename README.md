<h1 align="center">
  Sistema de Clínica com Spring Security
</h1>

<p align="center">
  <strong>Uma aplicação Java dedicada para o gerenciamento de serviços e rotinas clínicas utilizando o ecossistema Spring.</strong>
</p>

## 💻 Sobre o Projeto

O Projeto Clínica Spring Security foi desenvolvido com o foco em solidificar conhecimentos avançados de ecossistema Java orientados à Web e, principalmente, às camadas de segurança providas pelo Spring Security. 

O sistema simula as transações de gerenciamento interno de uma clínica, onde a integridade dos dados e as premissas de autorização (quem pode ver o que) são tratadas usando as mais rigorosas abordagens do Java Enterprise moderno.

## 🚀 Tecnologias Aplicadas

As ferramentas envolvidas nesse backend focam em segurança, consistência e persistência:

- **Java JDK**
- **Spring MVC** para o estruturação do painel de controle e direcionamentos
- **Spring Security** (Autenticação, Autorização e Sessões)
- **Spring Data / Hibernate (JPA)** persistência relacional com o banco de dados.
- **MySQL**
- Injeção de Dependências
- **API JavaMail** para disparo de serviços de notificação interna.
- O Frontend é construído usando abordagens JSP e dinâmicas com **jQuery** e **AJAX**.

## 📈 Features e Aprendizado

- **Gestão de Roles (Hierarquias):** Criação de escopos de usuários. Impedir que um funcionário sem permissão acesse rotas exclusivas do gestor através de anotações e WebSecurity.
- **Desbloqueios Dinâmicos (AJAX):** Várias telas do frontend utilizam AJAX garantindo a performance da aplicação e menor número de _reloads_ na tela.
- **Arquitetura em MVC:** Divisão limpa e elegante entre as Models (entidades), Controllers (agentes lógicos) e as Views.

## 🛠️ Setup Localmente

1. Tenha uma instância do MySQL rodando em sua máquina e faça o _dump_ (Crie e popule com o código via script).
2. Configure as propriedades para o MySQL apontarem na sua instalação em _application.properties_ (ou outro XML de persistência local).
3. Importe o projeto no seu editor (Spring Tools Suite / IntelliJ / Eclipse).
4. Utilize o banco padrão para se logar no sistema. O script de banco inicial já provê o usuário teste.
