# Recursos - Semana 10: Otimização de Recursos (Parte 2)

## Tópicos Abordados
*   Gestão de arranque de serviços.
*   Otimização de memória (swap).

## Objetivos de Aprendizagem
*   Otimizar o arranque do sistema.
*   Ajustar a utilização da memória swap.

## Material de Apoio

### Apresentação: Otimização de Arranque e Memória Swap

#### Slide 1: Título
*   **Título:** Otimização de Recursos em SO Open Source (Parte 2)
*   **Subtítulo:** Gestão de Arranque e Otimização de Memória Swap

#### Slide 2: Revisão da Otimização de Recursos
*   **Conteúdo:** Recapitulando a importância da otimização e a monitorização de processos. Foco na otimização do arranque e da memória.

#### Slide 3: Gestão de Arranque de Serviços
*   **Conteúdo:** O que são serviços (daemons). Como os serviços são iniciados no arranque do sistema. Systemd como sistema de inicialização padrão na maioria das distribuições Linux.

#### Slide 4: Comandos `systemctl` Essenciais
*   **Conteúdo:** `systemctl status`, `systemctl start`, `systemctl stop`, `systemctl enable`, `systemctl disable`. Exemplos práticos de como gerir serviços.

#### Slide 5: Identificando Serviços Desnecessários
*   **Conteúdo:** Como verificar quais serviços estão a ser executados e quais podem ser desativados para melhorar o tempo de arranque e o consumo de recursos.

#### Slide 6: Otimização da Memória Swap
*   **Conteúdo:** O que é a área de swap. Quando e como o sistema usa a swap. O parâmetro `swappiness`.

#### Slide 7: Ajustando `swappiness`
*   **Conteúdo:** Explicação do valor de `swappiness` (0 a 100). Como alterar o valor temporariamente e permanentemente (`/etc/sysctl.conf`). Impacto no desempenho.

#### Slide 8: Monitorização da Swap
*   **Conteúdo:** Comandos para verificar o uso da swap (`free -h`, `swapon -s`). Identificar se a swap está a ser usada excessivamente.

#### Slide 9: Considerações sobre o Tamanho da Partição Swap
*   **Conteúdo:** Recomendações para o tamanho da swap em diferentes cenários (pouca RAM, muita RAM, hibernação).

#### Slide 10: Conclusão
*   **Conteúdo:** A gestão eficiente do arranque de serviços e a otimização da memória swap são passos importantes para um sistema Open Source rápido e responsivo.

### Artigo Introdutório: Otimizando o Arranque e a Memória Swap no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, identificar serviços em execução e desativar um serviço desnecessário. Alterar o valor de `swappiness` e observar o impacto no uso da memória. (a ser detalhado na tarefa do Teams).

