# Recursos - Semana 23: Instalação de Aplicativos - Gestores de Pacotes (Parte 2)

## Tópicos Abordados
*   Atualização e remoção de pacotes.
*   Gestão de repositórios.

## Objetivos de Aprendizagem
*   Manter o sistema atualizado.
*   Adicionar e remover repositórios de software.

## Material de Apoio

### Apresentação: Manutenção de Software com Gestores de Pacotes

#### Slide 1: Título
*   **Título:** Instalação de Aplicativos - Gestores de Pacotes (Parte 2)
*   **Subtítulo:** Atualização, Remoção e Gestão de Repositórios

#### Slide 2: A Importância da Manutenção de Software
*   **Conteúdo:** Segurança (correções de vulnerabilidades), estabilidade (bugs corrigidos), novas funcionalidades. O papel dos gestores de pacotes.

#### Slide 3: Atualização de Pacotes (APT - Debian/Ubuntu)
*   **Conteúdo:** `apt update` (atualiza a lista de pacotes), `apt upgrade` (atualiza pacotes instalados), `apt full-upgrade` (atualiza com resolução de dependências complexas), `apt autoremove` (remove pacotes desnecessários).

#### Slide 4: Atualização de Pacotes (DNF/YUM - Red Hat/CentOS/Fedora)
*   **Conteúdo:** `dnf check-update`, `dnf upgrade`, `dnf autoremove`. Comparativo com APT.

#### Slide 5: Remoção de Pacotes (APT)
*   **Conteúdo:** `apt remove <pacote>` (remove o pacote, mantém ficheiros de configuração), `apt purge <pacote>` (remove o pacote e os ficheiros de configuração).

#### Slide 6: Remoção de Pacotes (DNF/YUM)
*   **Conteúdo:** `dnf remove <pacote>`. Como remover pacotes e suas dependências.

#### Slide 7: Gestão de Repositórios (APT)
*   **Conteúdo:** Adicionar novos repositórios (`add-apt-repository`). Ficheiros `/etc/apt/sources.list` e `/etc/apt/sources.list.d/`. Chaves GPG.

#### Slide 8: Gestão de Repositórios (DNF/YUM)
*   **Conteúdo:** Ficheiros `.repo` em `/etc/yum.repos.d/`. Como adicionar e remover repositórios.

#### Slide 9: Problemas Comuns na Gestão de Pacotes
*   **Conteúdo:** Conflitos de dependências, chaves GPG ausentes, repositórios quebrados. Como diagnosticar e resolver.

#### Slide 10: Conclusão
*   **Conteúdo:** A gestão eficaz de pacotes e repositórios é fundamental para manter um sistema Open Source seguro, estável e atualizado.

### Artigo Introdutório: Manutenção de Software no Linux com Gestores de Pacotes

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, realizar uma atualização completa do sistema. Instalar um pacote, removê-lo e depois purgá-lo. Adicionar um repositório de terceiros e instalar um pacote a partir dele. (a ser detalhado na tarefa do Teams).

