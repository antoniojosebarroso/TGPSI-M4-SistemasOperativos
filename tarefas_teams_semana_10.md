# Tarefas Microsoft Teams - Semana 10: Otimização de Recursos (Parte 2)

## Título da Tarefa: Otimizando o Arranque e a Memória Swap

## Descrição:
Nesta semana, vamos focar na otimização do arranque do sistema e na gestão da memória swap. A tarefa prática permitirá aos alunos identificar e desativar serviços desnecessários e ajustar o comportamento da swap para melhorar o desempenho do sistema.

## Objetivos:
*   Otimizar o arranque do sistema, gerindo serviços.
*   Ajustar a utilização da memória swap para melhor desempenho.
*   Utilizar comandos `systemctl` e configurar o parâmetro `swappiness`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre otimização de arranque e memória swap).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop), execute os seguintes passos:
    *   **Gestão de Serviços:**
        *   Abra um terminal e liste todos os serviços em execução: `systemctl list-units --type=service --state=running`.
        *   Identifique um serviço que considere desnecessário para um ambiente de desktop (ex: `cups.service` se não usar impressora, ou `bluetooth.service` se não tiver bluetooth). **Cuidado para não desativar serviços críticos!**
        *   Desative o serviço escolhido para que não inicie no próximo arranque: `sudo systemctl disable <nome_do_servico>`.
        *   Pare o serviço imediatamente: `sudo systemctl stop <nome_do_servico>`.
        *   Verifique o estado do serviço: `systemctl status <nome_do_servico>`.
    *   **Otimização da Memória Swap:**
        *   Verifique o valor atual de `swappiness`: `cat /proc/sys/vm/swappiness`.
        *   Altere o valor de `swappiness` para 10 (temporariamente): `sudo sysctl vm.swappiness=10`. Este valor faz com que o sistema use menos a swap.
        *   Para tornar a alteração permanente, edite o ficheiro `/etc/sysctl.conf` e adicione ou altere a linha `vm.swappiness=10`. Guarde o ficheiro.
        *   Aplique as alterações permanentemente: `sudo sysctl -p`.
        *   Verifique novamente o valor de `swappiness`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o serviço desativado e parado.
    *   Captura de ecrã do terminal mostrando o valor de `swappiness` antes e depois da alteração.
    *   Uma breve justificação para a escolha do serviço desativado e para o novo valor de `swappiness`.
    *   Uma reflexão sobre como estas otimizações podem impactar o desempenho do sistema.

## Critérios de Avaliação:
*   **Execução dos Comandos (50%):** Demonstração correta da gestão de serviços e da configuração de `swappiness`.
*   **Relatório (30%):** Clareza das capturas de ecrã e da justificação das escolhas e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

