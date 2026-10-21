# The Dev News · blog responsivo

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![Sem framework](https://img.shields.io/badge/sem_framework-só_HTML_e_CSS-555)

Página de um blog de tecnologia feita **só com HTML e CSS**, sem framework e sem JavaScript, fiel a um protótipo do [Figma](https://www.figma.com/design/4JJ2iYIuL7FW1AQo6JYwl8) e funcionando do celular até monitor ultrawide.

Desafio de HTML e CSS da formação **Engenheiro de Software (Escola DNC)**, entregue e aprovado na avaliação do projeto.

<p align="center">
  <img src="docs/desktop.png" alt="Layout desktop" width="70%">
  &nbsp;
  <img src="docs/mobile.png" alt="Layout mobile" width="20%">
</p>

## Como o layout se adapta

| Tela | Breakpoint | Layout |
|---|---|---|
| Mobile | até 48rem | uma coluna, tudo empilhado |
| Tablet | 48rem a 64rem | posts em grid de 2 colunas, sidebar abaixo |
| Desktop | a partir de 64rem | posts à esquerda, sidebar fixa à direita |
| Ultrawide | a partir de 160rem | conteúdo centralizado com largura máxima |

Breakpoints em `rem` e não em `px`: se a pessoa aumenta a fonte do navegador, o layout muda junto em vez de quebrar.

## O que tem de cuidado aqui

- **Grid para a estrutura, Flexbox para os componentes.** O esqueleto da página (posts + sidebar) é CSS Grid. Dentro dos cards e da navegação, Flexbox.
- **HTML semântico.** `header`, `nav`, `main`, `article`, `aside` e `footer` no lugar de `div` genérica, o que ajuda leitor de tela e SEO.
- **Acessibilidade básica feita direito.** Link "Pular para o conteúdo" para quem navega pelo teclado e `aria-label` na navegação.
- **Unidades relativas** (`rem`/`em`) em tamanhos e espaçamentos.

## O que aprendi

- Transformar um protótipo do Figma em página real, medida por medida
- Quando usar Grid e quando usar Flexbox
- Pensar mobile-first e organizar media queries por faixa de tela
- Que acessibilidade começa na estrutura do HTML, não no fim do projeto

## Rodando

Não precisa instalar nada:

```bash
git clone https://github.com/lucas-gonzales-dev/blog-responsivo.git
cd blog-responsivo
# abra o index.html no navegador
```

---

Feito por **Lucas Leite Gonzales** · [LinkedIn](https://www.linkedin.com/in/lucas-leite-gonzales-dev/)
