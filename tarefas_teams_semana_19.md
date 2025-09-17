# Tarefas Microsoft Teams - Semana 19: Resolução de Problemas - Arranque e Sistema de Ficheiros

## Título da Tarefa: Diagnóstico e Recuperação de Problemas de Arranque e Ficheiros

## Descrição:
Nesta semana, vamos focar na resolução de problemas comuns relacionados com o arranque do sistema e o sistema de ficheiros em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos simular e resolver cenários de falha.

## Objetivos:
*   Diagnosticar problemas de arranque do sistema.
*   Recuperar sistemas de ficheiros danificados.
*   Utilizar ferramentas de recuperação como `fsck` e o modo de recuperação do GRUB.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre resolução de problemas de arranque e sistema de ficheiros).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Simulação de Problema de Arranque (GRUB):**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Edite o ficheiro `/etc/default/grub` e introduza um erro intencional (ex: altere `GRUB_TIMEOUT_STYLE=hidden` para `GRUB_TIMEOUT_STYLE=hiden`).
        *   Atualize o GRUB: `sudo update-grub`.
        *   Reinicie a VM. O sistema deverá falhar no arranque ou apresentar um erro no GRUB.
        *   **Recuperação:** Use o modo de recuperação do GRUB (geralmente pressionando `c` para a linha de comando) para corrigir o erro ou arranque o sistema usando um kernel mais antigo. Após arrancar, corrija o ficheiro `/etc/default/grub`, execute `sudo update-grub` e reinicie normalmente.
    *   **Simulação de Problema no Sistema de Ficheiros:**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Crie uma nova partição pequena (ex: 1GB) e formate-a com ext4. Monte-a em `/mnt/teste`.
        *   Simule uma falha de energia durante uma operação de escrita na partição (ex: `dd if=/dev/urandom of=/mnt/teste/arquivo_grande bs=1M count=500` e desligue a VM abruptamente).
        *   Reinicie a VM. O sistema pode tentar reparar a partição automaticamente ou pode ser necessário fazê-lo manualmente.
        *   **Recuperação:** Se a partição não montar ou apresentar erros, use `sudo fsck /dev/<particao_teste>` (ex: `/dev/sdb1`) para verificar e reparar o sistema de ficheiros. Monte a partição novamente.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do erro de arranque do GRUB.
    *   Captura de ecrã do terminal mostrando os passos de recuperação do GRUB.
    *   Captura de ecrã do terminal mostrando a execução do `fsck` e a recuperação do sistema de ficheiros.
    *   Uma breve reflexão sobre a importância de backups e de saber usar as ferramentas de recuperação.

## Critérios de Avaliação:
*   **Diagnóstico e Recuperação (60%):** Capacidade de simular, diagnosticar e resolver problemas de arranque e sistema de ficheiros.
*   **Relatório (20%):** Clareza das capturas de ecrã e da descrição dos problemas e soluções.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

