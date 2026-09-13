# Relatório de Validação e Testes (/docs/testes.md)

## 🧪 Evidências dos Testes Realizados

### Teste 1: Autenticação e Perfis (Aluno vs. Professor)
* **Objetivo:** Verificar se a interface se adapta de acordo com o perfil selecionado na tela de login.
* **Ação:** Realizado login alternando os botões "Aluno" e "Professor".
* **Resultado:** O sistema altera corretamente os campos do formulário (Matrícula/SIAPE), as abas disponíveis no menu e o selo de identificação do usuário. Teste aprovado.

### Teste 2: Atualização de Status do Professor em Tempo Real
* **Objetivo:** Garantir que o professor consiga publicar sua presença e que isso reflita dinamicamente no painel.
* **Ação:** Acessado o "Painel de Edição" do professor, selecionado o status "Em Sala de Aula" com a observação "Sala 04" e enviado o formulário.
* **Resultado:** A tabela principal de status foi atualizada na hora, alterando a tag do professor para o estado e cor correspondentes. Dados mantidos via `localStorage`. Teste aprovado.

### Teste 3: Edição Dinâmica da Grade Horária
* **Objetivo:** Permitir ao professor ajustar as disciplinas da tabela semanal.
* **Ação:** Selecionado o dia (Quinta), horário (14:00) e inserida a disciplina "Projeto Integrador III".
* **Resultado:** A célula da tabela correspondente na aba "Grade Horária" atualizou o texto instantaneamente. Teste aprovado.

### Teste 4: Busca e Filtragem de Professores
* **Objetivo:** Facilitar a localização de informações pelos alunos.
* **Ação:** Digitação no campo de pesquisa da aba principal.
* **Resultado:** A lista de professores foi filtrada dinamicamente conforme o texto digitado. Teste aprovado.

---

## 💬 Feedback da Validação com Usuários
* **Interface Simples:** Os usuários destacaram a facilidade de navegação entre as abas e a clareza das tabelas divididas por turno (Manhã e Tarde).
* **Agilidade:** O acompanhamento em tempo real evita deslocamentos desnecessários ao campus para checar a presença física dos professores.
