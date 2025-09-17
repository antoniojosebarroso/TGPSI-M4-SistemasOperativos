# Recursos - Semana 20: Resolução de Problemas - Rede e Conectividade

## Tópicos Abordados
*   Diagnóstico de problemas de rede (ping, traceroute, netstat).
*   Resolução de problemas de DNS.

## Objetivos de Aprendizagem
*   Diagnosticar e resolver problemas de conectividade de rede.
*   Utilizar ferramentas de diagnóstico.

## Material de Apoio

### Apresentação: Diagnóstico e Resolução de Problemas de Rede

#### Slide 1: Título
*   **Título:** Resolução de Problemas - Rede e Conectividade
*   **Subtítulo:** Ferramentas e Técnicas de Diagnóstico no Linux

#### Slide 2: Introdução aos Problemas de Rede
*   **Conteúdo:** A importância da conectividade de rede. Cenários comuns de falha de rede (sem internet, não consegue aceder a um servidor, etc.).

#### Slide 3: `ping` - Testando a Conectividade Básica
*   **Conteúdo:** Como usar `ping` para verificar a acessibilidade de um host. Opções (`-c`, `-i`). Interpretação dos resultados.

#### Slide 4: `traceroute` / `tracepath` - Rastreando a Rota
*   **Conteúdo:** Como `traceroute` funciona para mostrar o caminho que os pacotes percorrem até um destino. Identificação de pontos de falha na rede.

#### Slide 5: `netstat` / `ss` - Conexões e Portas
*   **Conteúdo:** Uso de `netstat` (ou `ss` como alternativa moderna) para listar conexões de rede ativas, portas abertas e estatísticas de rede. Opções úteis (`-tulnp`).

#### Slide 6: `ip` - Informações Detalhadas da Interface
*   **Conteúdo:** Uso do comando `ip` para ver endereços IP, rotas, estado das interfaces de rede. (`ip a`, `ip r`, `ip link`).

#### Slide 7: Resolução de Problemas de DNS
*   **Conteúdo:** Sintomas de problemas de DNS (não consegue aceder a sites por nome, mas consegue por IP). Verificação do `/etc/resolv.conf`.

#### Slide 8: Ferramentas de Consulta DNS (`dig`, `nslookup`)
*   **Conteúdo:** Como usar `dig` e `nslookup` para consultar servidores DNS e diagnosticar problemas de resolução de nomes.

#### Slide 9: Reiniciar Serviços de Rede
*   **Conteúdo:** Quando e como reiniciar serviços de rede (`systemctl restart NetworkManager`, `systemctl restart networking`).

#### Slide 10: Conclusão
*   **Conteúdo:** O domínio das ferramentas de diagnóstico de rede é essencial para manter a conectividade e resolver problemas rapidamente em sistemas Open Source.

### Artigo Introdutório: Guia de Diagnóstico e Resolução de Problemas de Rede no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, simular um problema de rede (ex: configurar um DNS incorreto ou bloquear uma porta com firewall) e usar as ferramentas aprendidas para diagnosticar e resolver o problema. (a ser detalhado na tarefa do Teams).

