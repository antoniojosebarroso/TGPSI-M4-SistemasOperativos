# Tarefas Microsoft Teams - Semana 21: Resolução de Problemas - Aplicações e Permissões

## Título da Tarefa: Diagnóstico e Resolução de Problemas em Aplicações e Permissões

## Descrição:
Nesta semana, vamos focar na resolução de problemas comuns relacionados com o funcionamento de aplicações e com as permissões de ficheiros e diretórios em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos diagnosticar e resolver cenários de falha de aplicações e problemas de acesso.

## Objetivos:
*   Diagnosticar problemas de execução de aplicações.
*   Resolver problemas de permissões de ficheiros e diretórios.
*   Utilizar comandos como `strace`, `lsof`, `chmod`, `chown`.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre resolução de problemas de aplicações e permissões).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Simulação de Problema de Permissões (Ficheiro):**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Crie um ficheiro de texto: `echo "Conteúdo secreto" > /tmp/secreto.txt`.
        *   Altere as permissões para que apenas o proprietário possa ler e escrever: `chmod 600 /tmp/secreto.txt`.
        *   Tente ler o ficheiro como outro utilizador (ex: `su - outro_utilizador` e `cat /tmp/secreto.txt`). Deverá falhar.
        *   **Diagnóstico e Recuperação:** Use `ls -l /tmp/secreto.txt` para verificar as permissões. Corrija as permissões para permitir que outros utilizadores leiam o ficheiro: `chmod 644 /tmp/secreto.txt`. Teste novamente.
    *   **Simulação de Problema de Permissões (Execução de Script):**
        *   Crie um script shell simples: `echo '#!/bin/bash
echo "Olá do script!"' > /tmp/meu_script.sh`.
        *   Tente executar o script: `/tmp/meu_script.sh`. Deverá falhar com "Permission denied".
        *   **Diagnóstico e Recuperação:** Use `ls -l /tmp/meu_script.sh` para verificar as permissões. Adicione permissão de execução: `chmod +x /tmp/meu_script.sh`. Teste novamente.
    *   **Diagnóstico de Aplicações (Opcional):**
        *   Instale uma aplicação simples (ex: `htop`).
        *   Tente executar `strace htop` para ver as chamadas de sistema que a aplicação faz. Analise a saída para entender como a aplicação interage com o sistema.
        *   Use `lsof -i :<porta>` (ex: `lsof -i :80`) para ver qual processo está a usar uma porta específica.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o problema de permissões no ficheiro e a sua resolução.
    *   Captura de ecrã do terminal mostrando o problema de execução do script e a sua resolução.
    *   (Opcional) Captura de ecrã do terminal mostrando a saída de `strace` ou `lsof`.
    *   Uma breve reflexão sobre a importância das permissões para a segurança e o funcionamento correto das aplicações.

## Critérios de Avaliação:
*   **Diagnóstico e Resolução (60%):** Capacidade de simular, diagnosticar e resolver problemas de permissões em ficheiros e scripts.
*   **Uso de Ferramentas (20%):** Demonstração correta do uso de `chmod`, `chown` e (opcionalmente) `strace`/`lsof`.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição dos problemas e soluções.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

