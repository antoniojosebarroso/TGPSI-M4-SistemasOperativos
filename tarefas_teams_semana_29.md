Descrição:
Nesta semana, vamos focar na implementação de estratégias de backup e recuperação de dados em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos utilizar ferramentas como `tar` e `rsync` para criar e restaurar backups.

## Objetivos:
*   Desenvolver uma estratégia de backup eficaz.
*   Utilizar `tar` para arquivar e comprimir dados.
*   Utilizar `rsync` para sincronizar e fazer backups incrementais.
*   Simular a recuperação de dados a partir de um backup.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre backup e recuperação).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Preparação:** Crie um diretório de teste com alguns ficheiros e subdiretórios: `mkdir -p ~/backup_teste/docs && echo "ficheiro1" > ~/backup_teste/docs/file1.txt && echo "ficheiro2" > ~/backup_teste/file2.txt`.
    *   **Backup com `tar`:**
        *   Crie um backup completo do diretório `backup_teste` para um ficheiro `.tar.gz` no diretório `/tmp`: `tar -czvf /tmp/backup_completo.tar.gz ~/backup_teste`.
        *   Verifique o conteúdo do backup: `tar -tzvf /tmp/backup_completo.tar.gz`.
    *   **Backup com `rsync`:**
        *   Crie um diretório de destino para o `rsync`: `mkdir ~/backup_rsync`.
        *   Faça o primeiro backup (sincronização inicial): `rsync -avz ~/backup_teste/ ~/backup_rsync/`.
        *   Modifique um ficheiro no diretório original (ex: `echo "novo conteudo" >> ~/backup_teste/docs/file1.txt`).
        *   Faça um segundo backup incremental: `rsync -avz ~/backup_teste/ ~/backup_rsync/`.
        *   Observe que apenas o ficheiro modificado foi transferido.
    *   **Simulação de Perda de Dados e Recuperação:**
        *   Apague o diretório original: `rm -rf ~/backup_teste`.
        *   **Recuperação com `tar`:** Extraia o backup completo para o seu diretório home: `tar -xzvf /tmp/backup_completo.tar.gz -C ~`.
        *   Verifique se os ficheiros foram restaurados (o `file1.txt` deverá ter o conteúdo original).
        *   **Recuperação com `rsync`:** Apague novamente o diretório original. Copie os ficheiros do `backup_rsync` de volta para o diretório original: `rsync -avz ~/backup_rsync/ ~/backup_teste/`.
        *   Verifique se os ficheiros foram restaurados (o `file1.txt` deverá ter o conteúdo modificado).
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a criação do backup com `tar` e a sua extração.
    *   Captura de ecrã do terminal mostrando os dois comandos `rsync` (inicial e incremental) e a recuperação dos dados.
    *   Uma breve reflexão sobre as vantagens e desvantagens de `tar` e `rsync` para diferentes cenários de backup.

## Critérios de Avaliação:
*   **Implementação de Backup (60%):** Demonstração correta do uso de `tar` e `rsync` para criar backups.
*   **Recuperação de Dados (20%):** Capacidade de restaurar dados a partir dos backups criados.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

