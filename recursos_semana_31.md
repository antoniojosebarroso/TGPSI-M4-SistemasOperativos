# Recursos - Semana 31: Automação de Tarefas

## Tópicos Abordados
*   Cron jobs.
*   Scripts shell para automação.

## Objetivos de Aprendizagem
*   Automatizar tarefas repetitivas.
*   Escrever scripts shell básicos.

## Material de Apoio

### Apresentação: Automação de Tarefas no Linux

#### Slide 1: Título
*   **Título:** Automação de Tarefas
*   **Subtítulo:** Cron Jobs e Shell Scripting para Eficiência

#### Slide 2: A Importância da Automação
*   **Conteúdo:** Porquê automatizar (redução de erros, economia de tempo, execução consistente). Exemplos de tarefas automatizáveis.

#### Slide 3: Cron - Agendamento de Tarefas
*   **Conteúdo:** O que é Cron. Sua função no agendamento de comandos e scripts para execução em horários específicos. O daemon `crond`.

#### Slide 4: `crontab` - Editando a Tabela Cron
*   **Conteúdo:** Uso do comando `crontab -e` para editar a tabela de tarefas do utilizador. Sintaxe das entradas cron (minuto, hora, dia do mês, mês, dia da semana, comando).

#### Slide 5: Exemplos de Cron Jobs
*   **Conteúdo:** Executar um script diariamente, semanalmente, a cada hora. Redirecionamento de saída. Variáveis de ambiente.

#### Slide 6: Introdução ao Shell Scripting
*   **Conteúdo:** O que é um script shell. Vantagens (automatização, portabilidade, flexibilidade). O shebang (`#!/bin/bash`).

#### Slide 7: Elementos Básicos de um Script Shell
*   **Conteúdo:** Variáveis, comandos, estruturas de controlo (if/else, for/while), entrada/saída de dados.

#### Slide 8: Criando um Script Simples
*   **Conteúdo:** Exemplo de um script para fazer backup de um diretório ou verificar o espaço em disco. Permissões de execução (`chmod +x`).

#### Slide 9: Boas Práticas em Shell Scripting
*   **Conteúdo:** Comentários, tratamento de erros, validação de entrada, uso de funções.

#### Slide 10: Conclusão
*   **Conteúdo:** A automação de tarefas com cron jobs e shell scripting é uma habilidade poderosa para qualquer administrador de sistemas Linux, aumentando a eficiência e a confiabilidade.

### Artigo Introdutório: Guia Completo de Automação de Tarefas no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, criar um cron job para executar um script shell simples (ex: que registe a data e hora num ficheiro de log) a cada 5 minutos. Criar um script shell que verifique o espaço em disco e envie um alerta se estiver abaixo de um limite. (a ser detalhado na tarefa do Teams).

