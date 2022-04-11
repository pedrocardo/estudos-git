# Sobre Git

Git é um sistema de controle de versão distribuído. Com ele, é possível rastrear e coordenar modificações em arquivos.

O Git funciona com repositórios - diretórios com arquivos rastreados e pastas chamadas _.git_.

## Estados de arquivos

Arquivos podem estar, em relação ao último _commit_ do repositório, em um dos seguintes estados:

- no estado _untracked_, o arquivo não foi rastreado;
- no estado _modified_, o arquivo possui modificações;
- no estado _deleted_, o arquivo foi deletado;
- no estado _staged_, o arquivo está pronto para ser salvo em uma nova versão;
- no estado _unmodified_, o arquivo não possui modificações.

## _Glob_ _patterns_

_Glob_ _patterns_ são padrões de escrita que especificam conjuntos de arquivos, utilzando _wildcards_.

Esses padrões de escrita podem ser utilizados em comandos do Git e arquivos _.gitignore_.

Por exemplo, o _wildcard_ \* pode ser utilizado para combinar arquivos com nomes que comecem ou terminem com caracteres específicos.
