# Tarefas Microsoft Teams - Semana 20: Resolução de Problemas - Rede e Conectividade

## Título da Tarefa: Diagnóstico e Resolução de Problemas de Rede

## Descrição:
Nesta semana, vamos focar na resolução de problemas comuns relacionados com a rede e a conectividade em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos diagnosticar e resolver cenários de falha de rede.

## Objetivos:
*   Diagnosticar problemas de conectividade de rede.
*   Utilizar ferramentas de diagnóstico de rede como `ping`, `traceroute`, `netstat`, `ss`, `ip`.
*   Resolver problemas comuns de configuração de rede.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre resolução de problemas de rede).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Simulação de Problema de DNS:**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Edite o ficheiro `/etc/resolv.conf` e altere o servidor DNS para um endereço IP inválido (ex: `nameserver 1.2.3.4`).
        *   Tente aceder a um site pelo nome (ex: `ping google.com`). Deverá falhar.
        *   Tente aceder a um site pelo IP (ex: `ping 142.250.184.142`). Deverá funcionar.
        *   **Diagnóstico e Recuperação:** Use `dig google.com` para confirmar o problema de DNS. Corrija o ficheiro `/etc/resolv.conf` para o servidor DNS correto (ex: 8.8.8.8 ou o do seu router). Teste novamente.
    *   **Simulação de Problema de Gateway:**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Remova a rota padrão (gateway) da sua tabela de rotas: `sudo ip route del default`.
        *   Tente aceder a um site externo (ex: `ping google.com`). Deverá falhar.
        *   **Diagnóstico e Recuperação:** Use `ip r` para verificar a tabela de rotas. Adicione a rota padrão novamente: `sudo ip route add default via <IP_do_seu_gateway>`. Teste novamente.
    *   **Análise de Portas Abertas:**
        *   Use `ss -tuln` ou `netstat -tuln` para listar as portas TCP e UDP abertas no seu sistema. Identifique os serviços associados a essas portas.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o problema de DNS e a sua resolução.
    *   Captura de ecrã do terminal mostrando o problema de gateway e a sua resolução.
    *   Captura de ecrã do terminal mostrando a saída de `ss -tuln` ou `netstat -tuln`.
    *   Uma breve reflexão sobre a importância de saber diagnosticar problemas de rede para manter a conectividade do sistema.

## Critérios de Avaliação:
*   **Diagnóstico e Resolução (60%):** Capacidade de simular, diagnosticar e resolver problemas de DNS e gateway.
*   **Uso de Ferramentas (20%):** Demonstração correta do uso de ferramentas de diagnóstico de rede.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição dos problemas e soluções.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

