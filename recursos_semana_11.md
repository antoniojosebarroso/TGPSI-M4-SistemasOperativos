# Recursos - Semana 11: Instalação de Dispositivos e Device Drivers (Parte 1)

## Tópicos Abordados
*   Identificação de hardware (lspci, lsusb).
*   Noções de módulos de kernel.

## Objetivos de Aprendizagem
*   Identificar o hardware instalado.
*   Compreender o papel dos módulos de kernel.

## Material de Apoio

### Apresentação: Hardware e Drivers no Linux

#### Slide 1: Título
*   **Título:** Instalação de Dispositivos e Device Drivers (Parte 1)
*   **Subtítulo:** Identificação de Hardware e Módulos de Kernel

#### Slide 2: Como o Linux Interage com o Hardware?
*   **Conteúdo:** Introdução ao conceito de drivers de dispositivo. A importância do kernel na gestão de hardware.

#### Slide 3: Identificação de Hardware com `lspci`
*   **Conteúdo:** Uso do comando `lspci` para listar dispositivos PCI (placas gráficas, placas de rede, controladores de armazenamento). Opções úteis (`-v`, `-k`).

#### Slide 4: Identificação de Hardware com `lsusb`
*   **Conteúdo:** Uso do comando `lsusb` para listar dispositivos USB (pen drives, impressoras, webcams). Opções úteis (`-v`).

#### Slide 5: Outras Ferramentas de Identificação de Hardware
*   **Conteúdo:** `lshw` (informações detalhadas de hardware), `dmidecode` (informações da BIOS/UEFI), `hwinfo`.

#### Slide 6: O que são Módulos de Kernel?
*   **Conteúdo:** Pequenos pedaços de código que podem ser carregados e descarregados do kernel em tempo de execução. Permitem adicionar suporte a hardware sem recompilar o kernel.

#### Slide 7: Gestão de Módulos de Kernel com `lsmod`
*   **Conteúdo:** Uso do comando `lsmod` para listar os módulos de kernel atualmente carregados. Entender a saída do comando.

#### Slide 8: Gestão de Módulos de Kernel com `modprobe` e `rmmod`
*   **Conteúdo:** Carregar (`modprobe`) e descarregar (`rmmod`) módulos de kernel. Casos de uso e precauções.

#### Slide 9: Onde os Módulos de Kernel Estão Armazenados?
*   **Conteúdo:** O diretório `/lib/modules/<kernel-version>`. O ficheiro `modules.dep`.

#### Slide 10: Conclusão
*   **Conteúdo:** A capacidade de identificar hardware e gerir módulos de kernel é fundamental para a instalação e configuração de drivers em sistemas Open Source.

### Artigo Introdutório: Guia para Identificação de Hardware e Gestão de Módulos de Kernel no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, utilizar os comandos `lspci`, `lsusb` e `lsmod` para identificar o hardware virtualizado e os módulos de kernel carregados. (a ser detalhado na tarefa do Teams).

