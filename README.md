# Sistema de Verificação de Usuário

Este repositório contém um exemplo de código para realizar a verificação de credenciais de usuário em um banco de dados. Ele inclui uma classe Java chamada `User`, que implementa métodos para estabelecer conexão com o banco de dados e validar usuários.

## Estrutura do Código

O projeto possui as seguintes funcionalidades principais:

### 1. **Conexão com o Banco de Dados**
O método `conectarBD()` é responsável por:
- Estabelecer uma conexão com o banco de dados MySQL.
- Carregar o driver do banco de dados.
- Retornar um objeto `Connection` que pode ser utilizado para executar consultas.

### 2. **Verificação de Usuários**
O método `verificarUsuario(String login, String senha)`:
- Recebe o login e a senha como parâmetros.
- Constrói uma consulta SQL para buscar o usuário correspondente no banco de dados.
- Retorna `true` se o usuário for encontrado e `false` caso contrário.

## Principais Pontos do Código

- **Entrada:** Login e senha do usuário.
- **Processo:** Conexão com o banco de dados, construção e execução da consulta SQL.
- **Saída:** Um valor booleano indicando se o usuário foi encontrado.

## Requisitos para Execução

- **Ambiente:** 
  - Java Development Kit (JDK) 8 ou superior.
  - Banco de dados MySQL instalado e configurado.
  
- **Dependências:**
  - Biblioteca do driver JDBC para MySQL (`com.mysql.DriverManager`).
  - Credenciais de acesso ao banco de dados (atualmente configuradas no código).

## Configuração do Ambiente

1. Certifique-se de que o banco de dados MySQL está rodando.
2. Crie um banco de dados chamado `test` com uma tabela chamada `usuarios`:
    ```sql
    CREATE DATABASE test;
    USE test;

    CREATE TABLE usuarios (
        id INT AUTO_INCREMENT PRIMARY KEY,
        nome VARCHAR(100),
        login VARCHAR(50),
        senha VARCHAR(50)
    );
    ```
3. Insira dados de teste na tabela:
    ```sql
    INSERT INTO usuarios (nome, login, senha) VALUES
    ('João Silva', 'joao', '1234'),
    ('Maria Oliveira', 'maria', 'abcd');
    ```

4. Certifique-se de que as credenciais de acesso ao banco de dados no código (`user`, `password`) estão corretas.
