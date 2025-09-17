# Recursos - Semana 12: Instalação de Dispositivos e Device Drivers (Parte 2)

## Tópicos Abordados
*   Instalação de drivers proprietários (ex: placas gráficas).
*   Configuração de dispositivos de rede.

## Objetivos de Aprendizagem
*   Instalar drivers adicionais.
*   Configurar interfaces de rede.

## Material de Apoio

### Apresentação: Configurando Drivers e Rede

#### Slide 1: Título
*   **Título:** Instalação de Dispositivos e Device Drivers (Parte 2)
*   **Subtítulo:** Drivers Proprietários e Configuração de Rede

#### Slide 2: Drivers Proprietários vs. Open Source
*   **Conteúdo:** Diferenças entre drivers Open Source (geralmente incluídos no kernel) e drivers proprietários (fornecidos pelos fabricantes). Razões para usar drivers proprietários (desempenho, funcionalidades).

#### Slide 3: Instalação de Drivers de Placa Gráfica (NVIDIA/AMD)
*   **Conteúdo:** Métodos de instalação (repositórios oficiais, PPA, download direto do fabricante). Cuidados a ter (compatibilidade, conflitos).

#### Slide 4: Verificação da Instalação do Driver
*   **Conteúdo:** Comandos para verificar se o driver foi instalado corretamente (ex: `nvidia-smi`, `glxinfo`).

#### Slide 5: Configuração de Dispositivos de Rede
*   **Conteúdo:** Introdução às interfaces de rede (Ethernet, Wi-Fi). Nomes das interfaces (eth0, wlan0, enpXsY).

#### Slide 6: Ferramentas de Configuração de Rede
*   **Conteúdo:** `ip` (substituto moderno do `ifconfig`), `nmcli` (NetworkManager CLI), `nmtui` (NetworkManager TUI).

#### Slide 7: Configuração de IP Estático
*   **Conteúdo:** Como configurar um endereço IP estático, máscara de sub-rede, gateway e DNS via linha de comando e ficheiros de configuração (`/etc/netplan/` no Ubuntu, `/etc/sysconfig/network-scripts/` no CentOS).

#### Slide 8: Configuração de Wi-Fi
*   **Conteúdo:** Conectar a redes Wi-Fi via linha de comando (`nmcli dev wifi connect`) e ferramentas gráficas.

#### Slide 9: Resolução de Problemas Básicos de Rede
*   **Conteúdo:** `ping`, `ip a`, `ip r`, `resolvectl`. Diagnóstico de problemas de conectividade.

#### Slide 10: Conclusão
*   **Conteúdo:** A instalação de drivers proprietários e a configuração de rede são passos cruciais para garantir o funcionamento completo e a conectividade do SO Open Source.

### Artigo Introdutório: Guia para Instalação de Drivers e Configuração de Rede no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, simular a instalação de um driver proprietário (ex: usando um driver genérico ou um pacote de teste). Configurar uma interface de rede com IP estático e testar a conectividade. (a ser detalhado na tarefa do Teams).

