# Portfólio — David Jorshuam

Site pessoal: https://djorshuam.github.io/portfolio/

Página única em HTML, CSS e JavaScript puro, sem build.

A seção "Pergunte sobre o David" responde perguntas em português: divide o
portfólio em trechos, busca os mais relevantes (BM25 com sinônimos, direto no
navegador) e mostra cada trecho com link para a seção de origem. É a parte de
recuperação de um RAG, sem texto gerado por IA, então não inventa nada; quando
não acha, diz que não encontrou. A aba SQL aceita consultas de leitura:

```sql
SELECT nome, status FROM projetos WHERE tipo = 'corporativo';
SELECT categoria, COUNT(*) FROM skills GROUP BY categoria ORDER BY count(*) DESC;
```

Este repositório é publicado automaticamente a partir de um repositório
privado; mudanças feitas direto aqui são sobrescritas na próxima publicação.

Rodar localmente: `python3 -m http.server 8000` e abrir http://localhost:8000
