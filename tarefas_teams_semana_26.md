# Tarefas Microsoft Teams - Semana 26: Instalação de Aplicativos - Aplicações de Servidor

## Título da Tarefa: Configurando um Servidor de Base de Dados e um Servidor Web Avançado

## Descrição:
Nesta semana, vamos focar na instalação e configuração de aplicações de servidor essenciais em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos instalar e configurar um servidor de base de dados (MySQL/MariaDB) e um servidor web com suporte a PHP.

## Objetivos:
*   Instalar e configurar um servidor de base de dados.
*   Instalar e configurar um servidor web com suporte a linguagens de script (PHP).
*   Testar a integração entre o servidor web e a base de dados.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre aplicações de servidor).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Server), execute os seguintes passos:
    *   **Instalação e Configuração do Servidor de Base de Dados (MariaDB/MySQL):**
        *   Instale o MariaDB Server: `sudo apt install mariadb-server`.
        *   Execute o script de segurança pós-instalação: `sudo mysql_secure_installation` (defina uma senha para o root, remova utilizadores anónimos, etc.).
        *   Crie uma base de dados e um utilizador para ela:
            *   `sudo mysql -u root -p`
            *   `CREATE DATABASE minha_app_db;`
            *   `CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'sua_senha_segura';`
            *   `GRANT ALL PRIVILEGES ON minha_app_db.* TO 'app_user'@'localhost';`
            *   `FLUSH PRIVILEGES;`
            *   `EXIT;`
    *   **Instalação e Configuração do Servidor Web com PHP (LAMP/LEMP Stack):**
        *   Instale o Apache2 (se ainda não tiver) e o PHP com módulos essenciais:
            *   `sudo apt install apache2 php libapache2-mod-php php-mysql`
        *   Reinicie o Apache: `sudo systemctl restart apache2`.
        *   Crie um ficheiro de teste PHP (`info.php`) no diretório web (`/var/www/html/`):
            *   `echo 


<?php phpinfo(); ?>" | sudo tee /var/www/html/info.php`
        *   **No seu navegador:** Aceda a `http://<IP_da_VM>/info.php`. Deverá ver a página de informações do PHP.
        *   Crie um ficheiro PHP simples (`db_test.php`) para testar a conexão com a base de dados:
            ```php
            <?php
            $servername = "localhost";
            $username = "app_user";
            $password = "sua_senha_segura";
            $dbname = "minha_app_db";

            // Create connection
            $conn = new mysqli($servername, $username, $password, $dbname);

            // Check connection
            if ($conn->connect_error) {
                die("Connection failed: " . $conn->connect_error);
            }
            echo "Connected successfully to database!";
            $conn->close();
            ?>
            ```
            *   `echo '<?php $servername = 


<?php
            $servername = "localhost";
            $username = "app_user";
            $password = "sua_senha_segura";
            $dbname = "minha_app_db";

            // Create connection
            $conn = new mysqli($servername, $username, $password, $dbname);

            // Check connection
            if ($conn->connect_error) {
                die("Connection failed: " . $conn->connect_error);
            }
            echo "Connected successfully to database!";
            $conn->close();
            ?>
            ' | sudo tee /var/www/html/db_test.php`
        *   **No seu navegador:** Aceda a `http://<IP_da_VM>/db_test.php`. Deverá ver a mensagem de conexão bem-sucedida.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a criação da base de dados e do utilizador no MariaDB/MySQL.
    *   Captura de ecrã do navegador mostrando a página `info.php`.
    *   Captura de ecrã do navegador mostrando a página `db_test.php` com a mensagem de conexão bem-sucedida.
    *   Uma breve reflexão sobre a importância de um stack LAMP/LEMP para o desenvolvimento e alojamento de aplicações web dinâmicas.

## Critérios de Avaliação:
*   **Servidor de Base de Dados (40%):** O MariaDB/MySQL deve estar instalado, seguro e com uma base de dados e utilizador criados.
*   **Servidor Web com PHP (40%):** O Apache2 com PHP deve estar instalado e a funcionar, e a conexão com a base de dados deve ser bem-sucedida.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

