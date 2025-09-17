# Tarefas Microsoft Teams - Semana 15: Configuração do Sistema - Utilizadores e Permissões

## Título da Tarefa: Gerindo Utilizadores e Controlando Acessos

## Descrição:
Nesta semana, vamos focar na gestão de utilizadores e grupos, bem como no sistema de permissões de ficheiros e diretórios em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos criar utilizadores, gerir grupos e aplicar permissões para controlar o acesso a recursos.

## Objetivos:
*   Criar, modificar e remover utilizadores e grupos.
*   Compreender e aplicar permissões de ficheiros e diretórios (rwx).
*   Utilizar comandos como `useradd`, `usermod`, `groupadd`, `chmod`, `chown`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre gestão de utilizadores e permissões).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Gestão de Utilizadores e Grupos:**
        *   Crie um novo utilizador chamado `aluno_a`: `sudo useradd -m -s /bin/bash aluno_a`.
        *   Defina uma senha para `aluno_a`: `sudo passwd aluno_a`.
        *   Crie um novo grupo chamado `desenvolvimento`: `sudo groupadd desenvolvimento`.
        *   Adicione o utilizador `aluno_a` ao grupo `desenvolvimento`: `sudo usermod -aG desenvolvimento aluno_a`.
        *   Verifique se o utilizador `aluno_a` pertence ao grupo `desenvolvimento`: `groups aluno_a`.
        *   Crie um segundo utilizador chamado `aluno_b` e adicione-o ao grupo `desenvolvimento`.
    *   **Gestão de Permissões:**
        *   Crie um diretório chamado `projeto_comum` no diretório `/home`: `sudo mkdir /home/projeto_comum`.
        *   Altere o proprietário do diretório para `aluno_a` e o grupo para `desenvolvimento`: `sudo chown aluno_a:desenvolvimento /home/projeto_comum`.
        *   Defina as permissões para que o proprietário tenha leitura, escrita e execução (rwx), o grupo tenha leitura, escrita e execução (rwx), e outros não tenham permissão alguma: `sudo chmod 770 /home/projeto_comum`.
        *   Verifique as permissões: `ls -ld /home/projeto_comum`.
        *   Crie um ficheiro dentro de `projeto_comum` como `aluno_a` (faça `su - aluno_a` para mudar de utilizador). Verifique as permissões do ficheiro.
        *   Tente aceder e modificar o ficheiro como `aluno_b` (faça `su - aluno_b`).
        *   Tente aceder ao diretório `projeto_comum` como um utilizador que não seja `aluno_a` ou `aluno_b` (ex: o seu utilizador principal).
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a criação dos utilizadores e grupos, e a adição dos utilizadores aos grupos.
    *   Captura de ecrã do terminal mostrando a alteração de proprietário/grupo e as permissões do diretório `projeto_comum`.
    *   Captura de ecrã do terminal mostrando a tentativa de acesso/modificação do ficheiro por `aluno_b` e por um utilizador fora do grupo `desenvolvimento`.
    *   Uma breve reflexão sobre a importância das permissões para a segurança e colaboração em sistemas multiutilizador.

## Critérios de Avaliação:
*   **Gestão de Utilizadores e Grupos (40%):** Criação e configuração correta de utilizadores e grupos.
*   **Gestão de Permissões (40%):** Aplicação correta das permissões de ficheiros e diretórios e demonstração do controlo de acesso.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

