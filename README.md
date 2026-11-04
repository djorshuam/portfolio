# Portfólio — David Jorshuam

Site pessoal: https://djorshuam.github.io/portfolio/

Página única em HTML, CSS e JavaScript puro, sem build. O terminal do topo
responde a comandos (`help`, `tabelas`, `projetos`) e a SQL de leitura sobre o
próprio portfólio:

```sql
SELECT nome, status FROM projetos WHERE tipo = 'corporativo';
SELECT categoria, COUNT(*) FROM skills GROUP BY categoria ORDER BY count(*) DESC;
```

Este repositório é publicado automaticamente a partir de um repositório
privado; mudanças feitas direto aqui são sobrescritas na próxima publicação.

Rodar localmente: `python3 -m http.server 8000` e abrir http://localhost:8000
