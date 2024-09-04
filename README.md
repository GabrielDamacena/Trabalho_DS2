# XChat

# Sistema de Comunicação com Chatbot

## Descrição e Objetivo do Projeto

### Descrição
Este projeto é um sistema de comunicação que inclui uma plataforma web e um aplicativo móvel, permitindo a interação em tempo real entre múltiplos usuários em uma única linha de conversa. O sistema também conta com um chatbot que pode enviar mensagens automáticas em horários programados e emitir alertas. O objetivo é melhorar a comunicação de grupo e a gestão de mensagens por meio de automação e programação.

### Objetivo
- Facilitar a comunicação simultânea entre múltiplos usuários em uma única linha de conversa.
- Fornecer um chatbot que possa enviar mensagens programadas e emitir alertas automáticos.
- Melhorar a eficiência das comunicações através da automação e da gestão de mensagens programadas.

## Tecnologias Utilizadas

- **Frontend Web:**
  - **Framework/Libraries:** React.js, Vue.js ou Angular
  - **CSS Framework:** Tailwind CSS ou Bootstrap
  - **Biblioteca para gerenciamento de estado:** Redux ou Vuex

- **Frontend Mobile:**
  - **Framework:** React Native ou Flutter

- **Backend:**
  - **Linguagem:** Node.js (JavaScript) ou Python
  - **Framework:** Express.js (para Node.js) ou Django (para Python)
  - **Banco de Dados:** PostgreSQL ou MongoDB
  - **Servidor:** Nginx ou Apache

- **Chatbot:**
  - **Plataforma:** Dialogflow, Microsoft Bot Framework ou uma solução personalizada com Node.js

- **Programação de Mensagens:**
  - **Biblioteca para agendamento:** node-schedule (para Node.js) ou Celery (para Python)

- **Documentação da API:**
  - **Ferramenta:** Postman

## Requisitos Funcionais

1. **Cadastro e Autenticação:**
   - Registro de usuários com e-mail e senha.
   - Login e logout.
   - Recuperação e redefinição de senha.
   - Verificação de e-mail.

2. **Gerenciamento de Usuários:**
   - Adicionar e remover usuários na linha de conversa.
   - Definir permissões e papéis (administrador, membro).

3. **Comunicação em Linha:**
   - Envio e recebimento de mensagens em tempo real.
   - Exibição de mensagens para todos os participantes.

4. **Funcionalidade do Chatbot:**
   - Envio de mensagens automáticas em horários programados.
   - Emissão de alertas e notificações baseadas em eventos.

5. **Programação de Mensagens:**
   - Interface para criar, visualizar e gerenciar mensagens programadas.
   - Agendamento de mensagens para horários específicos.

6. **Notificações:**
   - Notificações de novas mensagens.
   - Notificações para mensagens programadas e alertas do chatbot.

7. **Histórico de Mensagens:**
   - Armazenamento e acesso ao histórico de mensagens.
   - Funcionalidade de busca e filtragem.

## Requisitos Não Funcionais

1. **Desempenho:**
   - Suporte para alta simultaneidade de usuários.
   - Entrega de mensagens em tempo real com latência mínima.

2. **Segurança:**
   - Criptografia de dados em trânsito e em repouso.
   - Proteção contra ataques comuns como injeção de SQL e CSRF.

3. **Usabilidade:**
   - Interface intuitiva e amigável.
   - Design responsivo para web e dispositivos móveis.

4. **Escalabilidade:**
   - Arquitetura escalável para suportar crescimento de usuários e mensagens.
   - Facilidade de adição de novas funcionalidades.

5. **Disponibilidade e Confiabilidade:**
   - Alta disponibilidade e plano de backup e recuperação de dados.

6. **Compatibilidade:**
   - Compatibilidade com principais navegadores e plataformas móveis.

## Regras de Negócio

1. **Limitações de Mensagens:**
   - Limite de caracteres por mensagem.
   - Mensagens longas podem ser divididas ou truncadas com aviso.

2. **Gerenciamento do Chatbot:**
   - Regras predefinidas para envio de mensagens e alertas.
   - Mensagens do chatbot identificadas claramente.

3. **Programação e Alertas:**
   - Definição clara de data e hora para envio de mensagens programadas.
   - Validação de horários e datas para evitar erros.

4. **Controle de Acesso:**
   - Controle sobre quem pode gerenciar o chatbot e mensagens programadas.
   - Adição e remoção de usuários controladas por permissões.

5. **Compliance e Privacidade:**
   - Conformidade com leis de proteção de dados (GDPR, LGPD).
   - Opções de consentimento e controle de informações pessoais.


## Fluxos das Principais Telas

1. **Tela de Login/Registro:**
   - Campos: E-mail, Senha
   - Ações: Login, Registro, Recuperar Senha

2. **Tela Principal (Linha de Conversa):**
   - Exibição de mensagens em tempo real.
   - Campo de entrada de mensagem.
   - Botão de envio.

3. **Tela de Gerenciamento de Mensagens Programadas:**
   - Listagem de mensagens programadas.
   - Interface para adicionar, editar ou remover mensagens programadas.

4. **Tela de Configurações do Chatbot:**
   - Definir regras e condições para o chatbot.
   - Configurar mensagens automáticas e alertas.

5. **Tela de Histórico de Mensagens:**
   - Visualização e pesquisa no histórico de mensagens.

## Documentação da API com Postman

1. **Endpoints Básicos:**
   - **POST /api/users/register:** Registro de novos usuários.
   - **POST /api/users/login:** Autenticação de usuários.
   - **GET /api/conversations/:id:** Obter detalhes da linha de conversa.
   - **POST /api/conversations/:id/messages:** Enviar mensagem.
   - **GET /api/conversations/:id/messages:** Obter mensagens da linha de conversa.
   - **POST /api/scheduled-messages:** Agendar nova mensagem.
   - **GET /api/scheduled-messages:** Listar mensagens programadas.

