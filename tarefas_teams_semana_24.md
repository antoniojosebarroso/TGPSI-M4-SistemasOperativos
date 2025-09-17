# Tarefas Microsoft Teams - Semana 24: Instalação de Aplicativos - Compilação a partir do Código Fonte

## Título da Tarefa: Compilando e Gerenciando Software Personalizado

## Descrição:
Nesta semana, vamos aprofundar a instalação de software a partir do código fonte, compreendendo o ciclo de vida de um programa compilado e as ferramentas necessárias. A tarefa prática permitirá aos alunos compilar e instalar um programa, e gerir as suas dependências.

## Objetivos:
*   Compreender o processo completo de compilação de software a partir do código fonte.
*   Identificar e resolver dependências de compilação.
*   Gerir software instalado manualmente.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre compilação a partir do código fonte).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Preparação:** Certifique-se de que tem as ferramentas de compilação instaladas (`build-essential`).
    *   **Download do Código Fonte:** Escolha um programa Open Source simples para compilar. Sugestões:
        *   `figlet` (gerador de arte ASCII)
        *   `sl` (locomotiva a vapor no terminal)
        *   `fortune` (citações aleatórias)
        Faça o download do código fonte (geralmente um ficheiro `.tar.gz` ou `.zip`) de um site como GitHub ou SourceForge.
    *   **Compilação e Instalação:**
        *   Descompacte o ficheiro: `tar -xvzf <nome_do_ficheiro.tar.gz>`.
        *   Navegue para o diretório descompactado.
        *   Leia o ficheiro `README` ou `INSTALL` para obter instruções específicas de compilação (os passos `./configure`, `make`, `sudo make install` são comuns, mas podem variar).
        *   Execute os comandos de compilação e instalação. Se encontrar erros de dependência, pesquise como instalar as bibliotecas ou pacotes de desenvolvimento necessários (geralmente terminam em `-dev` ou `-devel`).
    *   **Verificação:** Após a instalação, verifique se o programa funciona corretamente executando-o no terminal.
    *   **Remoção (Opcional):** Se o programa tiver um `Makefile` com a opção `uninstall`, pode tentar `sudo make uninstall`. Caso contrário, anote os ficheiros instalados para remoção manual.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o download e descompactação do código fonte.
    *   Captura de ecrã do terminal mostrando os comandos de compilação e instalação (incluindo a instalação de quaisquer dependências que tenha encontrado).
    *   Captura de ecrã do terminal mostrando a execução bem-sucedida do programa compilado.
    *   Uma breve reflexão sobre a complexidade e os benefícios de compilar software a partir do código fonte, especialmente em comparação com a instalação via gestores de pacotes.

## Critérios de Avaliação:
*   **Compilação e Instalação (60%):** O programa deve ser compilado e instalado com sucesso, e as dependências devem ser resolvidas.
*   **Resolução de Problemas (20%):** Capacidade de identificar e resolver erros de compilação ou dependências.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

