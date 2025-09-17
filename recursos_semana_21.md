# Recursos - Semana 21: Resolução de Problemas - Aplicações e Permissões

## Tópicos Abordados
*   Problemas de dependências de aplicações.
*   Erros de permissões.

## Objetivos de Aprendizagem
*   Resolver problemas de instalação de aplicações.
*   Corrigir erros de permissões.

## Material de Apoio

### Apresentação: Resolução de Problemas de Aplicações e Permissões

#### Slide 1: Título
*   **Título:** Resolução de Problemas - Aplicações e Permissões
*   **Subtítulo:** Diagnóstico e Correção no SO Open Source

#### Slide 2: Introdução aos Problemas de Aplicações
*   **Conteúdo:** Cenários comuns de falha de aplicações (não inicia, funciona incorretamente, erros durante a instalação). A importância de logs e mensagens de erro.

#### Slide 3: Problemas de Dependências
*   **Conteúdo:** O que são dependências de software. Como gestores de pacotes lidam com elas. Erros comuns de dependências ausentes ou conflitantes.

#### Slide 4: Diagnóstico de Dependências
*   **Conteúdo:** Ferramentas para verificar dependências (`apt-cache depends`, `dpkg -s`, `ldd`). Como resolver dependências manualmente ou com o gestor de pacotes (`apt install -f`).

#### Slide 5: Erros de Permissões em Aplicações
*   **Conteúdo:** Sintomas de problemas de permissões (aplicação não consegue ler/escrever ficheiros, não consegue iniciar, 


acesso negado). Onde procurar (logs da aplicação, `/var/log/syslog`).

#### Slide 6: Corrigindo Erros de Permissões
*   **Conteúdo:** Uso de `chmod` e `chown` para ajustar permissões e propriedade de ficheiros e diretórios. Precauções ao alterar permissões em ficheiros de sistema.

#### Slide 7: Logs de Aplicações
*   **Conteúdo:** Onde as aplicações guardam os seus logs (`/var/log/`, diretórios específicos da aplicação). Como ler e interpretar logs para identificar a causa dos problemas.

#### Slide 8: Ferramentas de Debugging
*   **Conteúdo:** Breve introdução a ferramentas como `strace` (rastrear chamadas de sistema) e `lsof` (listar ficheiros abertos) para diagnóstico avançado.

#### Slide 9: Boas Práticas para Evitar Problemas
*   **Conteúdo:** Manter o sistema atualizado. Instalar software de fontes confiáveis. Fazer backups regulares. Entender as permissões antes de alterar.

#### Slide 10: Conclusão
*   **Conteúdo:** A resolução de problemas de aplicações e permissões exige uma abordagem sistemática e o conhecimento das ferramentas de diagnóstico e correção.

### Artigo Introdutório: Guia de Resolução de Problemas de Aplicações e Permissões no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, simular um problema de dependência ao tentar instalar um pacote sem as suas dependências. Simular um erro de permissão ao tentar executar um script sem permissão de execução e corrigir o problema. (a ser detalhado na tarefa do Teams).

