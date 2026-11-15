# 📖 Guia Rápido de Consulta — Curso PyDjango Edu

Material de apoio oficial do projeto **BookShelf**.

---

## 1. Comandos Essenciais (Terminal & Django)

| Ação | Comando |
| :--- | :--- |
| Criar ambiente virtual | `python -m venv venv` |
| Ativar venv (Linux/Mac) | `source venv/bin/activate` |
| Ativar venv (Windows) | `.\venv\Scripts\Activate.ps1` |
| Instalar Django | `pip install django` |
| Salvar dependências | `pip freeze > requirements.txt` |
| Criar novo projeto | `django-admin startproject config .` |
| Criar novo aplicativo | `python manage.py startapp livros` |
| Rodar servidor local | `python manage.py runserver` |
| Criar migrações | `python manage.py makemigrations` |
| Aplicar migrações | `python manage.py migrate` |
| Criar superusuário | `python manage.py createsuperuser` |
| Abrir shell interativo | `python manage.py shell` |
| Executar testes | `python manage.py test` |

---

## 2. Principais Métodos HTTP (Aula 03)

- **GET**: Solicita dados de um recurso (ex: abrir a lista de livros).
- **POST**: Envia dados para criar um novo recurso (ex: cadastrar um livro).
- **PUT / PATCH**: Atualiza um recurso existente.
- **DELETE**: Remove um recurso.

### Códigos de Status Mais Comuns
- `200 OK`: Requisição bem-sucedida.
- `302 Found`: Redirecionamento (comum após envio de formulários).
- `403 Forbidden`: Acesso negado (ex: falta de permissão ou token CSRF inválido).
- `404 Not Found`: Página ou registro não encontrado.
- `500 Internal Server Error`: Erro interno no código Python/Django.

---

## 3. Consultas Rápidas no Django ORM (Aula 20)

Supondo o modelo `Livro`:
```python
# Buscar todos os livros
Livro.objects.all()

# Buscar um livro específico pelo ID (chave primária)
Livro.objects.get(id=1)

# Filtrar livros por condição (ex: gênero)
Livro.objects.filter(genero__nome="Ficção")

# Busca parcial sem diferenciar maiúsculas/minúsculas
Livro.objects.filter(titulo__icontains="python")

# Ordenar resultados (use '-' para ordem decrescente)
Livro.objects.order_by("-ano_publicacao")

# Contar registros
Livro.objects.count()
