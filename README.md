# Dev Portfolio

Projeto simples de portfólio pessoal criado como atividade da disciplina de HTML/CSS do 1º ano do curso de Informática.

## Descrição

Este repositório contém uma página estática que apresenta um layout de portfólio com seções para Início, Sobre, Projetos e Contato. O objetivo é praticar estruturas HTML semânticas e estilização com CSS, trabalhando também com imagens, formulários e incorporação de mapa (iframe).

A página foi desenvolvida pensando em clareza visual e prática didática para a disciplina.

## Tecnologias

- HTML5
- CSS3

## Como executar

Método rápido (abrir arquivo):

1. Abra o arquivo `index.html` no navegador (duplo-clique ou arrastar para o navegador).

Método via servidor local (recomendado para evitar restrições com iframes ou CORS):

- Usando Python (se tiver o Python instalado):

```powershell
cd "/dev-portifolio"
python -m http.server 8000
```

Em seguida abra no navegador: `http://localhost:8000`

- Ou use a extensão "Live Server" do VS Code para servir o projeto localmente.

## Estrutura do projeto

- `index.html` — Página principal com as seções do portfólio.
- `css/style.css` — Estilos do site (background, overlay, layout das seções, nav, formulários).
- `images/` — Imagens usadas (fotos, background e thumbnails de projetos).
- `README.md` — Este arquivo.

## Seções principais

- Início (`#inicio`): Cabeçalho com título, imagem de background e overlay colorida para melhorar legibilidade.
- Sobre (`#sobre`): Foto e descrição pessoal / habilidades.
- Projetos (`#projetos`): Cards com imagens e descrições de projetos de exemplo.
- Contato (`#contato`): Iframe do Google Maps e formulário de contato (apenas front-end; sem envio backend).

## Contribuições

Esta é uma atividade de disciplina; contribuições são bem-vindas para melhorias visuais, responsividade ou acessibilidade. Abra issues ou envie pull requests se quiser colaborar.

## Licença

Sinta-se livre para usar este projeto como referência para estudos. Não há restrições formais de licença aqui — se desejar, adicione um arquivo LICENSE com a licença apropriada.

---

Desenvolvido por Manoel Carvalho — atividade da disciplina de HTML/CSS (1º ano, curso de Informática).