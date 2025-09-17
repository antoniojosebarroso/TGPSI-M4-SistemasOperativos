# Tarefas Microsoft Teams - Semana 17: Múltiplas Configurações do Sistema - Dual Boot

## Título da Tarefa: Implementando um Ambiente Dual Boot

## Descrição:
Nesta semana, vamos explorar a configuração de sistemas com múltiplas opções de arranque, focando na implementação de um ambiente Dual Boot. A tarefa prática permitirá aos alunos instalar dois sistemas operativos na mesma máquina virtual e gerir o menu de arranque.

## Objetivos:
*   Compreender o conceito e a implementação de Dual Boot.
*   Instalar dois sistemas operativos (ex: Windows e Linux) na mesma máquina virtual.
*   Gerir o menu de arranque (GRUB).

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre Dual Boot).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop), execute os seguintes passos:
    *   **Preparação da VM:** Crie uma nova máquina virtual com um disco rígido de pelo menos 60GB. Instale o Windows (ou outro SO proprietário) primeiro, deixando espaço não alocado no disco para o Linux (ex: 30GB para Windows, 30GB para Linux).
    *   **Instalação do SO Open Source:** Inicie a instalação de uma distribuição Linux (ex: Ubuntu Desktop) na mesma VM.
    *   No passo de particionamento, escolha a opção "Instalar lado a lado" ou "Algo mais" para criar as partições Linux no espaço não alocado. Certifique-se de que o GRUB (bootloader) é instalado no disco principal.
    *   Conclua a instalação do Linux.
    *   **Teste do Dual Boot:** Reinicie a VM. Deverá aparecer o menu do GRUB, permitindo escolher entre o Windows e o Linux. Inicie ambos os sistemas para confirmar que funcionam corretamente.
    *   **Configuração do GRUB (Opcional):** Edite o ficheiro `/etc/default/grub` para alterar a ordem de arranque ou o tempo de espera. Após a edição, execute `sudo update-grub` e reinicie para ver as alterações.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do ecrã de particionamento durante a instalação do Linux, mostrando as partições do Windows e do Linux.
    *   Captura de ecrã do menu do GRUB, mostrando as opções de arranque para ambos os sistemas operativos.
    *   Captura de ecrã de ambos os sistemas operativos (Windows e Linux) a funcionar na mesma VM.
    *   Uma breve reflexão sobre as vantagens e desvantagens de um ambiente Dual Boot.

## Critérios de Avaliação:
*   **Implementação do Dual Boot (60%):** Ambos os sistemas operativos devem estar instalados e a funcionar corretamente, com o menu do GRUB a permitir a escolha entre eles.
*   **Relatório (20%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

