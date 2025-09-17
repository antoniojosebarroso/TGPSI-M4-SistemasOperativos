# Recursos - Semana 30: Monitorização e Logs

## Tópicos Abordados
*   Ferramentas de monitorização (Nagios, Zabbix - introdução).
*   Análise de logs (journalctl, rsyslog).

## Objetivos de Aprendizagem
*   Monitorizar o estado do sistema.
*   Analisar logs para diagnóstico.

## Material de Apoio

### Apresentação: Monitorização e Análise de Logs no Linux

#### Slide 1: Título
*   **Título:** Monitorização e Logs
*   **Subtítulo:** Mantendo o Sistema Saudável e Identificando Problemas

#### Slide 2: A Importância da Monitorização
*   **Conteúdo:** Porquê monitorizar (desempenho, disponibilidade, segurança). Identificação proativa de problemas. Planeamento de capacidade.

#### Slide 3: Ferramentas de Monitorização (Introdução)
*   **Conteúdo:** Nagios (monitorização de infraestrutura), Zabbix (monitorização distribuída, gráficos). Breve visão geral das suas capacidades.

#### Slide 4: Monitorização Local com `top`/`htop` e `free`
*   **Conteúdo:** Revisão de ferramentas já conhecidas para monitorização em tempo real de CPU, memória e processos.

#### Slide 5: Monitorização de Disco com `df` e `du`
*   **Conteúdo:** Uso de `df -h` para verificar o espaço em disco. Uso de `du -sh` para verificar o tamanho de diretórios.

#### Slide 6: O que são Logs?
*   **Conteúdo:** Registos de eventos do sistema e aplicações. A importância dos logs para auditoria, diagnóstico e segurança.

#### Slide 7: `rsyslog` - O Serviço de Logging Tradicional
*   **Conteúdo:** Como `rsyslog` funciona. Ficheiros de configuração (`/etc/rsyslog.conf`). Onde os logs são armazenados (`/var/log/`).

#### Slide 8: `journalctl` - O Cliente do Systemd Journal
*   **Conteúdo:** Como usar `journalctl` para consultar o journal do systemd. Opções úteis (`-f`, `-u`, `-p`, `--since`, `--until`).

#### Slide 9: Análise de Logs com `grep`
*   **Conteúdo:** Uso do comando `grep` para filtrar informações relevantes em ficheiros de log. Exemplos práticos.

#### Slide 10: Conclusão
*   **Conteúdo:** A monitorização contínua e a análise de logs são práticas essenciais para garantir a estabilidade, desempenho e segurança de sistemas Open Source.

### Artigo Introdutório: Guia de Monitorização e Análise de Logs no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, usar `df`, `du` e `journalctl` para monitorizar o uso de disco e analisar os logs do sistema. Filtrar logs para encontrar eventos específicos. (a ser detalhado na tarefa do Teams).

