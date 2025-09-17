# Recursos - Semana 28: Segurança em Sistemas Open Source (Avançado)

## Tópicos Abordados
*   Criptografia de disco (LUKS).
*   Autenticação (PAM).

## Objetivos de Aprendizagem
*   Implementar criptografia de disco.
*   Configurar métodos de autenticação.

## Material de Apoio

### Apresentação: Segurança Avançada em SO Open Source

#### Slide 1: Título
*   **Título:** Segurança em Sistemas Open Source (Avançado)
*   **Subtítulo:** Criptografia de Disco e Autenticação PAM

#### Slide 2: Aprofundando a Segurança
*   **Conteúdo:** Revisão dos princípios básicos de segurança. A necessidade de medidas de segurança mais robustas para proteger dados sensíveis.

#### Slide 3: Criptografia de Disco - Porquê?
*   **Conteúdo:** Proteção de dados em caso de roubo ou perda do dispositivo. Conformidade com regulamentações de privacidade. Conceito de criptografia em repouso.

#### Slide 4: LUKS (Linux Unified Key Setup)
*   **Conteúdo:** O padrão para criptografia de disco em Linux. Como funciona (cabeçalho LUKS, chaves, volume criptografado). Vantagens.

#### Slide 5: Implementação de LUKS
*   **Conteúdo:** Criação de uma partição criptografada (`cryptsetup luksFormat`). Abertura e fecho do volume (`cryptsetup luksOpen`, `cryptsetup luksClose`). Montagem do sistema de ficheiros.

#### Slide 6: Autenticação no Linux
*   **Conteúdo:** Como o Linux lida com a autenticação de utilizadores. O papel dos módulos de autenticação.

#### Slide 7: PAM (Pluggable Authentication Modules)
*   **Conteúdo:** O que é PAM. Sua arquitetura modular e flexível. Como permite configurar diferentes métodos de autenticação (senhas, biometria, smart cards).

#### Slide 8: Configuração de PAM
*   **Conteúdo:** Ficheiros de configuração em `/etc/pam.d/`. Exemplos de módulos PAM (`pam_unix.so`, `pam_cracklib.so`, `pam_faillock.so`).

#### Slide 9: Exemplos de Uso de PAM
*   **Conteúdo:** Reforçar políticas de senha (complexidade, histórico). Bloquear contas após múltiplas tentativas falhadas. Autenticação de dois fatores.

#### Slide 10: Conclusão
*   **Conteúdo:** A criptografia de disco com LUKS e a configuração avançada de autenticação com PAM são ferramentas poderosas para fortalecer a segurança de sistemas Open Source.

### Artigo Introdutório: Guia de Criptografia de Disco e Autenticação PAM no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, criar uma partição criptografada com LUKS e montá-la. Configurar uma política de senha mais forte usando PAM (ex: exigir senhas mais longas ou complexas). (a ser detalhado na tarefa do Teams).

