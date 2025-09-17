# Recursos - Semana 18: Múltiplas Configurações do Sistema - LVM

## Tópicos Abordados
*   Introdução ao Logical Volume Manager (LVM).
*   Criação de volumes lógicos.

## Objetivos de Aprendizagem
*   Utilizar LVM para gestão flexível de armazenamento.
*   Criar e expandir volumes lógicos.

## Material de Apoio

### Apresentação: Gerenciamento de Volumes Lógicos com LVM

#### Slide 1: Título
*   **Título:** Múltiplas Configurações do Sistema - LVM
*   **Subtítulo:** Gerenciamento Flexível de Armazenamento no Linux

#### Slide 2: O que é LVM?
*   **Conteúdo:** Definição de Logical Volume Manager. Abstração da camada física de armazenamento. Vantagens (redimensionamento dinâmico, snapshots, flexibilidade).

#### Slide 3: Conceitos Chave do LVM
*   **Conteúdo:** Physical Volumes (PVs), Volume Groups (VGs), Logical Volumes (LVs). Explicação da hierarquia e como se relacionam.

#### Slide 4: Physical Volumes (PVs)
*   **Conteúdo:** Discos ou partições físicas inicializadas para uso com LVM. Comando `pvcreate`.

#### Slide 5: Volume Groups (VGs)
*   **Conteúdo:** Agrupamento de um ou mais PVs. Atua como um 


pool de armazenamento. Comandos `vgcreate`, `vgextend`, `vgreduce`.

#### Slide 6: Logical Volumes (LVs)
*   **Conteúdo:** Partições virtuais criadas a partir de um VG. Podem ser redimensionadas facilmente. Comandos `lvcreate`, `lvextend`, `lvreduce`.

#### Slide 7: Criando um Volume Lógico (Passo a Passo)
*   **Conteúdo:** Exemplo prático: `pvcreate`, `vgcreate`, `lvcreate`, `mkfs`, `mount`.

#### Slide 8: Redimensionamento de Volumes Lógicos
*   **Conteúdo:** Como expandir e encolher LVs. A importância de redimensionar o sistema de ficheiros após redimensionar o LV.

#### Slide 9: Snapshots com LVM
*   **Conteúdo:** O que são snapshots e como o LVM os suporta. Casos de uso (backup, testes).

#### Slide 10: Conclusão
*   **Conteúdo:** LVM oferece uma flexibilidade incomparável na gestão de armazenamento, sendo uma ferramenta poderosa para administradores de sistemas Linux.

### Artigo Introdutório: Guia Completo de LVM no Linux

(Conteúdo do artigo a ser desenvolvido)

## Atividades Sugeridas
*   Numa VM, criar um esquema de armazenamento usando LVM: criar PVs, VGs e LVs. Montar os LVs e testar o redimensionamento de um LV. (a ser detalhado na tarefa do Teams).

