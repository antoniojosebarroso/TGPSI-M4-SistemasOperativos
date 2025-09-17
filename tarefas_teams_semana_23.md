Descrição:
Nesta semana, vamos aprofundar a gestão de pacotes, focando na gestão de repositórios e na compilação de software a partir do código fonte. A tarefa prática permitirá aos alunos adicionar repositórios, instalar pacotes de diferentes fontes e compilar um programa simples.

## Objetivos:
*   Gerir repositórios de software (adicionar, remover).
*   Compreender o processo de compilação de software a partir do código fonte.
*   Instalar software de diferentes fontes.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre gestão de repositórios e compilação).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Gestão de Repositórios:**
        *   Adicione o repositório PPA (Personal Package Archive) do `neofetch` (se ainda não o tiver instalado ou quiser uma versão mais recente):
            *   `sudo add-apt-repository ppa:dawidd0811/neofetch`
            *   `sudo apt update`
            *   `sudo apt install neofetch`
        *   Remova o PPA: `sudo add-apt-repository --remove ppa:dawidd0811/neofetch`.
        *   Remova o `neofetch` e limpe os pacotes órfãos: `sudo apt purge neofetch && sudo apt autoremove`.
    *   **Compilação a partir do Código Fonte:**
        *   Instale as ferramentas de compilação: `sudo apt install build-essential`.
        *   Faça o download do código fonte de um programa simples (ex: `htop` ou `cowsay` se não o tiver instalado via `apt`). Use `wget` para baixar o `.tar.gz` ou `.zip` do site oficial (ex: `https://github.com/htop-dev/htop/releases`).
        *   Descompacte o ficheiro: `tar -xvzf <nome_do_ficheiro.tar.gz>`.
        *   Navegue para o diretório descompactado.
        *   Execute os comandos de compilação (geralmente):
            *   `./configure`
            *   `make`
            *   `sudo make install`
        *   Verifique se o programa foi instalado e funciona.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a adição e remoção do PPA, e a instalação do `neofetch`.
    *   Captura de ecrã do terminal mostrando os comandos de compilação (`./configure`, `make`, `sudo make install`) e a execução bem-sucedida do programa compilado.
    *   Uma breve reflexão sobre as vantagens e desvantagens de instalar software via gestor de pacotes vs. compilação a partir do código fonte.

## Critérios de Avaliação:
*   **Gestão de Repositórios (40%):** Demonstração correta da adição e remoção de PPAs.
*   **Compilação de Software (40%):** Execução bem-sucedida do processo de compilação e instalação de um programa a partir do código fonte.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

