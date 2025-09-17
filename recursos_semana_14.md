# Recursos - Semana 14: Configuração do Sistema - Rede (Parte 2)

## Tópicos Abordados
*   Configuração de firewall (ufw, iptables básico).
*   Partilha de ficheiros (NFS/Samba).

## Objetivos de Aprendizagem
*   Implementar regras básicas de firewall.
*   Configurar partilha de ficheiros.

## Material de Apoio

### Apresentação: Segurança e Partilha de Rede

#### Slide 1: Título
*   **Título:** Configuração do Sistema - Rede (Parte 2)
*   **Subtítulo:** Firewall e Partilha de Ficheiros

#### Slide 2: Introdução à Firewall
*   **Conteúdo:** O que é uma firewall e a sua importância na segurança de rede. Tipos de firewall (baseada em host, baseada em rede).

#### Slide 3: `ufw` (Uncomplicated Firewall)
*   **Conteúdo:** Uma interface mais simples para gerir `iptables`. Comandos básicos (`ufw enable`, `ufw disable`, `ufw status`, `ufw allow`, `ufw deny`). Exemplos de regras.

#### Slide 4: `iptables` (Conceitos Básicos)
*   **Conteúdo:** Como `iptables` funciona (tabelas, cadeias, regras). Comandos básicos para listar regras (`iptables -L`). A complexidade do `iptables` e a razão para usar `ufw`.

#### Slide 5: Partilha de Ficheiros com NFS (Network File System)
*   **Conteúdo:** O que é NFS. Quando usar NFS (partilha entre sistemas Linux/Unix). Instalação e configuração básica (servidor e cliente).

#### Slide 6: Configuração do Servidor NFS
*   **Conteúdo:** Edição do ficheiro `/etc/exports`. Opções de exportação (rw, sync, no_subtree_check). Reiniciar o serviço NFS.

#### Slide 7: Configuração do Cliente NFS
*   **Conteúdo:** Montagem de partilhas NFS (`mount -t nfs`). Montagem automática no arranque (`/etc/fstab`).

#### Slide 8: Partilha de Ficheiros com Samba
*   **Conteúdo:** O que é Samba. Quando usar Samba (partilha entre sistemas Linux e Windows). Instalação e configuração básica.

#### Slide 9: Configuração do Samba
*   **Conteúdo:** Edição do ficheiro `/etc/samba/smb.conf`. Criação de utilizadores Samba (`smbpasswd`). Reiniciar o serviço Samba.

#### Slide 10: Conclusão
*   **Conteúdo:** A configuração de firewall e a partilha de ficheiros são serviços de rede essenciais para a segurança e colaboração em ambientes Open Source.

### Artigo Introdutório: Guia para Configuração de Firewall e Partilha de Ficheiros no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, configurar o `ufw` para permitir apenas o tráfego SSH e HTTP. Configurar uma partilha NFS ou Samba e aceder a ela a partir de outra VM ou do sistema anfitrião. (a ser detalhado na tarefa do Teams).

