# Tarefas Microsoft Teams - Semana 9: Otimização de Recursos (Parte 1)

## Título da Tarefa: Monitorização e Gestão de Processos

## Descrição:
Nesta semana, vamos aprender a monitorizar e gerir os recursos do sistema operativo, focando na identificação e controlo de processos. A tarefa prática permitirá usar ferramentas de linha de comando para analisar o desempenho do sistema.

## Objetivos:
*   Monitorizar o uso de recursos do sistema (CPU, memória).
*   Identificar e gerir processos em execução.
*   Utilizar ferramentas de linha de comando como `top`, `htop`, `ps` e `kill`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre monitorização e gestão de processos).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop), execute os seguintes passos:
    *   Abra um terminal e execute o comando `top`. Observe as informações apresentadas (uso de CPU, memória, lista de processos). Identifique o processo que mais consome CPU e o que mais consome memória.
    *   Instale o `htop` (se ainda não estiver instalado: `sudo apt install htop`). Execute `htop` e explore a sua interface interativa. Identifique as mesmas informações que no `top`.
    *   Abra uma segunda instância do terminal e inicie um processo que consuma recursos (ex: `yes > /dev/null` para consumir CPU, ou um programa que faça muitos cálculos).
    *   No `htop` ou `top`, identifique o PID (Process ID) do processo que acabou de iniciar.
    *   No segundo terminal, use o comando `kill <PID>` para terminar o processo que iniciou. Observe a reação no `htop`/`top`.
    *   Use `ps aux | grep <nome_do_processo>` para procurar um processo específico e verificar se ele está em execução.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do `top` ou `htop` mostrando o processo que mais consome CPU e memória.
    *   Captura de ecrã do terminal mostrando o comando `kill` a ser executado e a confirmação da terminação do processo.
    *   Uma breve descrição da diferença entre `top` e `htop` e qual deles prefere usar e porquê.
    *   Uma reflexão sobre a importância de saber gerir processos para a otimização do sistema.

## Critérios de Avaliação:
*   **Execução dos Comandos (50%):** Demonstração correta do uso de `top`, `htop`, `ps` e `kill`.
*   **Relatório (30%):** Clareza das capturas de ecrã e da descrição das ferramentas e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

