# 🎓 Sistema de Gestão Escolar EJA (Complementar)

> **Solução complementar leve, responsiva e de baixo custo para administração da Educação de Jovens e Adultos (EJA).**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Type](https://img.shields.io/badge/architecture-SPA-emerald.svg)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-black.svg)
![Database](https://img.shields.io/badge/database-Supabase%20PostgreSQL-green.svg)

---

## 📌 Sobre o Projeto

Este software foi desenvolvido sob encomenda para suprir necessidades administrativas e pedagógicas específicas do programa de **Educação de Jovens e Adultos (EJA)** em uma instituição de ensino.

Como a escola já utiliza um sistema proprietário legado para a gestão escolar principal, este projeto atua de forma **complementar e especializada**[cite: 1]. Além disso, devido ao **orçamento reduzido**[cite: 1], foi desenhada uma arquitetura *Zero-Server Overhead*, utilizando **SPA (Single Page Application)**[cite: 1] hospedada no **GitHub Pages**[cite: 1] e utilizando o **Supabase**[cite: 1] como banco de dados e autenticação Serverless (BaaS).

---

## ⚡ Principais Funcionalidades

- 📊 **Dashboard Dinâmico:** Visualização rápida de métricas gerais da escola, alertas em tempo real de baixa frequência (< 85%) e alunos com pendências em notas.
- 🎓 **Gestão Completa de Alunos (CRUD):**
  - Cadastro completo com foto de perfil, RA, Matrícula, Série e Telefone[cite: 1].
  - Suporte a registro de **NEE** (Necessidades Educacionais Especiais)[cite: 1].
  - Busca inteligente, filtros por status e paginação otimizada.
  - Exportação direta de dados dos alunos para **Excel (.xlsx)**.
- 📅 **Controle de Presença & Plantão de Dúvidas:**
  - **Chamada Diária:** Registro de presença/ausência com salvamento em tempo real[cite: 1].
  - **Plantão:** Registro e acompanhamento de atendimento aos estudantes.
  - **Calendário e Frequência:** Grade mensal visual do percentual de presença.
- 📝 **Notas e Atividades:**
  - Lançamento simplificado por disciplinas e itinerários[cite: 1].
  - Média calculada automaticamente com sistema de *lock* (bloqueio de edição simultânea) para evitar conflitos de professores.
- 📑 **Relatórios & Emissão de PDF:**
  - Geração de boletins e fichas do aluno formatados para impressão em PDF[cite: 1].
  - Exportação em lote compactada em arquivo `.ZIP`.
- 💬 **Módulo Buscativa (WhatsApp):**
  - Botão de ação rápida integrado ao WhatsApp para contato direto com alunos em risco de evasão[cite: 1].
- 🔐 **Controle de Acesso e Segurança:**
  - Níveis de acesso distintos (Administrador vs. Professor)[cite: 1].
  - Suporte a modo noturno (Dark Mode)[cite: 1], Backup/Restauração de dados em JSON e Log de Atividades[cite: 1].

---

## 🛠️ Tecnologias Utilizadas

### **Frontend**
- **HTML5 & CSS3 Variables** (Design customizado com temas Claro/Escuro)
- **Bootstrap 5.3** & **FontAwesome 6** (Interface responsiva e moderna)
- **JavaScript Vanilla (ES6+)** (Sem frameworks pesados, garantindo carregamento ultrarrápido)
- **PWA (Progressive Web App):** Instalável em dispositivos móveis e desktops.
- **Bibliotecas Auxiliares:** `SheetJS` (Excel), `html2pdf.js` (PDF) e `JSZip`.

### **Backend & Infraestrutura**
- **Hosting:** [GitHub Pages](https://pages.github.com/) (Hospedagem estática gratuita com SSL)
- **Database & Auth:** [Supabase](https://supabase.com/) (PostgreSQL relacional com GoTrue Auth)

---

## 🚀 Como Executar o Projeto Localmente

Como o projeto é uma SPA pura, não é necessário instalar dependências de Node.js ou compilar pacotes.

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)
   cd nome-do-repositorio
