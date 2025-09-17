# Recursos - Semana 6: Instalação e Particionamento (Parte 1)

## Tópicos Abordados
*   Início do processo de instalação.
*   Conceitos de particionamento (MBR vs GPT, partições primárias, estendidas, lógicas).

## Objetivos de Aprendizagem
*   Compreender a importância do particionamento.
*   Diferenciar os tipos de tabelas de partições.

## Material de Apoio

### Apresentação: Fundamentos de Particionamento de Disco

#### Slide 1: Título
*   **Título:** Instalação e Particionamento de SO Open Source (Parte 1)
*   **Subtítulo:** Conceitos Essenciais de Particionamento

#### Slide 2: O Processo de Instalação
*   **Conteúdo:** Visão geral das etapas de instalação de um SO Open Source. A importância da preparação e do particionamento.

#### Slide 3: O que é Particionamento?
*   **Conteúdo:** Divisão física ou lógica de um disco rígido em várias seções. Razões para particionar (organização, segurança, múltiplos SOs).

#### Slide 4: Master Boot Record (MBR)
*   **Conteúdo:** Histórico, estrutura (boot loader, tabela de partições). Limitações (4 partições primárias, 2TB de tamanho máximo).

#### Slide 5: GUID Partition Table (GPT)
*   **Conteúdo:** Sucessor do MBR. Vantagens (suporte a mais de 4 partições primárias, discos maiores que 2TB, redundância). Associado a UEFI.

#### Slide 6: Tipos de Partições (MBR)
*   **Conteúdo:** Partições Primárias, Partições Estendidas, Partições Lógicas. Como contornar a limitação de 4 partições primárias com partições estendidas.

#### Slide 7: Tipos de Partições (GPT)
*   **Conteúdo:** Todas as partições são primárias. Sem as limitações do MBR.

#### Slide 8: Esquemas de Particionamento Comuns
*   **Conteúdo:** Exemplos de como particionar um disco para um SO Open Source (ex: /, /home, swap).

#### Slide 9: Ferramentas de Particionamento
*   **Conteúdo:** GParted, fdisk, parted. Breve introdução às ferramentas que serão usadas.

#### Slide 10: Conclusão
*   **Conteúdo:** A escolha do esquema de particionamento é crucial para a estabilidade e flexibilidade do sistema. MBR vs GPT e seus casos de uso.

### Artigo Introdutório: Guia Essencial de Particionamento de Disco

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Pesquisa e discussão sobre as diferenças práticas entre MBR e GPT e quando usar cada um. (a ser detalhado na tarefa do Teams).

