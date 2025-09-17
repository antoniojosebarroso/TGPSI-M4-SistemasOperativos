# Recursos - Semana 13: Configuração do Sistema - Rede (Parte 1)

## Tópicos Abordados
*   Configuração de endereçamento IP (estático/dinâmico).
*   Configuração de DNS.

## Objetivos de Aprendizagem
*   Configurar a rede básica do sistema.
*   Resolver problemas de conectividade.

## Material de Apoio

### Apresentação: Configuração de Rede Essencial

#### Slide 1: Título
*   **Título:** Configuração do Sistema - Rede (Parte 1)
*   **Subtítulo:** Endereçamento IP e DNS

#### Slide 2: Fundamentos de Rede no Linux
*   **Conteúdo:** Breve revisão dos conceitos de rede (IP, máscara de sub-rede, gateway, DNS). A importância da conectividade para um SO moderno.

#### Slide 3: Endereçamento IP Dinâmico (DHCP)
*   **Conteúdo:** Como o DHCP funciona. Vantagens (facilidade de configuração). Desvantagens (endereço IP pode mudar). Como verificar o IP via DHCP (`ip a`, `ifconfig`).

#### Slide 4: Endereçamento IP Estático
*   **Conteúdo:** Quando usar IP estático (servidores, dispositivos com acesso fixo). Como configurar IP estático via linha de comando e ficheiros de configuração.

#### Slide 5: Configuração de IP Estático (Exemplo Debian/Ubuntu)
*   **Conteúdo:** Edição do ficheiro `/etc/netplan/*.yaml` (Ubuntu Server 18.04+). Exemplo de configuração com IP, máscara, gateway e DNS.

#### Slide 6: Configuração de IP Estático (Exemplo CentOS/RHEL)
*   **Conteúdo:** Edição do ficheiro `/etc/sysconfig/network-scripts/ifcfg-eth0`. Exemplo de configuração.

#### Slide 7: Configuração de DNS (Domain Name System)
*   **Conteúdo:** O que é DNS e a sua função. Como configurar servidores DNS (`/etc/resolv.conf`, NetworkManager).

#### Slide 8: Testando a Conectividade de Rede
*   **Conteúdo:** Comandos essenciais: `ping` (verificar conectividade com IP), `ping google.com` (verificar DNS), `ip r` (tabela de rotas).

#### Slide 9: Resolução de Problemas Básicos de Rede
*   **Conteúdo:** Cenários comuns de problemas (IP incorreto, gateway errado, DNS não configurado). Ferramentas de diagnóstico (`ip`, `ping`, `traceroute`).

#### Slide 10: Conclusão
*   **Conteúdo:** A configuração correta da rede é fundamental para o funcionamento do sistema. Dominar a configuração de IP e DNS é uma habilidade essencial.

### Artigo Introdutório: Guia Completo de Configuração de Rede no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, configurar uma interface de rede com um endereço IP estático, máscara de sub-rede, gateway e servidores DNS. Testar a conectividade com a internet e com outros dispositivos na rede virtual. (a ser detalhado na tarefa do Teams).

