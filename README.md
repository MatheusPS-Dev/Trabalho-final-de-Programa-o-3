# Entre Páginas — Clube de Leitura

Trabalho Final da disciplina de **Programação III**  
**Curso:** Tecnologia em Análise e Desenvolvimento de Sistemas — IFRO Campus Ariquemes  
**Aluno:** Matheus P. S. ([@MatheusPS-Dev](https://github.com/MatheusPS-Dev))  

🌐 **Site em produção:** [https://matheuspereirasantos2308.pythonanywhere.com/](https://matheuspereirasantos2308.pythonanywhere.com/)

---

## Sobre o Projeto

O **Entre Páginas** é um clube de leitura virtual desenvolvido em Django. A aplicação permite explorar livros por gênero, consultar avaliações da comunidade e ver a nota média de cada obra. Usuários cadastrados podem publicar resenhas (com nota de 1 a 5) e adicionar novos títulos ao acervo.

### Principais Recursos
- **Catálogo Literário:** Navegação com busca por título/autor e filtros por categoria.
- **Avaliações e Notas:** Resenhas com notas de 1 a 5, com cálculo automático da média e resumo de notas.
- **Autenticação:** Cadastro de novos leitores, login/logout e área "Minhas Resenhas".
- **Permissões:** Apenas o autor de uma resenha pode editá-la ou excluí-la. Cadastro de livros e resenhas restrito a usuários logados.
- **Painel Administrativo:** Django Admin com busca, filtros e gerenciamento completo do acervo.

---

## Tecnologias Utilizadas
- **Python 3.12**
- **Django 5.2**
- **SQLite**
- **HTML5, CSS3 e JavaScript**

---

## Como Executar Localmente

```bash
# 1. Clonar o repositório
git clone https://github.com/MatheusPS-Dev/Trabalho-final-de-Programa-o-3.git
cd Trabalho-final-de-Programa-o-3

# 2. Criar e ativar o ambiente virtual
python -m venv .venv
.venv\Scripts\activate      # Windows
# source .venv/bin/activate # Linux/macOS

# 3. Instalar as dependências
pip install -r requirements.txt

# 4. Executar as migrações do banco
python manage.py migrate

# 5. (Opcional) Carregar dados de exemplo (livros e resenhas)
python manage.py popular_dados

# 6. Criar um superusuário para o admin
python manage.py createsuperuser

# 7. Iniciar o servidor de desenvolvimento
python manage.py runserver
```

Acesse em: `http://127.0.0.1:8000`

---

## Testes Automatizados

Para rodar os testes unitários da aplicação:
```bash
python manage.py test
```
