# Dev Portfolio

Projeto simples de portfólio pessoal criado como atividade da disciplina de HTML/CSS do 1º ano do curso de Informática.

## Descrição

Este repositório contém uma página estática que apresenta um layout de portfólio com seções para Início, Sobre, Projetos e Contato. O objetivo é praticar estruturas HTML semânticas e estilização com CSS, trabalhando também com imagens, formulários e incorporação de mapa (iframe).

A página foi desenvolvida pensando em clareza visual e prática didática para a disciplina.

## Tecnologias

- HTML5
- CSS3
- Imagens (WebP / PNG / JPG)
- Nenhuma dependência ou build system — página estática

## Como executar

Método rápido (abrir arquivo):

1. Abra o arquivo `index.html` no navegador (duplo-clique ou arrastar para o navegador).

Método via servidor local (recomendado para evitar restrições com iframes ou CORS):

- Usando Python (se tiver o Python instalado):

```powershell
cd "c:\Users\allex\Documents\Dev\dev-portifolio"
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

## Como personalizar a imagem e a cor de overlay da seção Início

Abra `css/style.css` e procure pelo seletor `#inicio` e `#inicio::before`.

- Para trocar a imagem de fundo, altere:

```css
#inicio {
  background-image: url('../images/bg_hero_1.webp');
}
```

Substitua pelo caminho da sua imagem, por exemplo: `url('../images/minha_imagem.jpg')`.

- Para alterar a cor e a opacidade do overlay, ajuste `background-color` no pseudo-elemento:

```css
#inicio::before {
  background-color: rgba(174, 32, 157, 0.6); /* R, G, B, opacidade */
}
```

Aumente ou diminua o último valor (0.0 a 1.0) para alterar a transparência.

Alternativa sem pseudo-elemento (usando gradiente):

```css
#inicio {
  background-image: linear-gradient(rgba(174,32,157,0.55), rgba(174,32,157,0.55)), url('../images/bg_hero_1.webp');
}
```

## Observações e boas práticas

- `background-attachment: fixed;` pode causar comportamento estranho em dispositivos móveis. Se notar problemas em celulares, remova essa propriedade ou use media queries.
- O `nav` foi definido com `position: fixed` e `z-index` para garantir que fique acima do overlay. Se for preciso, ajuste `padding` e `z-index` em `css/style.css` para adequar ao seu layout.
- O formulário de contato não possui backend — para torná-lo funcional, conecte a um servidor ou use um serviço de terceiros (Formspree, Netlify Forms, etc.).

## Contribuições

Esta é uma atividade de disciplina; contribuições são bem-vindas para melhorias visuais, responsividade ou acessibilidade. Abra issues ou envie pull requests se quiser colaborar.

## Licença

Sinta-se livre para usar este projeto como referência para estudos. Não há restrições formais de licença aqui — se desejar, adicione um arquivo LICENSE com a licença apropriada.

---

Desenvolvido por Manoel Carvalho — atividade da disciplina de HTML/CSS (1º ano, curso de Informática).