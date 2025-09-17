Descrição:
Nesta semana, vamos configurar serviços essenciais em Sistemas Operativos Open Source, como o servidor SSH para acesso remoto seguro e um servidor web (Nginx ou Apache) para alojar conteúdo. A tarefa prática permitirá aos alunos instalar, configurar e testar estes serviços.

## Objetivos:
*   Configurar um servidor SSH para acesso remoto seguro.
*   Instalar e configurar um servidor web (Nginx ou Apache).
*   Alojamento de uma página web simples.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre SSH e servidores web).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Configuração do Servidor SSH:**
        *   Instale o servidor OpenSSH: `sudo apt install openssh-server`.
        *   Verifique o estado do serviço: `sudo systemctl status ssh`.
        *   **Numa segunda VM (cliente) ou no seu sistema anfitrião:** Tente conectar-se via SSH à sua VM: `ssh <seu_utilizador>@<IP_da_VM>`.
        *   **Opcional (mas recomendado):** Configure a autenticação por chave SSH (gerar par de chaves, copiar chave pública para a VM, desativar autenticação por senha).
    *   **Configuração do Servidor Web (Escolha um):**
        *   **Opção A: Nginx**
            *   Instale o Nginx: `sudo apt install nginx`.
            *   Verifique o estado do serviço: `sudo systemctl status nginx`.
            *   Crie um ficheiro `index.html` simples no diretório `/var/www/html/` (ex: `echo "<h1>Bem-vindo ao meu servidor Nginx!</h1>" | sudo tee /var/www/html/index.html`).
            *   **No seu navegador (no sistema anfitrião ou numa segunda VM):** Aceda ao endereço IP da sua VM. Deverá ver a página web que criou.
        *   **Opção B: Apache2**
            *   Instale o Apache2: `sudo apt install apache2`.
            *   Verifique o estado do serviço: `sudo systemctl status apache2`.
            *   Crie um ficheiro `index.html` simples no diretório `/var/www/html/` (ex: `echo "<h1>Bem-vindo ao meu servidor Apache!</h1>" | sudo tee /var/www/html/index.html`).
            *   **No seu navegador (no sistema anfitrião ou numa segunda VM):** Aceda ao endereço IP da sua VM. Deverá ver a página web que criou.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a conexão SSH bem-sucedida à sua VM.
    *   Captura de ecrã do navegador mostrando a página web alojada no seu servidor (Nginx ou Apache).
    *   Uma breve reflexão sobre a importância destes serviços para a administração de sistemas e para o desenvolvimento web.

## Critérios de Avaliação:
*   **Servidor SSH (40%):** O servidor SSH deve estar instalado e acessível remotamente.
*   **Servidor Web (40%):** O servidor web (Nginx ou Apache) deve estar instalado, configurado e a alojar uma página web acessível.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

