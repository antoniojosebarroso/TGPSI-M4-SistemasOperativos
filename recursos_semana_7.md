# Recursos - Semana 7: Instalação e Particionamento (Parte 2)

## Tópicos Abordados
*   Criação de partições (/, /home, swap).
*   Formatação de partições (ext4, XFS).

## Objetivos de Aprendizagem
*   Criar e formatar partições de acordo com um plano.
*   Selecionar o sistema de ficheiros adequado.

## Material de Apoio

### Apresentação: Criando e Formatando Partições

#### Slide 1: Título
*   **Título:** Instalação e Particionamento de SO Open Source (Parte 2)
*   **Subtítulo:** Criação e Formatação de Partições Essenciais

#### Slide 2: Revisão: Esquema de Particionamento
*   **Conteúdo:** Relembrar a importância de um plano de particionamento. Partições comuns em Linux: raiz (`/`), home (`/home`), swap.

#### Slide 3: Partição Raiz (`/`)
*   **Conteúdo:** Onde todo o sistema de ficheiros Linux começa. Contém o sistema operativo, programas e configurações. Importância do tamanho adequado.

#### Slide 4: Partição Home (`/home`)
*   **Conteúdo:** Onde os dados dos utilizadores são armazenados. Vantagens de ter uma partição `/home` separada (reinstalação do SO, backups).

#### Slide 5: Partição Swap
*   **Conteúdo:** Área de troca utilizada quando a RAM está cheia. Tamanho recomendado (geralmente 1x a 2x a RAM, ou conforme as necessidades).

#### Slide 6: Sistemas de Ficheiros para Linux
*   **Conteúdo:** Introdução aos sistemas de ficheiros mais comuns: ext4 (padrão, robusto), XFS (alto desempenho, escalabilidade), Btrfs (funcionalidades avançadas).

#### Slide 7: Formatação de Partições
*   **Conteúdo:** O que é formatar uma partição. Comandos básicos para formatar (ex: `mkfs.ext4`, `mkswap`).

#### Slide 8: Montagem de Partições
*   **Conteúdo:** O que é montar uma partição. O ficheiro `/etc/fstab`. Montagem automática no arranque.

#### Slide 9: Processo Prático de Particionamento e Formatação
*   **Conteúdo:** Demonstração passo a passo usando uma ferramenta gráfica (ex: instalador do Ubuntu) ou linha de comando (fdisk/parted + mkfs).

#### Slide 10: Conclusão
*   **Conteúdo:** A criação e formatação correta das partições são passos críticos para uma instalação bem-sucedida e um sistema estável. Escolha informada do sistema de ficheiros.

### Artigo Introdutório: Guia Prático de Criação e Formatação de Partições Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Instalação inicial de um SO Open Source em VM, realizando o particionamento manual com partições /, /home e swap, e escolhendo o sistema de ficheiros ext4. (a ser detalhado na tarefa do Teams).

