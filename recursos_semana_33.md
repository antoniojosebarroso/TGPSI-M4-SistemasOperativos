# Recursos - Semana 33: Gestão de Configuração (Introdução)

## Tópicos Abordados
*   Ansible (introdução).
*   Automatização de configurações.

## Objetivos de Aprendizagem
*   Compreender a gestão de configuração.
*   Utilizar Ansible para tarefas simples.

## Material de Apoio

### Apresentação: Introdução à Gestão de Configuração com Ansible

#### Slide 1: Título
*   **Título:** Gestão de Configuração (Introdução)
*   **Subtítulo:** Automatização com Ansible

#### Slide 2: O que é Gestão de Configuração?
*   **Conteúdo:** Definição e importância da gestão de configuração (consistência, escalabilidade, redução de erros). Exemplos de ferramentas (Ansible, Puppet, Chef).

#### Slide 3: Porquê Ansible?
*   **Conteúdo:** Simplicidade (baseado em SSH, sem agentes), fácil de aprender, poderoso, Open Source. Escrito em Python.

#### Slide 4: Arquitetura do Ansible
*   **Conteúdo:** Control Node (onde o Ansible é executado), Managed Nodes (servidores a serem configurados), Inventário (lista de hosts), Playbooks (instruções).

#### Slide 5: Inventário do Ansible
*   **Conteúdo:** O que é o ficheiro de inventário (`/etc/ansible/hosts`). Como definir grupos de hosts e variáveis.

#### Slide 6: Playbooks do Ansible
*   **Conteúdo:** O que são Playbooks (ficheiros YAML). Estrutura básica (hosts, tasks, handlers). Módulos do Ansible.

#### Slide 7: Módulos do Ansible
*   **Conteúdo:** Exemplos de módulos comuns (`apt`, `yum`, `service`, `copy`, `file`, `user`). Como os módulos executam tarefas nos Managed Nodes.

#### Slide 8: Exemplo de um Playbook Simples
*   **Conteúdo:** Playbook para instalar um pacote e iniciar um serviço (ex: Nginx).

#### Slide 9: Executando um Playbook
*   **Conteúdo:** Comando `ansible-playbook <nome_do_playbook.yml>`. Opções úteis (`--check`, `--diff`).

#### Slide 10: Conclusão
*   **Conteúdo:** Ansible é uma ferramenta essencial para automatizar a gestão de configuração, tornando a administração de sistemas mais eficiente e menos propensa a erros.

### Artigo Introdutório: Guia Essencial de Ansible para Iniciantes

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM (Control Node), instalar o Ansible. Criar um ficheiro de inventário e um playbook simples para instalar um pacote (ex: `htop`) numa outra VM (Managed Node). Executar o playbook. (a ser detalhado na tarefa do Teams).

