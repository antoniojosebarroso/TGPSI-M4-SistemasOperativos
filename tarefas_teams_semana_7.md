# Tarefas Microsoft Teams - Semana 7: Instalação e Particionamento (Parte 2)

## Título da Tarefa: Instalação Prática com Particionamento Manual

## Descrição:
Nesta semana, vamos aplicar os conhecimentos teóricos de particionamento numa instalação prática de um Sistema Operativo Open Source. A tarefa consiste em instalar um SO numa máquina virtual, realizando o particionamento manual do disco.

## Objetivos:
*   Aplicar os conceitos de particionamento numa instalação real.
*   Criar e formatar partições de acordo com um plano pré-definido.
*   Instalar com sucesso um SO Open Source com particionamento manual.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre criação e formatação de partições).
2.  **Instalação Prática em VM:**
    *   Utilize a máquina virtual criada na Semana 5.
    *   Faça o download da imagem ISO de uma distribuição Linux (ex: Ubuntu Desktop 22.04 LTS).
    *   Inicie a instalação do SO na sua VM.
    *   No passo de particionamento, escolha a opção de particionamento manual (ou "Algo mais" no Ubuntu).
    *   Crie as seguintes partições, de acordo com o plano que elaborou na Semana 6 (ou um plano semelhante):
        *   **Partição Raiz (`/`):** Tamanho adequado (ex: 20GB), sistema de ficheiros ext4.
        *   **Partição Home (`/home`):** Tamanho adequado (ex: 25GB), sistema de ficheiros ext4.
        *   **Partição Swap:** Tamanho adequado (ex: 2GB).
    *   Prossiga com a instalação até ao fim.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do ecrã de particionamento manual, mostrando as partições que criou.
    *   Captura de ecrã do sistema operativo instalado e a funcionar.
    *   Captura de ecrã do resultado do comando `lsblk` ou `df -h` no terminal, para mostrar as partições montadas.
    *   Uma breve descrição dos desafios que encontrou durante o processo de particionamento manual.
4.  **Discussão no Fórum:** Partilhe no fórum da Semana 7 uma dica ou um problema que encontrou durante a instalação com particionamento manual, e como o resolveu.

## Critérios de Avaliação:
*   **Instalação e Particionamento (60%):** O SO deve estar instalado e a funcionar corretamente com o esquema de particionamento manual implementado.
*   **Relatório (20%):** Clareza das capturas de ecrã e da descrição dos desafios.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

