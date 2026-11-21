# CHAT-REAL-TIME
Aplicação web de chat em tempo real com Node.js, WebSockets e persistência em JSON — atividade de Desenvolvimento Voltado à Web III (UNIGRAN EAD).
### Como funciona o código

# Sistema de Chat em Tempo Real com Node.js e WebSockets

Aplicação web de chat em tempo real desenvolvida em **Node.js** para a disciplina **Desenvolvimento Voltado à Web III** do curso de Tecnologia em Análise e Desenvolvimento de Sistemas (**UNIGRAN EAD**).

O sistema permite que múltiplos utilizadores se liguem e troquem mensagens instantaneamente por meio de **WebSockets** (`socket.io`), contando com um servidor HTTP (`express`) para servir a interface do utilizador, gestão de conexões em tempo real e persistência do histórico de mensagens num ficheiro **JSON**.

## Estrutura e Descrição do Código

- **`server.js`**: configura o servidor HTTP, entrega os ficheiros estáticos da pasta `public`, gere as ligações e desconexões via WebSocket, envia o histórico inicial aos clientes e guarda cada nova mensagem no ficheiro `mensagens.json`.
- **`public/index.html`**: interface web onde o utilizador introduz o seu nome, envia mensagens em tempo real e visualiza o histórico carregado e atualizado instantaneamente.
- **`mensagens.json`**: ficheiro JSON utilizado para persistir as mensagens trocadas no chat[cite: 1].
- **`package.json`**: define os metadados do projeto, o script de inicialização (`npm start`) e as dependências necessárias (`express` e `socket.io`)[cite: 1].

## Pré-requisitos

- [Node.js](https://nodejs.org/) instalado no computador[cite: 1].

## Como instalar as dependências

Abre o terminal na pasta raiz do projeto e executa[cite: 1]:

```bash
npm install
npm start
http://localhost:3000
