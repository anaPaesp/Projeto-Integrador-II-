# Arquitetura e Modelagem do Projeto

## 1. Visão Geral

O projeto tem como objetivo facilitar o acesso dos alunos aos horários e ao status dos professores do Colégio Técnico de Bom Jesus.

A proposta é desenvolver um site ou uma aba integrada ao SIGAA, onde os professores possam disponibilizar seus horários de atendimento e atualizar sua situação na instituição. Dessa forma, os alunos poderão consultar essas informações de maneira rápida e simples.

---

## 2. Usuários do Sistema

O sistema terá dois tipos principais de usuários:

### Professor

O professor poderá:

* Informar seu status na escola;
* Atualizar sua presença;
* Cadastrar seus horários de atendimento;
* Editar seus horários de atendimento.

### Aluno

O aluno poderá:

* Consultar os horários dos professores;
* Consultar o status dos professores;
* Verificar se o professor está presente, em aula ou ausente;
* Acessar as informações sem necessidade de aprovação.

---

## 3. Funcionamento do Sistema

O funcionamento básico do sistema será dividido entre professores e alunos.

O professor acessará o sistema para atualizar sua situação na escola e seus horários de atendimento.

Os alunos poderão acessar o sistema para consultar essas informações.

### Fluxo principal

1. O usuário acessa o sistema.
2. O sistema identifica se o usuário é professor ou aluno.
3. O professor pode atualizar seu status e seus horários.
4. O aluno pode consultar os horários e o status dos professores.
5. As informações são exibidas de forma simples e rápida.

---

## 4. Fluxograma

```text
                    INÍCIO
                       |
                       v
                Acessar o sistema
                       |
                       v
              Identificar usuário
                  /          \
                 /            \
                v              v
           PROFESSOR          ALUNO
                |                |
                v                v
       Atualizar status     Consultar horários
                |                |
                v                v
       Editar horários      Ver status do professor
                |                |
                \                /
                 \              /
                  v            v
                 Informações atualizadas
                       |
                       v
                      FIM
```

---

## 5. Status dos Professores

O sistema deverá apresentar de maneira clara o status atual do professor.

Os principais status previstos são:

* **Presente na sala**
* **Em aula**
* **Ausente**

Essas informações permitirão que o aluno saiba rapidamente se é possível procurar determinado professor na instituição.

---

## 6. Horários dos Professores

Cada professor deverá possuir seus horários de atendimento e aulas cadastrados no sistema.

O professor poderá editar essas informações quando houver alguma alteração.

Os alunos poderão consultar os horários para saber quando procurar determinado professor para tirar dúvidas ou realizar uma "subida" de aula.

---

## 7. Modelo de Funcionamento das Informações

O sistema terá como principais informações:

```text
PROFESSOR
   |
   |---- Nome
   |
   |---- Status atual
   |
   |---- Horários de atendimento
   |
   └---- Horários de aula
```

Cada professor estará associado às suas próprias informações de horário e ao seu status atual.

---

## 8. Controle de Acesso

O sistema deverá possuir diferentes permissões de acordo com o usuário.

```text
PROFESSOR
   |
   |---- Pode atualizar status
   |
   └---- Pode editar horários


ALUNO
   |
   |---- Pode visualizar horários
   |
   └---- Pode visualizar status
```

A edição dos horários ficará restrita aos professores ou ao coordenador, conforme definido nos requisitos do projeto.

---

## 9. Interface do Sistema

A interface deverá ser simples e objetiva, permitindo que o aluno encontre as informações necessárias em poucos cliques.

Uma possível estrutura da tela inicial seria:

```text
+------------------------------------------+
|       HORÁRIOS DOS PROFESSORES           |
+------------------------------------------+
|                                          |
| Professor       Status        Horários  |
|                                          |
| Professor 1     Presente      Ver        |
| Professor 2     Em Aula       Ver        |
| Professor 3     Ausente       Ver        |
|                                          |
+------------------------------------------+
```

Ao selecionar um professor, o aluno poderá visualizar seus horários de atendimento e aulas.

---

## 10. Responsabilidades do Sistema

O sistema deverá:

* Exibir os horários dos professores;
* Exibir o status atual dos professores;
* Permitir que professores atualizem sua presença;
* Permitir que professores editem seus horários;
* Permitir que alunos consultem as informações;
* Manter as informações organizadas e de fácil acesso.

---

## 11. Requisitos Relacionados à Modelagem

A modelagem foi desenvolvida considerando os requisitos definidos na primeira etapa do projeto.

O sistema deverá ser adaptável para computadores e dispositivos móveis, possuir uma interface simples e permitir que os alunos consultem os horários e status dos professores sem necessidade de aprovação.

A edição das informações deverá ficar restrita aos professores ou ao coordenador.

---

## 12. Tecnologias

As tecnologias definitivas ainda serão definidas durante a etapa de desenvolvimento do projeto.

A solução poderá ser desenvolvida como um site próprio ou futuramente integrada ao SIGAA, conforme a viabilidade técnica.

---

## 13. Conclusão

A modelagem apresentada representa a estrutura inicial do sistema proposto. Ela demonstra os principais usuários, funcionalidades, informações e fluxos necessários para solucionar o problema identificado na primeira etapa.

A modelagem poderá ser aprimorada durante a etapa de desenvolvimento, conforme novas necessidades forem identificadas.


https://trello.com/b/E3lhXEAU/sistema-de-controle-de-presenca
