# Tarefas Microsoft Teams - Semana 27: Segurança em Sistemas Open Source (Introdução)

## Título da Tarefa: Fundamentos de Segurança e Análise de Logs

## Descrição:
Nesta semana, vamos introduzir os princípios fundamentais de segurança em Sistemas Operativos Open Source, focando na importância das atualizações e na análise de logs. A tarefa prática permitirá aos alunos observar eventos de segurança em logs e configurar o sistema para receber notificações de atualizações.

## Objetivos:
*   Compreender os princípios básicos de segurança em SO Open Source.
*   Reconhecer a importância das atualizações de segurança.
*   Analisar logs do sistema para identificar eventos de segurança.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre segurança em SO Open Source).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Simulação de Tentativa de Login Falhada e Análise de Logs:**
        *   Abra um terminal e mantenha-o aberto para monitorizar logs.
        *   Abra um segundo terminal e tente fazer login como um utilizador inexistente ou com uma senha errada várias vezes (ex: `ssh usuario_inexistente@localhost` ou `su - usuario_inexistente`).
        *   No primeiro terminal, visualize o ficheiro de log de autenticação: `tail -f /var/log/auth.log`.
        *   Identifique as entradas que registam as tentativas de login falhadas. Anote a data, hora, utilizador e o tipo de erro.
    *   **Configuração de Notificações de Atualizações de Segurança:**
        *   Certifique-se de que o pacote `unattended-upgrades` está instalado: `sudo apt install unattended-upgrades`.
        *   Edite o ficheiro de configuração `/etc/apt/apt.conf.d/50unattended-upgrades` e certifique-se de que as linhas `Unattended-Upgrade::Mail` e `Unattended-Upgrade::MailOnlyOnError` estão configuradas para enviar e-mails (se tiver um servidor de e-mail configurado na VM, caso contrário, apenas observe a configuração).
        *   Configure o sistema para verificar e notificar sobre atualizações de segurança. Pode usar o comando `sudo dpkg-reconfigure -plow unattended-upgrades` para configurar as opções básicas.
        *   Verifique o ficheiro `/var/log/unattended-upgrades/unattended-upgrades.log` para ver o histórico de verificações e atualizações.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando as entradas no `/var/log/auth.log` que registam as tentativas de login falhadas.
    *   Captura de ecrã do terminal mostrando o ficheiro de configuração `50unattended-upgrades` com as opções de e-mail (mesmo que não esteja a enviar e-mails reais).
    *   Uma breve reflexão sobre a importância de monitorizar logs de segurança e de manter o sistema atualizado para prevenir ataques.

## Critérios de Avaliação:
*   **Análise de Logs (40%):** Capacidade de identificar e interpretar eventos de segurança no `auth.log`.
*   **Configuração de Atualizações (40%):** Demonstração da configuração de notificações de atualizações de segurança.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

