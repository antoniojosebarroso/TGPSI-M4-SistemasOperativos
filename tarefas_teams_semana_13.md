# Tarefas Microsoft Teams - Semana 13: Configuração do Sistema - Rede (Parte 1)

## Título da Tarefa: Configuração Avançada de Endereçamento IP e DNS

## Descrição:
Nesta semana, vamos aprofundar a configuração de rede em Sistemas Operativos Open Source, focando no endereçamento IP (estático/dinâmico) e na configuração de DNS. A tarefa prática permitirá aos alunos configurar e testar a conectividade de rede de forma mais detalhada.

## Objetivos:
*   Configurar o endereçamento IP de uma interface de rede (estático e dinâmico).
*   Configurar servidores DNS para resolução de nomes.
*   Diagnosticar e resolver problemas básicos de conectividade de rede.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre configuração de rede - Parte 1).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Configuração de IP Dinâmico (DHCP):**
        *   Certifique-se de que a sua interface de rede está configurada para DHCP (geralmente é o padrão). Se configurou IP estático na semana anterior, reverta para DHCP (no Netplan, altere `dhcp4: no` para `dhcp4: yes` e remova as linhas de `addresses`, `routes` e `nameservers`). Aplique as alterações: `sudo netplan apply`.
        *   Verifique o endereço IP atribuído via DHCP: `ip a`.
        *   Verifique os servidores DNS atribuídos: `cat /etc/resolv.conf` ou `resolvectl status`.
    *   **Configuração de IP Estático (Revisão e Aprofundamento):**
        *   Configure novamente a sua interface de rede com um IP estático, utilizando um endereço IP diferente do usado na Semana 12 (ex: `192.168.1.101/24`).
        *   Defina dois servidores DNS públicos (ex: 1.1.1.1 e 8.8.8.8).
        *   Aplique as alterações e verifique o novo endereço IP e os servidores DNS.
    *   **Teste de Conectividade e Diagnóstico:**
        *   Teste a conectividade com um site externo (ex: `ping google.com`).
        *   Se o `ping` falhar, tente `ping 8.8.8.8` (para testar a conectividade IP) e `dig google.com @8.8.8.8` (para testar a resolução DNS diretamente). Analise os resultados para identificar a causa do problema.
        *   Use `ip r` para verificar a tabela de rotas e garantir que o gateway está correto.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o IP atribuído via DHCP e os servidores DNS.
    *   Captura de ecrã do ficheiro de configuração de rede (Netplan ou outro) com o IP estático configurado.
    *   Captura de ecrã do terminal mostrando os resultados dos testes de `ping` e `dig` após a configuração estática.
    *   Uma breve descrição de um problema de conectividade que simulou ou encontrou e como o diagnosticou e resolveu.

## Critérios de Avaliação:
*   **Configuração de Rede (50%):** A interface de rede deve estar corretamente configurada com IP dinâmico e estático, e os servidores DNS devem ser funcionais.
*   **Diagnóstico de Problemas (30%):** Capacidade de usar ferramentas de diagnóstico para identificar e resolver problemas de conectividade.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição dos problemas e soluções.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

