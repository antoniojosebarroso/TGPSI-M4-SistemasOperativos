# Tarefas Microsoft Teams - Semana 18: Múltiplas Configurações do Sistema - LVM

## Título da Tarefa: Gerenciamento Flexível de Discos com LVM

## Descrição:
Nesta semana, vamos explorar o Logical Volume Manager (LVM), uma ferramenta poderosa para gerenciar o armazenamento de forma flexível em Sistemas Operativos Open Source. A tarefa prática permitirá aos alunos criar e estender volumes lógicos.

## Objetivos:
*   Compreender os conceitos de LVM (Physical Volumes, Volume Groups, Logical Volumes).
*   Criar e gerenciar volumes lógicos.
*   Estender volumes lógicos sem interrupção do serviço.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre LVM).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Server), execute os seguintes passos:
    *   **Preparação da VM:** Adicione dois novos discos virtuais à sua VM (ex: 5GB cada). Não os formate nem crie partições neles ainda.
    *   **Criação de Physical Volumes (PVs):**
        *   Identifique os novos discos (ex: `/dev/sdb`, `/dev/sdc`) usando `lsblk`.
        *   Crie Physical Volumes em cada disco: `sudo pvcreate /dev/sdb` e `sudo pvcreate /dev/sdc`.
        *   Verifique os PVs: `sudo pvdisplay`.
    *   **Criação de Volume Group (VG):**
        *   Crie um Volume Group chamado `dados_vg` que inclua os dois PVs: `sudo vgcreate dados_vg /dev/sdb /dev/sdc`.
        *   Verifique o VG: `sudo vgdisplay`.
    *   **Criação de Logical Volume (LV):**
        *   Crie um Logical Volume chamado `lv_web` de 5GB dentro do `dados_vg`: `sudo lvcreate -n lv_web -L 5G dados_vg`.
        *   Formate o LV com um sistema de ficheiros (ex: ext4): `sudo mkfs.ext4 /dev/dados_vg/lv_web`.
        *   Crie um ponto de montagem: `sudo mkdir /mnt/web`.
        *   Monte o LV: `sudo mount /dev/dados_vg/lv_web /mnt/web`.
        *   Adicione uma entrada em `/etc/fstab` para montagem automática no arranque.
        *   Verifique o LV: `sudo lvdisplay` e `df -h`.
    *   **Extensão de Logical Volume:**
        *   Estenda o `lv_web` em 2GB: `sudo lvextend -L +2G /dev/dados_vg/lv_web`.
        *   Redimensione o sistema de ficheiros para usar o novo espaço (para ext4): `sudo resize2fs /dev/dados_vg/lv_web`.
        *   Verifique o novo tamanho: `df -h`.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a criação dos PVs, VG e LV.
    *   Captura de ecrã do terminal mostrando o LV montado e o seu tamanho inicial (`df -h`).
    *   Captura de ecrã do terminal mostrando a extensão do LV e o seu novo tamanho (`df -h`).
    *   Uma breve reflexão sobre as vantagens do LVM para a gestão de armazenamento em servidores.

## Critérios de Avaliação:
*   **Implementação de LVM (60%):** Criação e extensão correta de PVs, VGs e LVs.
*   **Relatório (20%):** Clareza das capturas de ecrã e da descrição das configurações e da reflexão.
*   **Participação no Fórum (10%):** Qualidade da contribuição e da interação.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

