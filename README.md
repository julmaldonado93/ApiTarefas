# API Django REST Framework - Gerenciador de Tarefas

> ⚠️ Este projeto foi desenvolvido exclusivamente para fins de estudo e prática,
> como parte do meu aprendizado em Python, Django e Django REST Framework.

## 📋 Sobre o Projeto

API REST de gerenciamento de tarefas desenvolvida com Django REST Framework.
Projeto complementar ao [crud-django-tarefas](https://github.com/julmaldonado93/crud-django-tarefas),
evoluindo de um CRUD tradicional com templates HTML para uma API REST com JSON.

## 🚀 Funcionalidades

- Listar todas as tarefas
- Criar nova tarefa
- Detalhar uma tarefa
- Editar tarefa (completa ou parcial)
- Remover tarefa

## 🛠️ Tecnologias Utilizadas

- Python
- Django
- Django REST Framework
- SQLite

## 📦 Como rodar o projeto

1. Clone o repositório:
```bash
git clone https://github.com/julmaldonado93/api-django-tarefas.git
```

2. Crie e ative o ambiente virtual:
```bash
python -m venv .venv
.venv\Scripts\activate
```

3. Instale as dependências:
```bash
pip install django djangorestframework
```

4. Rode as migrações:
```bash
python manage.py migrate
```

5. Inicie o servidor:
```bash
python manage.py runserver
```

6. Acesse no navegador:
```
http://127.0.0.1:8000/api/
```

## 🔗 Endpoints

| Método | URL | Descrição |
|--------|-----|-----------|
| GET | `/api/tarefas/` | Lista todas as tarefas |
| POST | `/api/tarefas/` | Cria uma nova tarefa |
| GET | `/api/tarefas/{id}/` | Detalha uma tarefa |
| PUT | `/api/tarefas/{id}/` | Edita uma tarefa |
| PATCH | `/api/tarefas/{id}/` | Edita parcialmente uma tarefa |
| DELETE | `/api/tarefas/{id}/` | Remove uma tarefa |

## 📌 Modelo de Dados

| Campo | Tipo | Descrição |
|-------|------|-----------|
| nome | CharField | Nome da tarefa |
| descricao | TextField | Detalhes da tarefa (opcional) |
| completo | BooleanField | Status da tarefa (True/False) |
| data_criacao | DateTimeField | Gerada automaticamente |

## 👨‍💻 Autor

Julio Maldonado - [GitHub](https://github.com/julmaldonado93)
