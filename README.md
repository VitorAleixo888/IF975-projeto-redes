# Projeto de Redes de Computadores: Sistema de Chat com UDP

Este projeto implementa um sistema de chat simples usando o protocolo UDP. O sistema consiste em um cliente e um servidor que permitem a comunicação de mensagens entre diferentes usuários.

## Ferramentas Utilizadas

- Python 3
- Biblioteca padrão `socket` para comunicação de rede
- Biblioteca padrão `threading` para threads

## Funcionalidade

### Cliente

- **Recebimento de Mensagens**: As mensagens são recebidas e salvas em um arquivo temporário. Após receber a mensagem completa, ela é lida e exibida no terminal.
- **Identificação do Usuário**: O cliente solicita o nome do usuário na inicialização, que é usado para identificar as mensagens enviadas e recebidas.

### Servidor

- **Gerenciamento do Cliente**: Mantém uma lista de clientes conectados e seus endereços.
- **Comando de Conexão**: O servidor reconhece comandos específicos para conectar: `hi, meu nome eh <NOME_DE_USUARIO>`
- **Comando de Desconexão**: O servidor reconhece o comando específico para desconectar: `bye`

## Como Usar

1. **Inicie o Servidor**:
    
    python servidor.py
    

2. **Inicie o Cliente**:
    
    python cliente.py
    
    Insira o nome de usuário quando solicitado.

3. Digite as mensagens no cliente. As mensagens serão enviadas ao servidor e em seguida distribuídas a todos os clientes conectados.

4. Para se desconectar, digite `bye`.
