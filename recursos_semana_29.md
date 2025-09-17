# Recursos - Semana 29: Backup e Recuperação

## Tópicos Abordados
*   Estratégias de backup.
*   Ferramentas de backup (rsync, tar).
*   Recuperação de dados.

## Objetivos de Aprendizagem
*   Desenvolver uma estratégia de backup.
*   Utilizar ferramentas de backup.

## Material de Apoio

### Apresentação: Backup e Recuperação de Dados no Linux

#### Slide 1: Título
*   **Título:** Backup e Recuperação
*   **Subtítulo:** Protegendo os seus Dados em Sistemas Open Source

#### Slide 2: A Importância do Backup
*   **Conteúdo:** Porquê fazer backup (falha de hardware, erro humano, ataques de malware). A regra 3-2-1 de backup.

#### Slide 3: Estratégias de Backup
*   **Conteúdo:** Backup completo, incremental, diferencial. Vantagens e desvantagens de cada um. Frequência e retenção.

#### Slide 4: Ferramenta `tar` - Arquivamento e Compressão
*   **Conteúdo:** Uso do comando `tar` para criar e extrair arquivos (`tar -cvf`, `tar -xvf`). Opções de compressão (`-z`, `-j`, `-J`).

#### Slide 5: Ferramenta `rsync` - Sincronização Eficiente
*   **Conteúdo:** O que é `rsync`. Sincronização de ficheiros localmente e remotamente. Vantagens (transferência incremental, compressão, preservação de permissões).

#### Slide 6: Exemplos de Uso de `rsync`
*   **Conteúdo:** `rsync -avz source/ destination/`. Sincronização remota via SSH.

#### Slide 7: Outras Ferramentas de Backup
*   **Conteúdo:** `dump`/`restore`, `dd`, `borgbackup` (breve menção).

#### Slide 8: Recuperação de Dados
*   **Conteúdo:** O processo de recuperação a partir de um backup. Testar backups regularmente. Recuperação de ficheiros individuais ou de um sistema completo.

#### Slide 9: Boas Práticas de Backup
*   **Conteúdo:** Armazenamento off-site, criptografia de backups, automatização, documentação da estratégia.

#### Slide 10: Conclusão
*   **Conteúdo:** O backup e a recuperação são componentes críticos de qualquer plano de segurança. Uma estratégia bem definida e testada é essencial para a continuidade do negócio.

### Artigo Introdutório: Guia Completo de Backup e Recuperação no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, criar um backup de um diretório usando `tar` e `rsync`. Simular a perda de dados e restaurar os ficheiros a partir do backup. (a ser detalhado na tarefa do Teams).

