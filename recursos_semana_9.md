# Recursos - Semana 9: Otimização de Recursos (Parte 1)

## Tópicos Abordados
*   Gestão de processos (top, htop, kill).
*   Monitorização de recursos (CPU, memória).

## Objetivos de Aprendizagem
*   Monitorizar o uso de recursos do sistema.
*   Gerir processos em execução.

## Material de Apoio

### Apresentação: Monitorização e Gestão de Processos

#### Slide 1: Título
*   **Título:** Otimização de Recursos em SO Open Source (Parte 1)
*   **Subtítulo:** Monitorização e Gestão de Processos

#### Slide 2: Porquê Otimizar Recursos?
*   **Conteúdo:** Importância da otimização para desempenho, estabilidade e eficiência. Identificação de gargalos.

#### Slide 3: O que é um Processo?
*   **Conteúdo:** Definição de processo. Diferença entre processo e programa. Estados de um processo (execução, espera, parado).

#### Slide 4: `top` - Monitorização em Tempo Real
*   **Conteúdo:** Explicação das informações exibidas (PID, USER, %CPU, %MEM, TIME+, COMMAND). Ordenação e filtros.

#### Slide 5: `htop` - Uma Alternativa Interativa
*   **Conteúdo:** Vantagens do `htop` (interface colorida, fácil de usar, funcionalidades adicionais como árvores de processos e kills interativos).

#### Slide 6: Gestão de Processos com `ps`
*   **Conteúdo:** Comandos `ps aux`, `ps -ef`. Filtragem de processos. Obtenção de informações detalhadas sobre processos.

#### Slide 7: Controlando Processos com `kill`
*   **Conteúdo:** Sinais (SIGTERM, SIGKILL, SIGHUP). Uso do comando `kill`, `killall`, `pkill`. Exemplo de como terminar um processo problemático.

#### Slide 8: Monitorização de CPU
*   **Conteúdo:** Entender o uso da CPU. Identificar processos que consomem muita CPU. Load Average.

#### Slide 9: Monitorização de Memória
*   **Conteúdo:** Uso de RAM e Swap. Comandos `free -h`, `vmstat`. Identificar processos que consomem muita memória.

#### Slide 10: Conclusão
*   **Conteúdo:** A monitorização e gestão de processos são habilidades essenciais para administradores de sistemas. Ferramentas como `top`, `htop` e `kill` são indispensáveis.

### Artigo Introdutório: Guia Prático de Monitorização de Recursos Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Utilizar os comandos `top`, `htop` e `ps` para monitorizar os processos e o uso de recursos numa VM. Identificar e terminar um processo específico usando `kill`. (a ser detalhado na tarefa do Teams).

