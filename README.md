# Repositório do MySQL com Docker Compose

Este repositório contém um arquivo `docker-compose.yml` que permite implantar um contêiner MySQL de maneira fácil e rápida. O Docker Compose simplifica o processo de configuração e execução de aplicativos em contêineres usando várias imagens Docker.

## Pré-requisitos

Certifique-se de ter o Docker e o Docker Compose instalados em seu sistema antes de prosseguir.

- Docker: [Instalação do Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Instalação do Docker Compose](https://docs.docker.com/compose/install/)

## Como usar

1. Clone este repositório para o seu sistema:

   ```shell
   git clone https://github.com/seu-usuario/mysql-docker.git
   ```

2. Acesse o diretório do repositório:

   ```shell
   cd mysql-docker
   ```

3. Abra o arquivo `docker-compose.yml` em um editor de texto e personalize as variáveis de ambiente, se necessário. Você pode definir a senha do root do MySQL, o nome do banco de dados e outras configurações no arquivo `docker-compose.yml`.

4. Inicie o contêiner do MySQL executando o seguinte comando:

   ```shell
   docker-compose up -d
   ```

   Isso criará e iniciará o contêiner MySQL em segundo plano.

5. Aguarde até que o contêiner seja iniciado e o serviço MySQL esteja pronto para aceitar conexões.

6. Agora você pode se conectar ao banco de dados MySQL usando o host `localhost` e a porta `3306`. Use as credenciais fornecidas no arquivo `docker-compose.yml` para fazer login.

## Personalização do arquivo docker-compose.yml

No arquivo `docker-compose.yml`, você pode personalizar as seguintes variáveis de ambiente:

- `MYSQL_ROOT_PASSWORD`: senha para o usuário root do MySQL.
- `MYSQL_DATABASE`: nome do banco de dados a ser criado.
- `MYSQL_USER` e `MYSQL_PASSWORD`: credenciais para um usuário adicional no banco de dados.

Certifique-se de ajustar essas variáveis de acordo com suas necessidades antes de iniciar o contêiner.

## Contribuição

Se você quiser contribuir para este projeto, fique à vontade para abrir uma nova issue ou enviar uma solicitação de pull. Teremos prazer em revisar e mesclar as alterações.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE). Sinta-se à vontade para usá-lo conforme necessário.

---

# MySQL Repository with Docker Compose

This repository contains a `docker-compose.yml` file that allows you to deploy a MySQL container easily and quickly. Docker Compose simplifies the process of setting up and running applications in containers using multiple Docker images.

## Prerequisites

Make sure you have Docker and Docker Compose installed on your system before proceeding.

- Docker: [Docker Installation](https://docs.docker.com/get-docker/)
- Docker Compose: [Docker Compose Installation](https://docs.docker.com/compose/install/)

## How to Use

1. Clone this repository to your system:

   ```shell
   git clone https://github.com/your-username/mysql-docker.git
   ```

2. Navigate to the repository directory:

   ```shell
   cd mysql-docker
   ```

3. Open the `docker-compose.yml` file in a text editor and customize the environment variables if needed. You can set the MySQL root password, database name, and other configurations in the `docker-compose.yml` file.

4. Start the MySQL container by running the following command:

   ```shell
   docker-compose up -d
   ```

   This will create and start the MySQL container in the background.

5. Wait until the container is started, and the MySQL service is ready to accept connections.

6. Now, you can connect to the MySQL database using the host `localhost` and port `3306`. Use the credentials provided in the `docker-compose.yml` file to log in.

## Customizing the docker-compose.yml File

In the `docker-compose.yml` file, you can customize the following environment variables:

- `MYSQL_ROOT_PASSWORD`: password for the MySQL root user.
- `MYSQL_DATABASE`: name of the database to be created.
- `MYSQL_USER` and `MYSQL_PASSWORD`: credentials for an additional user in the database.

Make sure to adjust these variables according to your needs before starting the container.

## Contribution

If you would like to contribute to this project, feel free to open a new issue or submit a pull request. We'll be glad to review and merge the changes.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use it as needed.
