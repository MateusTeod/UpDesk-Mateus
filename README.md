# UpDesk-PIM-4
About Um projeto acadêmico onde será desenvolvido um sistema de abertura de chamado com inteligência artificial.
## BACKLOG DE PRODUTO
## Abertura de Chamado
- **Login**  
  - Nome completo  
  - E-mail  
  - ID  
  - Telefone  
- **Título do chamado**  
- **Descrição** (inserida pelo usuário)  
- **Anexo**  
- **Prioridade**  
- **Tempo de espera**  
- **Incidência**  
- **Finalizar chamado**  

---

## Gerenciamento de Chamado
- **Times de suporte**  
- **Categorização de chamados**  
- **Histórico de chamados**  
  - Ticket  
  - Nome do solicitante  
  - Status  
  - Categorização  
  - Data  
  - Backlog (conversas e informações)  
  - Descrição geral  
- **Chamados pendentes**  
- **Solicitação de urgência**  
- **Iniciar chamado**  
  - Exibir dados  
- **Validação de chamados pela IA** (triagem)  

---

## Gerenciamento de Usuários (Supervisor)
- **Usuários e funções**  
  - Supervisor  
  - Focal Point  
  - TI (níveis n1, n2, n3)  
  - Triagem  
  - Usuário
- **Encerramento de chamado**  

---

## Inteligência Artificial
- **Início do atendimento**  
- **Abrir chamado**  
- **Sugerir soluções**  
- **Direcionamento automatizado de chamado**  
- **Encerramento de chamado**  

---

# Use Cases - Requisitos

## Usuário
- Autenticar usuário  
- Abrir chamado  
- Monitorar chamados  
- Avaliar solução aplicada  

## Inteligência Artificial (IA)
- Analisar chamado  
- Sugerir soluções  
- Transferir atendimento para níveis apropriados  
- Aprender com feedback  

## Nível 1 (N1)
- Receber chamados de baixa e média complexidade  
- Resolver chamados de baixa e média complexidade  
- Transferir chamados para N2  
- Consultar histórico de chamados  

## Nível 2 (N2)
- Receber chamados escalados  
- Resolver chamados complexos (N2)  
- Consultar histórico de chamados  

## Supervisor
- **Gerenciar usuários**
  - Cadastrar usuários
  - Editar informações de usuários
  - Inativar usuários
- **Visualizar relatórios de usuários em chamados**

# Não funcionais 
- **Banco de dados**
  - Conceitual
  - Lógico
  - Físico
- **Protótipo Figma**
  - Baixa fidelidade
  - Média fidelidade
  - Alta fidelidade
- **Diagramas e casos de uso**
  - Casos de uso descritivo
  - Diagrama de casos de uso
  - Diagrama de sequência
  - Diagrama de implementação
  - Diagrama de classes
- **Testes**
  - Planilha de testes
- **Documentação PIM**
  - Resumo
  - Introdução
  - Análise de Sistemas Orientada a Objetos
  - Engenharia de Software 2
  - POO 1
  - Projeto de Interface com o Usuário
  - Banco de Dados
  - Economia de Mercado
  - Gestão estratégica de Recursos Humanos
## CRONOGRAMA DE EVOLUÇÃO
# Cronograma de Desenvolvimento - Software de Gestão de Chamados

Este documento detalha o cronograma do projeto, dividindo as tarefas por semana e por time (Desenvolvimento Web e ServerSide).

---

## **19/08/2025**

### **Desenvolvimento Web (Front-End)**
- **Kaique**: Implementação da tela de login.
- **Mariozan**: Implementação da tela inicial para o supervisor.
- **Filipe**: Desenvolvimento do card de perfil.
- **Andrei**: Desenvolvimento do card para chamados enviados.

### **ServerSide (Back-End)**
- **Jonatas**: Desenvolvimento do CRUD (Create, Read, Update, Delete) para o chat, utilizando MySQL.
- **Matheus**: Desenvolvimento do CRUD para perfis, utilizando MySQL.

---

## **26/08/2025**

### **Desenvolvimento Web (Front-End)**
- Desenvolvimento do card para editar perfis.
- Desenvolvimento do card de confirmação para excluir usuário.
- Desenvolvimento do card de confirmação de identidade.
- Implementação da tela de gerenciamento de usuários.
- Desenvolvimento do formulário de abertura de chamado.
- Implementação da tela de solução sugerida pela IA (Up Desk).
- Implementação da tela de chamado resolvido (Up Desk).

### **ServerSide (Back-End)**
- Definição da estrutura JSON da API.
- Desenvolvimento do servidor de requisições.
- Implementação da validação de login.

---

## **02/09/2025**

### **Desenvolvimento Web (Front-End)**
- Desenvolvimento do painel de triagem.
- Desenvolvimento do card de dados do chamado.
- Desenvolvimento do card de dados do chamado na triagem.
- Desenvolvimento do card para aprovar ações da IA.
- Desenvolvimento do card de prioridade do chamado.
- Desenvolvimento do card de confirmação de transferência de chamado.
- Desenvolvimento do card de feedback de transferência de chamado.
- Implementação do painel de visualização de chamados.
- Desenvolvimento do card de informações dos chamados.

