# Tarefas Microsoft Teams - Semana 14: Configuração do Sistema - Rede (Parte 2)

## Título da Tarefa: Implementando Firewall e Partilha de Ficheiros

## Descrição:
Nesta semana, vamos focar na segurança de rede através da configuração de firewall e na partilha de ficheiros entre sistemas. A tarefa prática permitirá aos alunos implementar regras básicas de firewall e configurar um serviço de partilha de ficheiros.

## Objetivos:
*   Implementar regras básicas de firewall usando `ufw`.
*   Configurar um serviço de partilha de ficheiros (NFS ou Samba).
*   Testar a segurança e a acessibilidade dos serviços configurados.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre firewall e partilha de ficheiros).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Desktop ou Server), execute os seguintes passos:
    *   **Configuração de Firewall com `ufw`:**
        *   Verifique o estado atual do `ufw`: `sudo ufw status`.
        *   Ative o `ufw` (se não estiver ativo): `sudo ufw enable`.
        *   Defina a política padrão para negar todas as conexões de entrada e permitir todas as de saída: `sudo ufw default deny incoming` e `sudo ufw default allow outgoing`.
        *   Permita o tráfego SSH (porta 22): `sudo ufw allow ssh`.
        *   Permita o tráfego HTTP (porta 80): `sudo ufw allow http`.
        *   Verifique novamente o estado do `ufw`: `sudo ufw status numbered`.
    *   **Configuração de Partilha de Ficheiros (Escolha uma opção):**
        *   **Opção A: NFS (Network File System) - Para partilha entre sistemas Linux/Unix**
            *   Instale o servidor NFS: `sudo apt install nfs-kernel-server`.
            *   Crie um diretório para partilhar: `sudo mkdir /srv/nfs/share`.
            *   Altere as permissões: `sudo chown nobody:nogroup /srv/nfs/share` e `sudo chmod 777 /srv/nfs/share`.
            *   Edite o ficheiro `/etc/exports` e adicione a linha: `/srv/nfs/share *(rw,sync,no_subtree_check)`.
            *   Exporte as partilhas: `sudo exportfs -a`.
            *   Reinicie o serviço NFS: `sudo systemctl restart nfs-kernel-server`.
            *   **Numa segunda VM (cliente Linux):** Instale o cliente NFS: `sudo apt install nfs-common`. Crie um ponto de montagem: `sudo mkdir /mnt/nfs`. Monte a partilha: `sudo mount <IP_do_servidor>:/srv/nfs/share /mnt/nfs`.
        *   **Opção B: Samba - Para partilha entre sistemas Linux e Windows**
            *   Instale o Samba: `sudo apt install samba`.
            *   Crie um diretório para partilhar: `sudo mkdir /srv/samba/share`.
            *   Altere as permissões: `sudo chmod 777 /srv/samba/share`.
            *   Edite o ficheiro `/etc/samba/smb.conf` e adicione a seguinte secção no final:
                ```
                [share]
                   comment = Shared Folder
                   path = /srv/samba/share
                   browsable = yes
                   writable = yes
                   guest ok = yes
                   read only = no
                ```
            *   Crie um utilizador Samba (com a mesma senha do utilizador do sistema): `sudo smbpasswd -a <seu_utilizador>`.
            *   Reinicie o serviço Samba: `sudo systemctl restart smbd nmbd`.
            *   **Numa segunda VM (cliente Linux ou Windows):** Tente aceder à partilha (ex: `smbclient -L <IP_do_servidor>` no Linux, ou `\\<IP_do_servidor>\share` no Windows Explorer).
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando o estado do `ufw` com as regras configuradas.
    *   Captura de ecrã do ficheiro de configuração do NFS (`/etc/exports`) ou Samba (`/etc/samba/smb.conf`) editado.
    *   Captura de ecrã do terminal (no cliente) mostrando o acesso bem-sucedido à partilha de ficheiros (NFS ou Samba).
    *   Uma breve reflexão sobre a importância da firewall e da partilha de ficheiros em ambientes de rede.

## Critérios de Avaliação:
*   **Configuração de Firewall (40%):** O `ufw` deve estar ativo e com as regras SSH e HTTP configuradas corretamente.
*   **Configuração de Partilha de Ficheiros (40%):** O serviço de partilha (NFS ou Samba) deve estar configurado e acessível a partir de um cliente.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

