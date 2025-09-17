# Recursos - Semana 16: Configuração do Sistema - Serviços Essenciais

## Tópicos Abordados
*   Configuração de serviços SSH.
*   Configuração de servidor web básico (Apache/Nginx).

## Objetivos de Aprendizagem
*   Configurar acesso remoto seguro.
*   Instalar e configurar um servidor web.

## Material de Apoio

### Apresentação: Serviços Essenciais em SO Open Source

#### Slide 1: Título
*   **Título:** Configuração do Sistema - Serviços Essenciais
*   **Subtítulo:** SSH e Servidores Web (Apache/Nginx)

#### Slide 2: Introdução aos Serviços de Rede
*   **Conteúdo:** O que são serviços de rede. A importância de configurar serviços essenciais para a funcionalidade do sistema.

#### Slide 3: SSH (Secure Shell) - Acesso Remoto Seguro
*   **Conteúdo:** O que é SSH. Vantagens (segurança, criptografia). Como funciona (cliente-servidor). Porta padrão (22).

#### Slide 4: Instalação e Configuração Básica do Servidor SSH
*   **Conteúdo:** Instalação do `openssh-server`. Ficheiro de configuração (`/etc/ssh/sshd_config`). Alterar porta, desativar login root, autenticação por chave.

#### Slide 5: Acesso SSH por Chaves
*   **Conteúdo:** Geração de pares de chaves (pública/privada). Copiar chave pública para o servidor (`ssh-copy-id`). Acesso sem senha.

#### Slide 6: Servidor Web Apache HTTP Server
*   **Conteúdo:** O que é Apache. Sua popularidade e flexibilidade. Instalação básica (`apache2`). Diretório padrão (`/var/www/html`).

#### Slide 7: Configuração Básica do Apache
*   **Conteúdo:** Ficheiros de configuração (`/etc/apache2/apache2.conf`, `sites-available`, `sites-enabled`). Ativar/desativar sites (`a2ensite`, `a2dissite`).

#### Slide 8: Servidor Web Nginx
*   **Conteúdo:** O que é Nginx. Sua eficiência e desempenho, especialmente como proxy reverso e para servir conteúdo estático. Instalação básica (`nginx`).

#### Slide 9: Configuração Básica do Nginx
*   **Conteúdo:** Ficheiros de configuração (`/etc/nginx/nginx.conf`, `sites-available`, `sites-enabled`). Estrutura de blocos de servidor.

#### Slide 10: Conclusão
*   **Conteúdo:** SSH e servidores web são serviços fundamentais para qualquer sistema Open Source conectado à rede. O domínio da sua configuração é crucial para administradores de sistemas.

### Artigo Introdutório: Guia para Configuração de SSH e Servidores Web no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, instalar e configurar o servidor SSH, permitindo acesso apenas por chave. Instalar e configurar um servidor web (Apache ou Nginx) e servir uma página HTML simples. (a ser detalhado na tarefa do Teams).

