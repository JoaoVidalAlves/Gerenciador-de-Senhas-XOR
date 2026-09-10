# Gerenciador de Senhas em C

Gerenciador de senhas desenvolvido em **C** para armazenar e gerenciar credenciais de diferentes serviços.

O sistema utiliza **criptografia baseada em XOR** para proteger as senhas antes de armazená-las em arquivos, evitando que sejam mantidas diretamente em texto legível.

## Funcionalidades

- Cadastro de credenciais
- Armazenamento de serviço, usuário e senha
- Criptografia das senhas utilizando XOR
- Armazenamento das credenciais criptografadas em arquivo
- Descriptografia das senhas durante a consulta
- Proteção por senha mestre
- Consulta das credenciais cadastradas
- Persistência dos dados entre execuções
- Interface via terminal

## Tecnologias e conceitos

- **C**
- `struct`
- Ponteiros
- Manipulação de arquivos
- Operações bit a bit
- XOR
- Persistência de dados
- Validação de entrada

## Armazenamento e criptografia

Antes de serem armazenadas, as senhas passam por um processo de criptografia utilizando a operação **XOR**.

De forma simplificada:

```text
Senha original
      ↓
  XOR + chave
      ↓
Senha criptografada
      ↓
   Arquivo
