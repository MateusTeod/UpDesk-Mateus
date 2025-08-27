<p align="center">
  | <a href="#sobre-o-projeto">Sobre o Projeto</a> |
  <a href="#backlog-do-produto">Backlog do Produto</a> |
  <a href="#cronograma-de-desenvolvimento">Cronograma de desenvolvimento |
  <a href="#cronograma-de-evolucao">Cronograma de Evolução</a> |
  <a href="#sprints">Sprints</a> |
  <a href="#tecnologias-utilizadas">Tecnologias</a> |
  <a href="#estrutura-de-pastas">Estrutura de Pastas</a> |  
  <br>  | <a href="#como-rodar-o-projeto">Como Rodar o Projeto</a> |  
 <a href="#documentacao">Documentação</a> |  
  <a href="#equipe">Equipe</a> |
</p>

# 🤖UpDesk-PIM-4
## 📜Sobre o Projeto <a id="sobre-o-projeto"></a>
O **UpDesk** tem como objetivo resolver uma dor comum de empresas e setores de TI: a dificuldade na triagem, priorização e acompanhamento de chamados de suporte.
Muitas vezes, usuários enfrentam demora no atendimento devido à falta de organização, categorização incorreta ou sobrecarga de analistas.
O UpDesk propõe uma solução inovadora com inteligência artificial integrada, permitindo a sugestão automática de soluções, categorização de chamados e direcionamento para o nível adequado de suporte.

---

## BACKLOG DE PRODUTO <a id="backlog-do-produto"></a>
- **Backlog do Produto**:  [Backlog do UpDesk](https://github.com/mancijo/UpDesk/blob/main/Analysis%20Planning/BacklogUpDesk.md)

---

## Cronograma de Desenvolvimento - Software de Gestão de Chamados <a id="cronogrma-de-desenvolvimento"></a>
- **Cronograma de sprint**: [Sprint Planning](https://github.com/mancijo/UpDesk/blob/main/Dev%20planning/sprintPlanning.md)
- **Etapa 1** → Levantamento de requisitos e modelagem inicial  
- **Etapa 2** → Protótipos em baixa, média e alta fidelidade (Figma)  
- **Etapa 3** → Implementação da interface web e modelagem do banco

- # 📅 Cronograma de Evolução <a id="cronograma-de-evolucao"></a>

| Fase / Sprint | Período        | Atividades Principais                                                                    |
| ------------- | -------------- | ---------------------------------------------------------------------------------------- |
| Planejamento  | 26/08 – 02/09  | Definição do backlog, levantamento de requisitos, configuração inicial do repositório    |
| Sprint 1      | 03/09 – 09/09  | Desenvolvimento do caso de uso                                                           |
| Sprint 2      | 10/09 – 16/09  | Desenvolvimento diagrama de classe                                                       |
| Sprint 3      | 17/09 – 23/09  | Desenvolvimento diagrama de sequência                                                    |
| Sprint 4      | 24/09 – 30/09  | Desenvolvimento diagrama de implantacão                                                  |
  
- ---

## 📊 Tabela de Sprints <a id="sprints"></a>

| Período da Sprint | Documentação | 
|-------------------|--------------|
| Sprint 1 | Planejamento inicial | 
| Sprint 2 | Backlog de Sprint | 
| Sprint 3 | Requisitos & Casos de Uso | 

---

## 🛠 Tecnologias Utilizadas <a id="tecnologias-utilizadas"></a>
- **Backend**: Python+Flask
- **Banco de Dados**: MS SQL Server  
- **Frontend**: HTML, CSS, JavaScript, Bootstrap  
- **Protótipos**: [Figma](https://www.figma.com/design/zsCyy2iAYMPcS7DAUR5rye/Sem-t%C3%ADtulo?node-id=1-1784&m=dev)  
- **Versionamento**: Git/GitHub  
- **Metodologia**: Scrum  

---

## 📂 Estrutura do Projeto <a id="estrutura-de-pastas"></a>
   
📁 app/                   # Pasta principal da aplicação  
 ┣ 📁 templates/          # Arquivos HTML (renderizados pelo Flask)  
 ┣ 📁 static/             # Arquivos estáticos (CSS, JS, imagens)  
 ┣ 📁 models/             # Classes e entidades do sistema (POO)  
 ┣ 📁 routes/             # Definição das rotas/endpoints do Flask  
 ┗ 📁 utils/              # Funções auxiliares (integração IA, helpers, etc.)  
   
📁 database/              # Configurações e scripts do banco de dados  
 ┗ 📄 schema.sql          # Estrutura inicial do banco de dados (DDL)  
  
📄 app.py                 # Arquivo principal da aplicação (ponto de entrada)  
📄 requirements.txt       # Lista de dependências Python do projeto 

---

## ▶️ Como Executar, Usar e Testar o Projeto <a id="como-rodar-o-projeto"></a>
1. Clone este repositório:  
   ```bash
   git clone https://github.com/mancijo/UpDesk.git
   ```
2. Configure o banco de dados no MS SQL Server utilizando os scripts em `/db`.
3. Abra o projeto no Visual Studio e restaure as dependências.
4. Execute a aplicação localmente.
5. Para testes, utilize os casos definidos em `/tests`.

---

## 📑 Documentação <a id="documentacao"></a>
Este documento reúne:

- Modelagem do banco de dados
- Diagramas de casos de uso e sequência
- Planejamentos de sprint
- Roteiros de teste
- Políticas de LGPD

---

## ✅ DoR (Definition of Ready)
Critérios que devem estar prontos antes que uma história entre em desenvolvimento:

- História descrita claramente.
- Critérios de aceitação definidos.
- Protótipo ou diagrama associado (quando necessário).
- Dependências mapeadas.
- Estimativa realizada pela equipe.

---

## ✅ DoD (Definition of Done)
Critérios para considerar uma história finalizada:

- Código desenvolvido, revisado e integrado.
- Testes unitários executados e aprovados.
- Critérios de aceitação atendidos.
- Documentação atualizada.
- Deploy interno validado.

---

## 📘 Manual do Usuário
### 🔐 Acesso
O usuário deve realizar login com e-mail e senha cadastrados.  
A autenticação garante o acesso às funcionalidades de acordo com a hierarquia.

### 📝 Abertura de Chamado
1. Clique em **Abrir Chamado**.  
2. Preencha os campos: título, descrição e categoria.  
3. A IA poderá sugerir soluções antes do envio.  
   - Caso o usuário aceite → o chamado é encerrado automaticamente.  
   - Caso recuse → o chamado segue para triagem.  

### 👥 Perfis de Usuário
- **Supervisor** → Gerencia usuários, acessos e relatórios.  
- **TI Nível 1** → Atende chamados de baixa/média complexidade.  
- **TI Nível 2** → Atende chamados de média/alta complexidade.  
- **Triagem** → Classifica chamados e valida ações da IA.  
- **Usuário Padrão** → Abre chamados.  
- **Inteligência Artificial** → Sugere soluções e categoriza chamados.

---

- ## 👥 Equipe do Projeto <a id="equipe"></a>
- **Product Owner (PO):** Jonatas Santos  
- **Scrum Master:** Andrei Mancijo  
- **Dev Team:**  
  - Mariozan Damasceno Lacerda Júnior  
  - Mateus Teodoro  
  - Kaique Batista da Silva  
  - Filipe Vitor dos Santos  

---

[Github](https://github.com/MateusTeod/)
[Linkedin](https://www.linkedin.com/in/mateus-teod)

