---
título: Mantenha a proporção de uma DIV
tags: dica, intermediário 
---

O conceito principal dessa dica é usar um valor de porcentagem no `padding-top`, pois ele se baseia no valor de `width` do elemento.

Ou seja: 

```css
  .el {
    width: 500px;
    padding-top: 100%; /* Transformaria esse elemento em 500x500 */
    padding-top: 50%;  /* Transformaria esse elemento em 500x250 */
  }
```

Se você quer que um vídeo, por exemplo, mantenha a proporção de 16:9, você pode dar à ele um padding de: `56,25%`.

```css
  .video-wrapper {
    width: 1400px;
    padding-top: 56.25%; /* Proporção: 16:9 */
    padding-top: 62.5%;  /* Proporção: 16:10 */
  }
```


Leia mais nesse artigo: https://css-tricks.com/aspect-ratio-boxes/ (Inglês)
