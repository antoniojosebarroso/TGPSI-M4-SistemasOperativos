# Tarefas Microsoft Teams - Semana 32: Virtualização e Contentores (Avançado)

## Título da Tarefa: Construindo e Executando Contentores Docker

## Descrição:
Nesta semana, vamos aprofundar o conceito de contentores e a sua implementação prática com Docker. A tarefa permitirá aos alunos instalar o Docker, criar um Dockerfile, construir uma imagem e executar um contentor.

## Objetivos:
*   Instalar e configurar o Docker.
*   Criar um Dockerfile para uma aplicação simples.
*   Construir uma imagem Docker a partir de um Dockerfile.
*   Executar e gerir contentores Docker.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre Docker e contentores).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Server), execute os seguintes passos:
    *   **Instalação do Docker:**
        *   Instale o Docker Engine seguindo as instruções oficiais para a sua distribuição (geralmente `sudo apt install docker.io` e `sudo systemctl enable --now docker`).
        *   Adicione o seu utilizador ao grupo `docker` para executar comandos Docker sem `sudo`: `sudo usermod -aG docker $USER` (terá de fazer logout e login novamente para que a alteração tenha efeito).
        *   Verifique a instalação: `docker run hello-world`.
    *   **Criação de um Dockerfile e Imagem:**
        *   Crie um diretório para o seu projeto Docker: `mkdir ~/my_web_app && cd ~/my_web_app`.
        *   Crie um ficheiro `index.html` simples: `echo "<h1>Olá do meu Contentor Docker!</h1>" > index.html`.
        *   Crie um Dockerfile com o seguinte conteúdo:
            ```dockerfile
            FROM nginx:latest
            COPY index.html /usr/share/nginx/html
            EXPOSE 80
            CMD ["nginx", "-g", "daemon off;"]
            ```
        *   Construa a imagem Docker: `docker build -t my-nginx-app .`.
        *   Verifique se a imagem foi criada: `docker images`.
    *   **Execução e Gestão de Contentores:**
        *   Execute o contentor: `docker run -d -p 8080:80 --name my-web-container my-nginx-app`.
        *   Verifique se o contentor está em execução: `docker ps`.
        *   **No seu navegador (no sistema anfitrião ou numa segunda VM):** Aceda a `http://<IP_da_VM>:8080`. Deverá ver a página web que criou.
        *   Pare e remova o contentor: `docker stop my-web-container` e `docker rm my-web-container`.
        *   Remova a imagem: `docker rmi my-nginx-app`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a instalação do Docker e a execução do `hello-world`.
    *   Captura de ecrã do terminal mostrando o Dockerfile, a construção da imagem e a execução do contentor.
    *   Captura de ecrã do navegador mostrando a página web servida pelo contentor Docker.
    *   Uma breve reflexão sobre as vantagens dos contentores em comparação com as máquinas virtuais tradicionais para o desenvolvimento e implantação de aplicações.

## Critérios de Avaliação:
*   **Instalação e Configuração do Docker (40%):** O Docker deve estar instalado e a funcionar corretamente.
*   **Criação e Execução de Contentor (40%):** O Dockerfile deve ser criado, a imagem construída e o contentor executado com sucesso, servindo a página web.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

