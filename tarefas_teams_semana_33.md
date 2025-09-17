# Tarefas Microsoft Teams - Semana 33: Gestão de Configuração (Introdução)

## Título da Tarefa: Automatizando Configurações com Ansible

## Descrição:
Nesta semana, vamos introduzir a gestão de configuração com Ansible, uma ferramenta poderosa para automatizar a configuração de múltiplos servidores. A tarefa prática permitirá aos alunos instalar o Ansible, criar um inventário e um playbook simples para configurar uma máquina remota.

## Objetivos:
*   Compreender os princípios da gestão de configuração.
*   Instalar e configurar o Ansible.
*   Criar um inventário de hosts.
*   Escrever e executar um playbook Ansible para automatizar tarefas.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre Ansible).
2.  **Exercícios Práticos em VM:** Numa máquina virtual (Control Node - ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Preparação:**
        *   Crie uma segunda VM (Managed Node - ex: Ubuntu Server) e certifique-se de que consegue aceder a ela via SSH a partir do Control Node (pode ser necessário instalar `openssh-server` no Managed Node e configurar a rede para que as VMs se comuniquem).
        *   Instale o Ansible no Control Node: `sudo apt update && sudo apt install ansible`.
    *   **Criação de Inventário:**
        *   Crie um ficheiro de inventário chamado `hosts.ini` no seu diretório home com o seguinte conteúdo (substitua `<IP_do_Managed_Node>` pelo IP da sua segunda VM):
            ```ini
            [webservers]
            managed_node ansible_host=<IP_do_Managed_Node> ansible_user=<seu_utilizador_no_managed_node> ansible_ssh_private_key_file=~/.ssh/id_rsa
            ```
        *   **Opcional:** Se não tiver chaves SSH configuradas, pode usar `ansible_password=<sua_senha_no_managed_node>` (não recomendado para produção).
        *   Teste a conectividade: `ansible -i hosts.ini webservers -m ping`.
    *   **Criação e Execução de Playbook:**
        *   Crie um playbook chamado `install_nginx.yml` no seu diretório home com o seguinte conteúdo:
            ```yaml
            ---
            - name: Instalar e configurar Nginx
              hosts: webservers
              become: yes
              tasks:
                - name: Atualizar cache de pacotes apt
                  apt: update_cache=yes

                - name: Instalar Nginx
                  apt: name=nginx state=present

                - name: Iniciar e ativar Nginx
                  service: name=nginx state=started enabled=yes

                - name: Copiar página index.html personalizada
                  copy:
                    content: 



                      src: /home/<seu_utilizador>/my_custom_index.html
                      dest: /var/www/html/index.html

            ```
        *   Crie um ficheiro `my_custom_index.html` no seu Control Node (no mesmo diretório do playbook) com o conteúdo que desejar (ex: `<h1>Olá do Ansible!</h1>`).
        *   Execute o playbook: `ansible-playbook -i hosts.ini install_nginx.yml`.
        *   **No seu navegador (no sistema anfitrião ou numa terceira VM):** Aceda ao endereço IP do Managed Node. Deverá ver a página web personalizada.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o teste de conectividade do Ansible (`ansible -i hosts.ini webservers -m ping`).
    *   Captura de ecrã do terminal mostrando a execução do playbook `install_nginx.yml`.
    *   Captura de ecrã do navegador mostrando a página web servida pelo Nginx no Managed Node, com o conteúdo personalizado.
    *   Uma breve reflexão sobre como o Ansible simplifica a gestão de configuração e a implantação de serviços em múltiplos servidores.

## Critérios de Avaliação:
*   **Configuração do Ansible (40%):** O Ansible deve estar instalado e o inventário configurado corretamente.
*   **Execução do Playbook (40%):** O playbook deve ser executado com sucesso, instalando e configurando o Nginx no Managed Node.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

