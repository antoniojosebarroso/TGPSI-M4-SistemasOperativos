# Recursos - Semana 24: Instalação de Aplicativos - Compilação a partir do Código Fonte

## Tópicos Abordados
*   Noções de compilação de software (make, configure).
*   Instalação de ferramentas de desenvolvimento.

## Objetivos de Aprendizagem
*   Compilar e instalar software a partir do código fonte.
*   Compreender o processo de compilação.

## Material de Apoio

### Apresentação: Compilando Software no Linux

#### Slide 1: Título
*   **Título:** Instalação de Aplicativos - Compilação a partir do Código Fonte
*   **Subtítulo:** Entendendo o Processo de Construção de Software

#### Slide 2: Porquê Compilar do Código Fonte?
*   **Conteúdo:** Vantagens (otimização, acesso a versões mais recentes, personalização, aprender como funciona). Desvantagens (complexidade, tempo, dependências).

#### Slide 3: Ferramentas Essenciais de Desenvolvimento
*   **Conteúdo:** `build-essential` (Debian/Ubuntu) ou `Development Tools` (Red Hat/CentOS). Compiladores (GCC), `make`, `autoconf`, `automake`, `libtool`.

#### Slide 4: O Processo Típico de Compilação (`./configure`, `make`, `make install`)
*   **Conteúdo:** Explicação das três etapas principais para compilar e instalar a maioria dos softwares Open Source.

#### Slide 5: `./configure` - Preparando a Compilação
*   **Conteúdo:** O que faz o script `configure` (verifica dependências, configura o `Makefile`). Opções comuns (`--prefix`, `--enable-feature`).

#### Slide 6: `make` - Compilando o Código
*   **Conteúdo:** O que faz o comando `make` (lê o `Makefile` e compila o código fonte). Como o `Makefile` define as regras de compilação.

#### Slide 7: `make install` - Instalando o Software
*   **Conteúdo:** O que faz o comando `make install` (copia os ficheiros compilados para os diretórios do sistema). A importância de saber onde os ficheiros são instalados.

#### Slide 8: Resolução de Problemas de Compilação
*   **Conteúdo:** Erros comuns (dependências ausentes, erros de sintaxe no código, problemas de configuração). Como ler mensagens de erro.

#### Slide 9: Desinstalação de Software Compilado
*   **Conteúdo:** `make uninstall` (se disponível). Remoção manual dos ficheiros instalados. A complexidade da desinstalação de software compilado.

#### Slide 10: Conclusão
*   **Conteúdo:** Compilar software do código fonte é uma habilidade avançada que oferece grande flexibilidade e controlo, mas exige um bom entendimento do processo.

### Artigo Introdutório: Guia Prático de Compilação de Software no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, instalar as ferramentas de desenvolvimento necessárias. Fazer o download do código fonte de uma aplicação simples (ex: `htop` ou `neofetch`) e compilá-la e instalá-la a partir do código fonte. (a ser detalhado na tarefa do Teams).

