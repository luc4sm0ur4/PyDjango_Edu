# 📚 BookShelf — Sistema de Biblioteca Digital

![Python](https://img.shields.io/badge/Python-3.11+-blue?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-5.0+-092E20?style=for-the-badge&logo=django&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em%20Produção-yellow?style=for-the-badge)

Repositório oficial do projeto integrador **BookShelf**, desenvolvido ao longo das **36 videoaulas (12 horas)** do curso **Desenvolvimento Web com Python e Django**, publicado no canal **PyDjango Edu**.

> 🎓 **Contexto Acadêmico:** Este projeto integra as atividades da disciplina de **Práticas Extensionistas 3**, sob orientação do professor **Patrick Letouze**.

---

## 🎯 Sobre o Projeto

O **BookShelf** é uma aplicação web de gerenciamento de biblioteca digital e controle de leitura pessoal. Ele foi projetado para evoluir progressivamente a cada módulo do curso, permitindo que o estudante aprenda na prática desde os fundamentos do protocolo HTTP até a preparação da aplicação para ambiente de produção.

### ✨ Funcionalidades Implementadas

- **Catálogo de Livros:** Cadastro, listagem, detalhamento, edição e exclusão (CRUD completo) de livros, autores e gêneros.
- **Gestão de Mídia:** Upload e exibição de capas de livros.
- **Autenticação e Permissões:** Sistema de cadastro, login, logout, sessões e controle de níveis de acesso.
- **Biblioteca Individual:** Associação de livros a cada usuário com controle de *status de leitura* (Quero Ler, Lendo, Lido) e avaliações.
- **Busca e Navegação:** Pesquisa dinâmica, filtros por categoria e paginação de resultados.
- **Painel Administrativo:** Área de gestão personalizada via Django Admin.
- **Segurança e Qualidade:** Proteção CSRF, validação de formulários (`ModelForms`), suíte de testes automatizados e configurações separadas para produção.

---

## 🗂️ Estrutura do Curso (16 Módulos)

| Bloco | Aulas | Tema Principal |
| :--- | :---: | :--- |
| **01** | 01 – 03 | Apresentação, Arquitetura Web e Protocolo HTTP |
| **02** | 04 – 05 | Configuração do Ambiente e Ambientes Virtuais (`venv`) |
| **03** | 06 – 08 | Fundamentos de Python e Orientação a Objetos para Web |
| **04** | 09 – 13 | Introdução ao Django, Estrutura, URLs e Views |
| **05** | 14 – 16 | Sistema de Templates, Herança e Construção da Interface |
| **06** | 17 – 22 | Modelagem de Banco de Dados, Migrations, ORM e CRUD |
| **07** | 23 – 25 | Formulários, Validações (`ModelForms`) e Upload de Imagens |
| **08** | 26 – 28 | Autenticação, Sessões, Permissões e Django Admin |
| **09** | 29 – 31 | Busca, Filtros, Paginação, Mensagens e Biblioteca Individual |
| **10** | 32 – 34 | Organização de Código, Segurança Básica e Testes |
| **11** | 35 – 36 | Configurações de Produção e Checklist Pré-Deploy |

---

## 🚀 Como Executar o Projeto Localmente

Siga os passos abaixo para rodar o projeto na sua máquina:

### 1. Clone o repositório

```bash
git clone https://github.com/SEU-USUARIO/pydjango-edu-bookshelf.git
cd pydjango-edu-bookshelf
```

### 2. Crie e ative o ambiente virtual

**No Linux/macOS:**

```bash
python3 -m venv venv
source venv/bin/activate
```

**No Windows (PowerShell):**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Configure as variáveis de ambiente e o banco de dados

```bash
cp .env.example .env
python manage.py migrate
```

### 5. Crie um superusuário (opcional, para acessar `/admin`)

```bash
python manage.py createsuperuser
```

### 6. Inicie o servidor de desenvolvimento

```bash
python manage.py runserver
```

Acesse no navegador: `http://127.0.0.1:8000/`

---

## 🌿 Navegando pelo Código por Aula

Para facilitar seus estudos, o código de cada aula está marcado com **Tags** no Git. Caso queira ver exatamente como o projeto estava ao final de uma aula específica (ex: Aula 20), execute:

```bash
git checkout aula-20
```

Para voltar à versão mais recente do projeto:

```bash
git checkout main
```

---

## 👨‍💻 Equipe de Desenvolvimento e Docência

- **Lucas José de Sousa Gomes** — *Coordenação, Fundamentos, Backend e Banco de Dados*
- **Lucas Carvalho da Luz Moura** — *Frontend, Templates, Formulários e Funcionalidades*
- **Daniel Viana de Lima** — *Autenticação, Segurança, Testes e Controle de Qualidade*

---

## 📄 Licença

Este projeto é distribuído sob a licença MIT para fins educacionais. Sinta-se à vontade para estudar, modificar e evoluir o código!
