# Recursos - Semana 27: Segurança em Sistemas Open Source (Introdução)

## Tópicos Abordados
*   Princípios de segurança.
*   Atualizações de segurança.
*   Auditoria de logs.

## Objetivos de Aprendizagem
*   Compreender a importância da segurança.
*   Manter o sistema seguro através de atualizações.
*   Analisar logs de segurança.

## Material de Apoio

### Apresentação: Fundamentos de Segurança em SO Open Source

#### Slide 1: Título
*   **Título:** Segurança em Sistemas Open Source (Introdução)
*   **Subtítulo:** Princípios, Atualizações e Auditoria de Logs

#### Slide 2: A Importância da Segurança
*   **Conteúdo:** Porquê a segurança é crucial em qualquer sistema. A natureza aberta do Open Source e a segurança (muitos olhos, mas também potenciais vulnerabilidades).

#### Slide 3: Princípios Básicos de Segurança
*   **Conteúdo:** Confidencialidade, Integridade, Disponibilidade (CIA Triad). Menor privilégio, defesa em profundidade, segmentação.

#### Slide 4: Atualizações de Segurança
*   **Conteúdo:** A importância de manter o sistema e as aplicações atualizadas. Como as atualizações corrigem vulnerabilidades. Automatização de atualizações.

#### Slide 5: Gestão de Patches e Vulnerabilidades
*   **Conteúdo:** Como os gestores de pacotes ajudam na gestão de patches. Fontes de informação sobre vulnerabilidades (CVEs).

#### Slide 6: Auditoria de Logs
*   **Conteúdo:** O que são logs de sistema. A importância de monitorizar logs para detetar atividades suspeitas ou problemas de segurança.

#### Slide 7: Ficheiros de Log Essenciais
*   **Conteúdo:** `/var/log/syslog`, `/var/log/auth.log` (autenticação), `/var/log/kern.log` (kernel). Ferramentas para visualizar logs (`cat`, `tail`, `grep`, `journalctl`).

#### Slide 8: Ferramentas de Análise de Logs
*   **Conteúdo:** Introdução a ferramentas como `logwatch` ou `fail2ban` (breve menção).

#### Slide 9: Boas Práticas de Segurança
*   **Conteúdo:** Senhas fortes, firewall, desativar serviços desnecessários, backups, monitorização regular.

#### Slide 10: Conclusão
*   **Conteúdo:** A segurança é um processo contínuo. Compreender os princípios e manter o sistema atualizado e monitorizado são passos fundamentais.

### Artigo Introdutório: Guia de Segurança Básica para Sistemas Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, simular uma tentativa de login falhada e verificar o `/var/log/auth.log`. Configurar o sistema para receber notificações de atualizações de segurança. (a ser detalhado na tarefa do Teams).

