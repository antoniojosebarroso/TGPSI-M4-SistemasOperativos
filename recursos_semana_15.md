# Recursos - Semana 15: Configuração do Sistema - Utilizadores e Permissões

## Tópicos Abordados
*   Gestão avançada de utilizadores e grupos.
*   Permissões de ficheiros e diretórios (chmod, chown).

## Objetivos de Aprendizagem
*   Gerir permissões de forma eficaz.
*   Controlar o acesso a ficheiros e diretórios.

## Material de Apoio

### Apresentação: Gestão de Utilizadores e Permissões

#### Slide 1: Título
*   **Título:** Configuração do Sistema - Utilizadores e Permissões
*   **Subtítulo:** Controlando o Acesso no SO Open Source

#### Slide 2: Revisão: Utilizadores e Grupos
*   **Conteúdo:** O que são utilizadores e grupos no Linux. O papel do `root`. Comandos básicos (`useradd`, `usermod`, `userdel`, `groupadd`, `groupdel`).

#### Slide 3: Ficheiros de Configuração de Utilizadores e Grupos
*   **Conteúdo:** `/etc/passwd`, `/etc/shadow`, `/etc/group`, `/etc/gshadow`. O que cada ficheiro armazena e a sua importância para a segurança.

#### Slide 4: Permissões de Ficheiros e Diretórios
*   **Conteúdo:** Os três tipos de permissões (leitura, escrita, execução). Os três tipos de utilizadores (proprietário, grupo, outros). Representação simbólica (rwx) e numérica (octal).

#### Slide 5: Comando `chmod`
*   **Conteúdo:** Alterar permissões de ficheiros e diretórios. Exemplos de uso com notação simbólica (`chmod u+x file.sh`) e numérica (`chmod 755 file.sh`).

#### Slide 6: Comando `chown`
*   **Conteúdo:** Alterar o proprietário de um ficheiro ou diretório. Exemplos de uso (`chown user:group file`).

#### Slide 7: Comando `chgrp`
*   **Conteúdo:** Alterar o grupo de um ficheiro ou diretório. Uso e diferenças em relação ao `chown`.

#### Slide 8: Permissões Especiais (SUID, SGID, Sticky Bit)
*   **Conteúdo:** Explicação do SUID (executar como proprietário), SGID (executar como grupo, herdar grupo em diretórios) e Sticky Bit (apenas proprietário pode apagar ficheiros em diretórios partilhados).

#### Slide 9: Máscara de Criação de Ficheiros (`umask`)
*   **Conteúdo:** Como o `umask` afeta as permissões padrão de novos ficheiros e diretórios. Como verificar e alterar o `umask`.

#### Slide 10: Conclusão
*   **Conteúdo:** A gestão de utilizadores e permissões é um pilar fundamental da segurança e administração de sistemas Open Source. O domínio destas ferramentas é essencial.

### Artigo Introdutório: Guia Completo de Gestão de Utilizadores e Permissões no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, criar novos utilizadores e grupos. Criar ficheiros e diretórios e alterar as suas permissões e proprietários usando `chmod` e `chown`. Testar o acesso com diferentes utilizadores. (a ser detalhado na tarefa do Teams).

