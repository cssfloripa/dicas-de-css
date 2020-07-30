---
título: Como esconder elementos Checkbox e Radio com acessibilidade
tags: intermediario, accessibilidade, checkbox, radio
---

Se você quer que algum elemento HTML fique escondido, mas permaneça com acessibilidade, nunca use `display: none;` ou `visibility: hidden;`. Essas propriedades escondem o elemento removendo-os do DOM e da **árvore de acessibilidade**.

### Como visualmente esconder qualquer elemento (texto) de maneira inclusiva.
*Suporte para IE9+* - **Fonte:** https://www.scottohara.me/blog/2017/04/14/inclusively-hidden.html

```css
.visually-hide {
    clip: rect(0 0 0 0);
    clip-path: inset(100%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap; 
    width: 1px;
}
```

### Escondendo Checkboxes de maneira inclusiva

```css
.checkbox-parent {
    /* Crie um posicionamento "relative" para o elemento pai da Checkbox, de preferencia, o Label */
    position: relative;

    /* Outros estilos do label vem aqui */
}

.checkbox-parent input[type="checkbox"] {
    /* Remover o checkbox do flow */
    position: absolute;

    /* Esconder o checkbox visualmente */
    opacity: 0;

    /* Ajuste o tamanho e posição, se necessário */
    width: 1em;
    height: 1em;

    /* Posição do Checkbox escondido */
    top: ...;
    left: ...;

    /* Em algumas ocasiões, você precisará definir um z-index */
    z-index: ...;
}
```

----

**Fonte:** [Blog da Sara Soueidan](https://www.sarasoueidan.com/blog/inclusively-hiding-and-styling-checkboxes-and-radio-buttons/) 
