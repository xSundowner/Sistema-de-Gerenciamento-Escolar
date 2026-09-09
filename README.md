# 🎓 Sistema de Gestão Escolar EJA

> Solução complementar, leve, responsiva e de baixo custo para a administração da **Educação de Jovens e Adultos (EJA)**.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Architecture](https://img.shields.io/badge/architecture-SPA-emerald.svg)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-black.svg)
![Database](https://img.shields.io/badge/database-Supabase%20PostgreSQL-green.svg)

---

## 📌 Sobre o Projeto

O **Sistema de Gestão Escolar EJA** foi desenvolvido sob encomenda para atender necessidades administrativas e pedagógicas específicas do programa de **Educação de Jovens e Adultos (EJA)** de uma instituição de ensino.

Como a escola já utiliza um sistema proprietário legado para sua gestão escolar principal, esta aplicação funciona como uma **solução complementar e especializada**, concentrando recursos específicos para o acompanhamento dos alunos, frequência, notas, atividades e processos administrativos relacionados à EJA.

Considerando também a necessidade de manter os custos operacionais reduzidos, o projeto utiliza uma arquitetura **Serverless / Zero-Server Overhead**, baseada em uma **SPA (Single Page Application)** hospedada gratuitamente no **GitHub Pages**, utilizando o **Supabase** como plataforma de banco de dados e autenticação.

### 🎯 Objetivos

* Centralizar informações específicas da EJA.
* Simplificar tarefas administrativas e pedagógicas.
* Facilitar o acompanhamento de frequência e desempenho dos alunos.
* Reduzir processos manuais e utilização de planilhas.
* Manter uma infraestrutura de baixo custo e fácil manutenção.
* Disponibilizar acesso responsivo em computadores, tablets e dispositivos móveis.

---

## ⚡ Principais Funcionalidades

### 📊 Dashboard

* Visualização rápida das principais métricas da escola.
* Indicadores de frequência dos alunos.
* Alertas para alunos com frequência abaixo de **85%**.
* Identificação de alunos com pendências relacionadas às notas.
* Atualização das informações de forma dinâmica.

### 🎓 Gestão de Alunos

Sistema completo de gerenciamento de alunos (CRUD):

* Cadastro e edição de informações pessoais.
* Foto de perfil.
* Registro Acadêmico (RA).
* Número de matrícula.
* Série.
* Telefone.
* Registro de **NEE (Necessidades Educacionais Especiais)**.
* Busca inteligente.
* Filtros por status.
* Paginação otimizada.
* Exportação dos dados para **Excel (.xlsx)**.

### 📅 Controle de Presença

* Chamada diária dos alunos.
* Registro de presença e ausência.
* Salvamento das informações em tempo real.
* Consulta do histórico de frequência.
* Visualização mensal do percentual de presença.
* Acompanhamento individual da frequência.

### 💬 Plantão de Dúvidas

* Registro de atendimentos realizados.
* Acompanhamento dos estudantes atendidos.
* Histórico dos atendimentos.
* Organização das informações por aluno e data.

### 📝 Notas e Atividades

* Lançamento de notas por disciplina.
* Organização por disciplinas e itinerários.
* Registro de atividades.
* Cálculo automático de médias.
* Sistema de **lock** para evitar conflitos durante a edição simultânea por professores.

### 📑 Relatórios e PDFs

* Geração de boletins.
* Geração de fichas individuais dos alunos.
* Documentos formatados para impressão.
* Exportação para **PDF**.
* Geração de relatórios em lote.
* Compactação de múltiplos documentos em arquivo **.ZIP**.

### 💬 Módulo Buscativa

Ferramenta voltada ao acompanhamento de alunos com risco de evasão:

* Identificação de alunos em situação de atenção.
* Ação rápida para contato.
* Integração com **WhatsApp**.
* Facilitação do processo de busca ativa e acompanhamento.

### 🔐 Controle de Acesso e Segurança

* Autenticação de usuários.
* Diferentes níveis de acesso:

  * **Administrador**
  * **Professor**
* Controle de permissões conforme o perfil.
* Log de atividades.
* Backup dos dados em **JSON**.
* Restauração de dados.
* Suporte a **Dark Mode**.

---

## 🛠️ Tecnologias Utilizadas

### Frontend

* **HTML5**
* **CSS3**
* **CSS Variables** para gerenciamento de temas.
* **Bootstrap 5.3** para interface responsiva.
* **Font Awesome 6** para ícones.
* **JavaScript Vanilla (ES6+)**.
* **PWA (Progressive Web App)** para instalação em desktops e dispositivos móveis.

### Bibliotecas

| Biblioteca       | Finalidade                                 |
| ---------------- | ------------------------------------------ |
| **SheetJS**      | Exportação e manipulação de arquivos Excel |
| **html2pdf.js**  | Geração de documentos PDF                  |
| **JSZip**        | Compactação de arquivos em `.ZIP`          |
| **Bootstrap**    | Componentes e responsividade da interface  |
| **Font Awesome** | Ícones da aplicação                        |

### Backend e Infraestrutura

* **GitHub Pages** — hospedagem estática gratuita com SSL.
* **Supabase** — plataforma Backend as a Service (BaaS).
* **PostgreSQL** — banco de dados relacional.
* **GoTrue Auth** — autenticação e gerenciamento de usuários.

---

## 🏗️ Arquitetura

A aplicação utiliza uma arquitetura **SPA (Single Page Application)**, mantendo a maior parte da lógica no frontend e utilizando o Supabase para os serviços de backend.

```text
┌──────────────────────────────┐
│         Usuário              │
│   Desktop / Tablet / Mobile  │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│       GitHub Pages           │
│      Frontend / SPA          │
│                              │
│ HTML + CSS + JavaScript      │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│          Supabase            │
│                              │
│  ┌──────────┐  ┌──────────┐ │
│  │PostgreSQL│  │   Auth   │ │
│  └──────────┘  └──────────┘ │
└──────────────────────────────┘
```

Essa abordagem elimina a necessidade de manter um servidor de aplicação próprio, reduzindo custos de infraestrutura e manutenção.

---

## 📱 Responsividade e PWA

A aplicação foi desenvolvida para funcionar em diferentes dispositivos e tamanhos de tela.

O suporte a **Progressive Web App (PWA)** permite que o sistema possa ser instalado como uma aplicação no:

* 💻 Windows
* 📱 Android
* 📱 iOS
* 🖥️ Outros dispositivos compatíveis

---

## 🚀 Deploy

O frontend pode ser hospedado diretamente através do **GitHub Pages**, eliminando custos de hospedagem tradicional.

O banco de dados e os serviços de autenticação são fornecidos pelo **Supabase**.

### Fluxo de publicação

```text
Código
   │
   ▼
GitHub Repository
   │
   ▼
GitHub Pages
   │
   ▼
Aplicação Web
   │
   ▼
Supabase
 ├── PostgreSQL
 └── Authentication
```

---

## 🔒 Segurança

A aplicação utiliza autenticação e controle de acesso para separar as permissões entre diferentes tipos de usuários.

O acesso aos dados deve ser protegido através das políticas de segurança do PostgreSQL/Supabase, utilizando **Row Level Security (RLS)** quando aplicável.

> **Importante:** credenciais, chaves privadas ou informações sensíveis do ambiente de produção não devem ser armazenadas diretamente no repositório.

---

## 📂 Estrutura do Projeto

Uma estrutura típica do projeto pode ser organizada da seguinte forma:

```text
/
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
│
├── components/
│
├── pages/
│
├── services/
│
├── index.html
├── manifest.json
├── service-worker.js
└── README.md
```

A estrutura pode variar conforme a organização atual do código-fonte.

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.

Consulte o arquivo [`LICENSE`](LICENSE) para obter mais informações.

---

## 👨‍💻 Desenvolvimento

Projeto desenvolvido como uma solução personalizada para apoiar os processos administrativos e pedagógicos da **Educação de Jovens e Adultos (EJA)**.

---
