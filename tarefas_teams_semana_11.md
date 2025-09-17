# Tarefas Microsoft Teams - Semana 11: Instalação de Dispositivos e Device Drivers (Parte 1)

## Título da Tarefa: Identificando Hardware e Módulos de Kernel

## Descrição:
Nesta semana, vamos aprender a identificar o hardware instalado num sistema Open Source e a compreender o papel dos módulos de kernel. A tarefa prática permitirá usar ferramentas de linha de comando para listar e gerir dispositivos e drivers.

## Objetivos:
*   Identificar o hardware instalado num sistema Linux.
*   Compreender o papel dos módulos de kernel na interação com o hardware.
*   Utilizar comandos como `lspci`, `lsusb` e `lsmod`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre identificação de hardware e módulos de kernel).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop), execute os seguintes passos:
    *   Abra um terminal e execute o comando `lspci`. Anote os principais dispositivos PCI listados (ex: placa gráfica, controlador Ethernet, controlador de armazenamento).
    *   Execute `lspci -k` para ver quais módulos de kernel estão a ser usados por cada dispositivo PCI.
    *   Execute o comando `lsusb`. Anote os dispositivos USB listados (ex: hub USB, teclado, rato).
    *   Execute `lsmod` para listar todos os módulos de kernel atualmente carregados. Tente identificar módulos relacionados com os dispositivos que listou com `lspci` e `lsusb`.
    *   Escolha um módulo de kernel que não seja crítico para o funcionamento do sistema (ex: um módulo de som ou de um dispositivo USB que não esteja em uso) e tente descarregá-lo (`sudo rmmod <nome_do_modulo>`). Verifique com `lsmod` se foi descarregado. **Cuidado para não descarregar módulos essenciais!**
    *   Carregue o módulo novamente (`sudo modprobe <nome_do_modulo>`).
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a saída de `lspci` e `lsusb`.
    *   Captura de ecrã do terminal mostrando o comando `sudo rmmod` e `sudo modprobe` e a verificação com `lsmod`.
    *   Uma breve descrição da função de pelo menos três módulos de kernel que identificou.
    *   Uma reflexão sobre a importância de saber identificar hardware e gerir módulos de kernel para a instalação de drivers.

## Critérios de Avaliação:
*   **Execução dos Comandos (50%):** Demonstração correta do uso de `lspci`, `lsusb`, `lsmod`, `rmmod` e `modprobe`.
*   **Relatório (30%):** Clareza das capturas de ecrã e da descrição dos módulos e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

