# Tarefas Microsoft Teams - Semana 31: Automação de Tarefas

## Título da Tarefa: Automatizando com Cron e Shell Scripts

## Descrição:
Nesta semana, vamos focar na automação de tarefas repetitivas em Sistemas Operativos Open Source, utilizando `cron` para agendamento e `shell scripts` para execução. A tarefa prática permitirá aos alunos criar e agendar scripts para otimizar a administração do sistema.

## Objetivos:
*   Automatizar tarefas utilizando `cron`.
*   Escrever `shell scripts` básicos para automação.
*   Compreender a importância da automação na administração de sistemas.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre automação de tarefas).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Criação de um Shell Script Simples:**
        *   Crie um script chamado `log_data.sh` no seu diretório home com o seguinte conteúdo:
            ```bash
            #!/bin/bash
            DATA=$(date)
            echo "O script foi executado em: $DATA" >> ~/script_log.txt
            ```
        *   Torne o script executável: `chmod +x ~/log_data.sh`.
        *   Teste o script: `~/log_data.sh`. Verifique o conteúdo de `~/script_log.txt`.
    *   **Agendamento com Cron:**
        *   Edite a sua tabela cron: `crontab -e`.
        *   Adicione a seguinte linha para executar o script a cada 5 minutos (para fins de teste):
            ```
            */5 * * * * /home/<seu_utilizador>/log_data.sh
            ```
        *   Guarde e saia do editor. O cron job será ativado.
        *   Aguarde 5-10 minutos e verifique o ficheiro `~/script_log.txt`. Deverá ver múltiplas entradas.
    *   **Criação de um Script de Verificação de Espaço em Disco:**
        *   Crie um script chamado `verifica_disco.sh` no seu diretório home com o seguinte conteúdo (substitua `90` pela percentagem de uso de disco que considera crítica):
            ```bash
            #!/bin/bash
            USO_DISCO=$(df -h / | awk 'NR==2 {print $5}' | sed 's/%//g')
            if [ "$USO_DISCO" -gt 90 ]; then
                echo "ALERTA: Uso de disco em / é de ${USO_DISCO}%!" >> ~/alerta_disco.log
            fi
            ```
        *   Torne o script executável: `chmod +x ~/verifica_disco.sh`.
        *   Teste o script manualmente. Se o uso de disco for superior a 90%, o ficheiro `~/alerta_disco.log` será criado/atualizado.
        *   Adicione este script ao cron para ser executado diariamente (ex: à 1h da manhã): `0 1 * * * /home/<seu_utilizador>/verifica_disco.sh`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o conteúdo do script `log_data.sh` e do ficheiro `script_log.txt` com as entradas do cron.
    *   Captura de ecrã do terminal mostrando o conteúdo do script `verifica_disco.sh` e (se aplicável) do ficheiro `alerta_disco.log`.
    *   Captura de ecrã do terminal mostrando a sua tabela cron (`crontab -l`).
    *   Uma breve reflexão sobre como a automação pode simplificar tarefas de administração de sistemas e melhorar a eficiência.

## Critérios de Avaliação:
*   **Criação e Execução de Scripts (40%):** Os scripts devem estar corretamente criados, executáveis e a funcionar como esperado.
*   **Agendamento com Cron (40%):** Os cron jobs devem estar configurados corretamente e a executar os scripts nos horários definidos.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

