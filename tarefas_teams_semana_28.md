# Tarefas Microsoft Teams - Semana 28: Segurança em Sistemas Open Source (Avançado)

## Título da Tarefa: Implementando Criptografia de Disco e Autenticação PAM

## Descrição:
Nesta semana, vamos aprofundar as medidas de segurança em Sistemas Operativos Open Source, focando na criptografia de disco com LUKS e na configuração avançada de autenticação com PAM. A tarefa prática permitirá aos alunos implementar estas funcionalidades para proteger dados sensíveis e reforçar as políticas de acesso.

## Objetivos:
*   Implementar criptografia de disco para proteger dados em repouso.
*   Configurar módulos PAM para reforçar políticas de autenticação.
*   Compreender a importância da segurança em profundidade.

## Atividades a Desenvolver:
1.  **Leitura e Compreensão:** Revise o material de apoio fornecido (apresentação e artigo introdutório sobre criptografia de disco e autenticação PAM).
2.  **Exercícios Práticos em VM:** Numa máquina virtual com um SO Open Source (ex: Ubuntu Server), execute os seguintes passos:
    *   **Criptografia de Disco com LUKS:**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Adicione um novo disco virtual à sua VM (ex: 5GB). Não o formate nem crie partições nele ainda.
        *   Crie uma partição criptografada com LUKS no novo disco (ex: `/dev/sdb`):
            *   `sudo cryptsetup luksFormat /dev/sdb` (confirme com YES e defina uma senha forte).
            *   `sudo cryptsetup luksOpen /dev/sdb meu_volume_seguro` (insira a senha).
            *   Formate o volume lógico aberto: `sudo mkfs.ext4 /dev/mapper/meu_volume_seguro`.
            *   Crie um ponto de montagem: `sudo mkdir /mnt/seguro`.
            *   Monte o volume: `sudo mount /dev/mapper/meu_volume_seguro /mnt/seguro`.
            *   Verifique o volume montado: `df -h`.
            *   Desmonte e feche o volume: `sudo umount /mnt/seguro` e `sudo cryptsetup luksClose meu_volume_seguro`.
    *   **Configuração de PAM para Política de Senha:**
        *   Faça um snapshot da sua VM antes de continuar.
        *   Edite o ficheiro `/etc/pam.d/common-password`.
        *   Adicione ou modifique a linha `password requisite pam_pwquality.so retry=3 minlen=12 difok=3 reject_username enforce_for_root` para exigir senhas mais fortes (mínimo 12 caracteres, 3 diferentes do anterior, etc.).
        *   Teste a nova política de senha tentando alterar a senha de um utilizador com uma senha fraca (`passwd <seu_utilizador>`). Deverá ser rejeitada.
3.  **Capturas de Ecrã e Relatório:** Crie um documento (PDF ou Word) com as seguintes capturas de ecrã e informações:
    *   Captura de ecrã do terminal mostrando a criação e montagem do volume LUKS.
    *   Captura de ecrã do terminal mostrando a tentativa falhada de alterar a senha com a nova política PAM.
    *   Uma breve reflexão sobre como a criptografia de disco e as políticas de senha fortes contribuem para a segurança de um sistema.

## Critérios de Avaliação:
*   **Criptografia de Disco (40%):** O volume LUKS deve ser criado, montado e desmontado corretamente.
*   **Configuração PAM (40%):** A política de senha deve ser configurada e testada com sucesso.
*   **Relatório (10%):** Clareza das capturas de ecrã e da descrição das operações e da reflexão.
*   **Pontualidade (10%):** Entrega da tarefa dentro do prazo estabelecido.

## Prazo de Entrega:
[Definir data e hora limite para a entrega do relatório e participação no fórum]

