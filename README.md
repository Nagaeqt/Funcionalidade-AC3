# 💪 PowerGym - Agendamento de Treinos com Personal

O **PowerGym** é um sistema web desenvolvido para gerenciamento de treinos e personal trainers.

Esta funcionalidade implementa o sistema de **agendamento de treinos com personal trainer**, permitindo que usuários escolham um profissional, selecionem horários e realizem agendamentos personalizados.

Projeto acadêmico desenvolvido para o curso de **Análise e Desenvolvimento de Sistemas (ADS)** da **Faculdade Impacta**.

---

# 👨‍💻 Autor

**Lucas Ryan Lima Malmagro - RA 2401867**

Projeto desenvolvido para fins educacionais.

---

# 📌 Objetivo da Funcionalidade

A funcionalidade de **agendamento de treinos** foi criada para permitir que usuários agendem aulas com personal trainers cadastrados no sistema.

O sistema permite:

- selecionar um personal trainer
- escolher data do treino
- escolher horário do treino
- selecionar quantidade de aulas
- calcular automaticamente o valor total
- visualizar agendamentos realizados
- cancelar agendamentos

Cada aula possui duração de:

- **60 minutos**

O valor total é calculado automaticamente com base:

- no valor da aula do personal
- na quantidade de aulas selecionadas

---

# 🚀 Funcionalidades Implementadas

## 📅 Agendamento de treino

O usuário pode:

- selecionar um personal trainer
- escolher a data do treino
- escolher o horário inicial
- definir quantidade de aulas
- adicionar observações

O sistema calcula automaticamente:

- horário final
- valor total do treino

---

## 💰 Cálculo automático do valor

O sistema multiplica:

valor da aula × quantidade de aulas

Exemplo:

- aula = R$ 75,00
- 2 aulas = R$ 150,00

---

## 🗂 Listagem de agendamentos

Após o cadastro, os agendamentos ficam visíveis na tela.

Informações exibidas:

- personal selecionado
- data do treino
- horário inicial
- horário final
- quantidade de aulas
- duração total
- valor total
- observações

---

## ❌ Cancelamento de agendamento

O usuário pode cancelar um treino agendado.

Ao cancelar:

- o registro é removido do banco de dados
- a tela atualiza automaticamente

---

# 🧩 Arquitetura da Funcionalidade

A funcionalidade segue arquitetura em **3 camadas**.

---

# 🎨 Front-end

Responsável pela interface visual do sistema.

Arquivos disponíveis em:

frontend

Tecnologias utilizadas:

- HTML
- CSS
- JavaScript

Funcionalidades da interface:

- seleção de personal trainer
- calendário para escolha da data
- seletor de horário
- cálculo automático do valor
- listagem de agendamentos
- cancelamento de treino

---

# ⚙ Back-end

Responsável pela lógica da aplicação.

Arquivos disponíveis em:

backend

Tecnologias utilizadas:

- Node.js
- Express

Responsabilidades:

- cadastro de agendamentos
- listagem de agendamentos
- cancelamento de treino
- cálculo de horários
- integração com PostgreSQL

---

# 🗄 Banco de Dados

Responsável pelo armazenamento persistente das informações.

Scripts disponíveis em:

banco

Tecnologia utilizada:

- PostgreSQL

---

# 🗄 Estrutura da Tabela de Agendamentos

Tabela principal:

agendamentos

Campos principais:

- id
- usuario_id
- personal_id
- data_agendamento
- horario_inicio
- horario_fim
- quantidade_aulas
- duracao_aula
- valor_unitario
- valor_total
- observacoes
- status
- created_at

---

# 🛠 Tecnologias Utilizadas

## Front-end

- HTML
- CSS
- JavaScript

## Back-end

- Node.js
- Express

## Banco de Dados

- PostgreSQL

## Ferramentas

- VS Code
- Git
- GitHub
- pgAdmin
- Thunder Client

---

# 📁 Estrutura do Projeto

powergym

├── backend  
│   ├── src  
│   │   ├── controllers  
│   │   │   └── agendamentoController.js  
│   │   │  
│   │   ├── routes  
│   │   │   └── agendamentoRoutes.js  
│   │   │  
│   │   └── server.js  

├── frontend  
│   ├── css  
│   │   └── style.css  
│   │  
│   ├── js  
│   │   └── agendamentos.js  
│   │  
│   └── agendamentos.html  

├── banco  
│   └── create_database.sql  

├── README.md  
└── LICENSE  

---

# 📡 Rotas da API

## Criar agendamento

POST /agendamentos

---

## Listar agendamentos

GET /agendamentos

---

## Cancelar agendamento

DELETE /agendamentos/:id

---

# 📚 Disciplina

Projeto desenvolvido para a disciplina:

Software Product

Curso:

Análise e Desenvolvimento de Sistemas (ADS)  
Faculdade Impacta

---

# 📄 Licença

Este projeto está sob a licença:

MIT License
