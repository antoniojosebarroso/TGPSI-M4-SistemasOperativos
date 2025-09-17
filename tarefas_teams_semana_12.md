# Tarefas Microsoft Teams - Semana 12: Instalação de Dispositivos e Device Drivers (Parte 2)

## Título da Tarefa: Instalação de Drivers e Configuração de Rede

## Descrição:
Nesta semana, vamos focar na instalação de drivers adicionais e na configuração de dispositivos de rede. A tarefa prática permitirá aos alunos simular a instalação de um driver proprietário e configurar uma interface de rede com IP estático.

## Objetivos:
*   Instalar drivers adicionais (proprietários ou genéricos).
*   Configurar interfaces de rede com IP estático.
*   Testar a conectividade de rede.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre drivers proprietários e configuração de rede).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop), execute os seguintes passos:
    *   **Simulação de Instalação de Driver:**
        *   Para simular a instalação de um driver proprietário, vamos instalar um pacote que geralmente requer drivers adicionais, como o `mesa-utils` para testar a aceleração 3D (embora não seja um driver proprietário, serve para o propósito de instalação de software relacionado a hardware).
        *   Instale o pacote: `sudo apt install mesa-utils`.
        *   Verifique a aceleração 3D: `glxinfo | grep "OpenGL renderer"` e `glxgears`.
        *   **Alternativa (se aplicável e com cuidado):** Se tiver uma placa NVIDIA, pode tentar instalar os drivers proprietários via `ubuntu-drivers autoinstall` ou manualmente (apenas se souber o que está a fazer e tiver um snapshot da VM).
    *   **Configuração de IP Estático:**
        *   Identifique a sua interface de rede principal (ex: `enp0s3` ou `eth0`) usando `ip a`.
        *   Edite o ficheiro de configuração de rede para definir um IP estático. No Ubuntu 20.04+, use Netplan. Crie ou edite um ficheiro `.yaml` em `/etc/netplan/` (ex: `01-netcfg.yaml`).
        *   Exemplo de configuração Netplan (substitua os valores pelos da sua rede virtual):
            ```yaml
            network:
              version: 2
              renderer: networkd
              ethernets:
                enp0s3: # Substitua pelo nome da sua interface
                  dhcp4: no
                  addresses: [192.168.1.100/24] # Seu IP estático e máscara
                  routes:
                    - to: default
                      via: 192.168.1.1 # Seu gateway
                  nameservers:
                    addresses: [8.8.8.8, 8.8.4.4] # Servidores DNS
            ```
        *   Aplique as alterações: `sudo netplan apply`.
        *   Verifique o novo endereço IP: `ip a`.
    *   **Teste de Conectividade:**
        *   Teste a conectividade com a internet: `ping google.com`.
        *   Teste a conectividade com o gateway: `ping 192.168.1.1` (substitua pelo seu gateway).
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o resultado da instalação do `mesa-utils` e do `glxinfo`.
    *   Captura de ecrã do ficheiro de configuração Netplan editado.
    *   Captura de ecrã do terminal mostrando o `ip a` após a aplicação das configurações de IP estático.
    *   Captura de ecrã do terminal mostrando os resultados dos testes de `ping`.
    *   Uma breve reflexão sobre a importância de configurar corretamente os drivers e a rede para o funcionamento pleno do sistema.

## Critérios de Avaliação:
*   **Execução dos Comandos (50%):** Demonstração correta da instalação de software relacionado a drivers e da configuração de IP estático.
*   **Relatório (30%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

