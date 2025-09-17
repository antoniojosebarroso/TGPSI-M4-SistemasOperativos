# Tarefas Microsoft Teams - Semana 30: Monitorização e Logs

## Título da Tarefa: Monitorizando o Sistema e Analisando Logs

## Descrição:
Nesta semana, vamos focar na monitorização do sistema e na análise de logs para garantir a saúde e o bom funcionamento dos Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos utilizar ferramentas de linha de comando para verificar o uso de recursos e diagnosticar problemas através dos logs.

## Objetivos:
*   Monitorizar o uso de disco, CPU e memória.
*   Analisar logs do sistema para identificar eventos e problemas.
*   Utilizar comandos como `df`, `du`, `journalctl` e `grep`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre monitorização e logs).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Monitorização de Disco:**
        *   Verifique o espaço livre em disco para todos os sistemas de ficheiros: `df -h`.
        *   Verifique o tamanho de um diretório específico (ex: `/var/log`): `sudo du -sh /var/log`.
        *   Identifique os 10 maiores ficheiros no diretório `/var/log` (ou outro diretório grande): `sudo find /var/log -type f -print0 | xargs -0 du -h | sort -rh | head -n 10`.
    *   **Análise de Logs com `journalctl`:**
        *   Visualize os logs mais recentes do sistema: `journalctl -f` (pressione Ctrl+C para sair).
        *   Visualize os logs de um serviço específico (ex: `ssh`): `journalctl -u ssh.service`.
        *   Visualize os logs dos últimos 30 minutos: `journalctl --since "30 minutes ago"`.
        *   Filtre os logs para encontrar mensagens de erro: `journalctl -p err`.
    *   **Análise de Logs com `grep`:**
        *   Procure por todas as ocorrências da palavra "error" no ficheiro `/var/log/syslog`: `grep -i "error" /var/log/syslog`.
        *   Procure por tentativas de login falhadas no ficheiro `/var/log/auth.log`: `grep "Failed password" /var/log/auth.log`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a saída de `df -h` e `sudo du -sh /var/log`.
    *   Captura de ecrã do terminal mostrando a saída de `journalctl -u ssh.service` ou `journalctl -p err`.
    *   Captura de ecrã do terminal mostrando a saída de `grep "Failed password" /var/log/auth.log`.
    *   Uma breve reflexão sobre como a monitorização e a análise de logs são cruciais para a manutenção e resolução de problemas em sistemas Linux.

## Critérios de Avaliação:
*   **Monitorização de Recursos (40%):** Demonstração correta do uso de `df`, `du` e `find` para monitorizar o disco.
*   **Análise de Logs (40%):** Demonstração correta do uso de `journalctl` e `grep` para analisar logs.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

