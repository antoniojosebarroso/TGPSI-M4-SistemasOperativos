# Recursos - Semana 19: Resolução de Problemas - Arranque e Sistema de Ficheiros

## Tópicos Abordados
*   Problemas comuns de arranque (GRUB).
*   Recuperação de sistema de ficheiros (fsck).

## Objetivos de Aprendizagem
*   Diagnosticar e resolver problemas de arranque.
*   Recuperar sistemas de ficheiros danificados.

## Material de Apoio

### Apresentação: Resolução de Problemas de Arranque e Ficheiros

#### Slide 1: Título
*   **Título:** Resolução de Problemas - Arranque e Sistema de Ficheiros
*   **Subtítulo:** Diagnóstico e Recuperação em SO Open Source

#### Slide 2: Introdução à Resolução de Problemas
*   **Conteúdo:** A importância de saber diagnosticar e resolver problemas em sistemas operativos. Ferramentas e metodologias.

#### Slide 3: Problemas Comuns de Arranque
*   **Conteúdo:** O sistema não arranca, ecrã preto, mensagens de erro do GRUB, kernel panic. Causas comuns (atualizações falhadas, configuração incorreta, hardware).

#### Slide 4: GRUB (Grand Unified Bootloader)
*   **Conteúdo:** O que é o GRUB. Sua função no processo de arranque. Ficheiros de configuração (`/boot/grub/grub.cfg`).

#### Slide 5: Recuperação do GRUB
*   **Conteúdo:** Usar um Live CD/USB para aceder ao sistema. Comandos `chroot`, `grub-install`, `update-grub`. Cenários de recuperação.

#### Slide 6: Sistema de Ficheiros Corrompido
*   **Conteúdo:** Causas de corrupção (falha de energia, desligamento incorreto, hardware defeituoso). Sintomas (ficheiros inacessíveis, erros de leitura/escrita).

#### Slide 7: `fsck` (File System Check)
*   **Conteúdo:** O que é `fsck`. Como usar para verificar e reparar sistemas de ficheiros. Opções (`-y`, `-f`). A importância de executar `fsck` em partições desmontadas.

#### Slide 8: Recuperação de Dados Básica
*   **Conteúdo:** Ferramentas como `testdisk` e `photorec` (breve introdução). A importância de backups regulares.

#### Slide 9: Modo de Recuperação (Recovery Mode)
*   **Conteúdo:** Como aceder ao modo de recuperação em distribuições Linux. Opções disponíveis (reparar sistema de ficheiros, ativar rede, shell de root).

#### Slide 10: Conclusão
*   **Conteúdo:** A resolução de problemas de arranque e sistema de ficheiros exige paciência e conhecimento das ferramentas certas. Backups são a melhor defesa.

### Artigo Introdutório: Guia de Resolução de Problemas de Arranque e Ficheiros no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, simular um problema de arranque (ex: corromper o GRUB) e tentar recuperá-lo usando um Live CD/USB. Simular um sistema de ficheiros corrompido e usar `fsck` para repará-lo. (a ser detalhado na tarefa do Teams).

