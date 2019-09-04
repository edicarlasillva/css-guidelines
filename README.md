# Guia de estilo CSS

Uma abordagem para escrever CSS gerenciável e escalável.

## Tópicos

## Terminologia

### Regra

Uma "regra" de CSS sempre começa com um "seletor" (ou grupo de seletores) que define a quais elementos HTML ele se aplica. Após o seletor, temos um bloco de declarações de "propriedades" e seus respectivos valores.

**Exemplo:**

```css
.header {
  color: #414141;               
  background-color: #EEEEEE;   
}
```

### Seletores

Os seletores determinam quais elementos na árvore de DOM serão estilizados pelas propriedades definidas.

**Exemplos:**

```css
.title {
  /* ... */
}

[aria-hidden] {
  /* ... */
}
```

### Propriedades

As propriedades são pares de chave-valor, onde uma regra pode conter uma ou mais declaração de propriedades.

**Exemplo:**

```css
/* some selector */ {
  background: #f1f1f1;
  color: #e18728;
}
```

## CSS

### Formato

- Use 2 espaços para identação.
- Prefira dashes `(-)` no lugar de camelCasing em nomes de classes.
- Não use seletores `ID`.
- Quando usar múltiplos seletores em uma regra, coloque cada um em uma linha.
- Coloque um espaço antes da abertura de chaves `{`.
- Em propriedades, coloque um espaço depois, mas não antes do caractere `:` (dois-pontos).
- Coloque chave de fechamento `}` em uma nova linha.
- Coloque linhas em branco entre declarações de regra.

**Exemplo:**

```css
.btn {
  border-radius: 50%;
  border: 2px solid white;
}

.btn:disabled,
.btn.btn-disabled {
  /* ... */
}
```

### Comentários

- Deixe um comentário sempre que o trecho não seja óbvio apenas a partir do código
- Prefira comentários em uma única linha

## BEM

A metodologia Block, Element, Modifier (comumente referida como BEM ) é uma convenção de nomenclatura popular para classes em HTML e CSS. Desenvolvido pela equipe da Yandex, seu objetivo é ajudar os desenvolvedores a entender melhor o relacionamento entre o HTML e o CSS em um determinado projeto.

A convenção de nomenclatura segue o padrão abaixo:

```css
.block {

}
.block__element {

}
.block--modifier {

}
```

- [Artigo sobre o BEM](https://css-tricks.com/bem-101/)
