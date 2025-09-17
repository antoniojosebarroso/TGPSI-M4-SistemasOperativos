# Recursos - Semana 22: Instalação de Aplicativos - Gestores de Pacotes (Parte 1)

## Tópicos Abordados
*   Introdução a gestores de pacotes (APT, DNF/YUM).
*   Instalação de pacotes básicos.

## Objetivos de Aprendizagem
*   Utilizar gestores de pacotes para instalar software.
*   Gerir dependências de pacotes.

## Material de Apoio

### Apresentação: Gestores de Pacotes no Linux

#### Slide 1: Título
*   **Título:** Instalação de Aplicativos - Gestores de Pacotes (Parte 1)
*   **Subtítulo:** APT, DNF/YUM e a Gestão de Software

#### Slide 2: O que é um Gestor de Pacotes?
*   **Conteúdo:** Definição e função de um gestor de pacotes. Vantagens (automatização de instalação, atualização, remoção, gestão de dependências).

#### Slide 3: Repositórios de Software
*   **Conteúdo:** O que são repositórios. A importância de fontes confiáveis. Ficheiros de configuração de repositórios (`/etc/apt/sources.list`, `/etc/yum.repos.d/`).

#### Slide 4: APT (Advanced Package Tool) - Debian/Ubuntu
*   **Conteúdo:** Comandos básicos: `apt update` (atualizar lista de pacotes), `apt install <pacote>` (instalar), `apt search <pacote>` (procurar).

#### Slide 5: DNF/YUM - Red Hat/CentOS/Fedora
*   **Conteúdo:** Comandos básicos: `dnf check-update` (atualizar lista), `dnf install <pacote>` (instalar), `dnf search <pacote>` (procurar). (YUM é o antecessor do DNF).

#### Slide 6: Instalação de Pacotes Básicos
*   **Conteúdo:** Exemplos práticos de instalação de software comum (ex: `htop`, `neofetch`, `git`).

#### Slide 7: Gestão de Dependências
*   **Conteúdo:** Como os gestores de pacotes resolvem automaticamente as dependências. O que acontece quando uma dependência está em falta.

#### Slide 8: Ficheiros `.deb` e `.rpm`
*   **Conteúdo:** Formatos de pacotes. Instalação manual com `dpkg -i` (Debian) e `rpm -i` (Red Hat). Precauções ao instalar pacotes fora dos repositórios.

#### Slide 9: Verificação de Pacotes Instalados
*   **Conteúdo:** Comandos para listar pacotes instalados (`apt list --installed`, `dpkg -l`, `dnf list installed`).

#### Slide 10: Conclusão
*   **Conteúdo:** Os gestores de pacotes são ferramentas indispensáveis para a administração de sistemas Linux, simplificando a gestão de software e garantindo a integridade do sistema.

### Artigo Introdutório: Guia Essencial de Gestores de Pacotes Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, utilizar o gestor de pacotes da distribuição (APT ou DNF) para instalar três pacotes de software diferentes. Pesquisar por um pacote específico e verificar as suas dependências. (a ser detalhado na tarefa do Teams).

