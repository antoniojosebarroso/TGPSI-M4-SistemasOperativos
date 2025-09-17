# Tarefas Microsoft Teams - Semana 22: Instalação de Aplicativos - Gestores de Pacotes (Parte 1)

## Título da Tarefa: Dominando os Gestores de Pacotes Debian/Ubuntu

## Descrição:
Nesta semana, vamos aprofundar a instalação de aplicativos em Sistemas Operativos Open Source, focando nos gestores de pacotes `apt` e `dpkg` da família Debian/Ubuntu. A tarefa prática permitirá aos alunos instalar, remover e gerir pacotes de software.

## Objetivos:
*   Compreender o funcionamento dos gestores de pacotes `apt` e `dpkg`.
*   Instalar, remover e atualizar pacotes de software.
*   Gerir repositórios de software.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre gestores de pacotes).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Atualização e Instalação de Pacotes:**
        *   Atualize a lista de pacotes: `sudo apt update`.
        *   Atualize os pacotes instalados: `sudo apt upgrade -y`.
        *   Instale um pacote simples (ex: `cowsay`): `sudo apt install cowsay`.
        *   Verifique se o pacote foi instalado e funciona: `cowsay "Olá, TGPSI!"`.
    *   **Remoção de Pacotes:**
        *   Remova o pacote `cowsay`, mantendo os ficheiros de configuração: `sudo apt remove cowsay`.
        *   Remova o pacote `cowsay` e os seus ficheiros de configuração: `sudo apt purge cowsay`.
    *   **Pesquisa de Pacotes:**
        *   Pesquise por um pacote (ex: `nginx`): `apt search nginx`.
        *   Obtenha informações detalhadas sobre um pacote: `apt show nginx`.
    *   **Gestão de Pacotes .deb com `dpkg`:**
        *   Faça o download de um pacote `.deb` (ex: o Google Chrome, ou outro pacote simples que não esteja nos repositórios padrão). Pode usar `wget` para baixar o ficheiro.
        *   Tente instalar o pacote usando `sudo dpkg -i <nome_do_pacote.deb>`. Observe os erros de dependência, se existirem.
        *   Resolva as dependências: `sudo apt install -f`.
        *   Remova o pacote instalado com `dpkg`: `sudo dpkg -r <nome_do_pacote>`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a instalação e execução do `cowsay`.
    *   Captura de ecrã do terminal mostrando a pesquisa e informações do `nginx`.
    *   Captura de ecrã do terminal mostrando a instalação de um pacote `.deb` com `dpkg` e a resolução de dependências com `apt install -f`.
    *   Uma breve reflexão sobre a importância dos gestores de pacotes para a manutenção de um sistema Linux.

## Critérios de Avaliação:
*   **Uso de Gestores de Pacotes (60%):** Demonstração correta do uso de `apt` e `dpkg` para instalar, remover, atualizar e pesquisar pacotes.
*   **Resolução de Dependências (20%):** Capacidade de resolver dependências de pacotes.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

